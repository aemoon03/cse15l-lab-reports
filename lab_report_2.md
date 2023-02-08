# Lab Report 2: Servers and Bugs 
### Part 1: 
My code is as follows: 
![image](https://user-images.githubusercontent.com/112985603/215298655-d2dafe68-b45f-4158-82bb-ba7b11db3c09.png)
![image](https://user-images.githubusercontent.com/112985603/215298665-448d8d88-ab40-49b8-854d-4426d3c21ab4.png)
Here are screenshots of the actual webpage itself:\
![image](https://user-images.githubusercontent.com/112985603/215299123-4390da19-4f12-4b1a-970f-8a089990eb95.png)\
In this screenshot, the method *handleRequest* is being used. This method takes the argument of a URI (the url of the webpage), and if "add-message" is found in the url, then it adds the string after "s=" in the url to an ArrayList called inputs. After this, inputs is formatted into a String called *display*, which is then returned and put on the display of the webpage.\
![image](https://user-images.githubusercontent.com/112985603/215299185-aa15b794-78ea-438f-b793-e6b454d70f14.png)\
Here, essentially the same thing is happening. Only this time, inputs already has one element inside of it from the previous call, so the next input is printed on the line under it. 
### Part 2: 
The bug that I chose to look at was the bug in **LinkedListExamples.java**.\
Here is one input that induces failure:\
![image](https://user-images.githubusercontent.com/112985603/215389822-bce89127-377a-4497-afe6-3687c79cb75c.png)

Here is one input that does not induce failure:\
![image](https://user-images.githubusercontent.com/112985603/215389382-df45def5-0e8f-4297-a60d-51588127f88c.png)\
The symptom of this bug is that it causes an infinite loop:\
![image](https://user-images.githubusercontent.com/112985603/215389938-4b66d35c-6a68-42fa-8e7b-2da15733135a.png)\
(it never finishes running due to infinite loop)\
The reason that this bug occurs is that the code originally assigns n.next to a new node, therefore causing n.next to never be null, meaning that the while
loop will never terminate, as seen in the code below:\
![image](https://user-images.githubusercontent.com/112985603/215417153-f4a1e30f-79ae-4b6f-8f96-93c81a7b4b48.png)\
This can be fixed by putting the line *n.next = new Node(value, null)* outside of the while loop.\
![image](https://user-images.githubusercontent.com/112985603/215417520-d686366e-18b7-4aca-bb24-a20894fec18f.png)\
As we can see, the JUnit tests now run correctly:\
![image](https://user-images.githubusercontent.com/112985603/215417605-163974f7-e13e-4f39-80de-4daa5952729d.png)\
This approach to the fix is valid, as it will successfully append the node to the end, after having looped through the entirety of the list, rather than creating 
new nodes infintely. 
### Part 3:
One thing that I learned in lab that I didn't have prior knowledge of was being able to create web servers in Java. Previously, that connection just had never been
made in my mind. In addition to this, I didn't know that you could create a web server using your own local host, and then create your own port, and then modify different constants and variables by manipulating the path of the url. Also, I learned that when doing this through the ssh remote server, you can connect to other students' web servers by finding the ieng6 computer that their website is on, and then typing their port into the url. 
