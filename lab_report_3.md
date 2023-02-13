**Researching Commands**

The command that I chose to research was the *grep* command. 

**Command 1: -m**\
Example 1:\
![image](https://user-images.githubusercontent.com/112985603/218572203-2c50b054-e816-4c7f-a819-7b70971fa727.png)\
Example 2:\
![image](https://user-images.githubusercontent.com/112985603/218572278-1a6e46b4-b7a6-48d8-b90e-93b2544b3ce2.png)\
The -m option only shows the amount of entries desired from the grep command. For example, in example 1, the desired count was 8, so -m returned 8 results from grep. Likewise, the second example shows that *grep -m 3* returns three results. I found this example through the *grep --help* command. 

**Command 2: -l**\
Example 1:\
![image](https://user-images.githubusercontent.com/112985603/218574205-c2c27f11-f8bb-477d-a61d-bb45098aaa4a.png)\
Example 2:\
![image](https://user-images.githubusercontent.com/112985603/218575134-903340a4-a52c-405d-8bb7-4ed1601a883b.png)\
The -l option prints only the names of the files that contain matches from the grep search. I found this example through the *grep --help* command.

**Command 3: -L**\
Example 1:\
![image](https://user-images.githubusercontent.com/112985603/218574446-7da5b307-7972-451f-abed-d3e85457ac84.png)\
Example 2:\
![image](https://user-images.githubusercontent.com/112985603/218575245-9c54078c-f36d-400d-a935-4d75a044f0fd.png)\
The -L option does the opposite of the -l option, in that it prints only the names of files that are NOT a match from the grep search. I found this example through the *grep --help* command.

**Command 4: -c**\
Example 1:\
![image](https://user-images.githubusercontent.com/112985603/218575856-781193a9-ac7e-4f05-91de-55b5f660516d.png)\
Example 2:\
![image](https://user-images.githubusercontent.com/112985603/218576000-75d73401-5854-4650-bd68-f6e53133f1ab.png)\
the -c option lists all of the files, and then states how many times the search word occurs in each file. For example, in example 1, we can see that the word "Japan" is mentioned once in the file *written_2/non-fiction/OUP/Abernathy/ch9.txt:0*. I found this example through the *grep --help* command.
