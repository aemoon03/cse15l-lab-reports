This blog post is intended to instruct a user on how to use remote access. 

In order to use remote access, there are three steps: 
1. Install VSCode 
   In order to install VSCode, head to the VSCode website (https://code.visualstudio.com/). 
   Once at the website, download vscode for your version of operating system (Windows, Apple, etc). 
   Once installed, open the program and it should look something like this: 
   ![image](https://user-images.githubusercontent.com/112985603/212772936-af967dc1-fec8-4f59-bbb1-685b10fa1e69.png)

2. Remotely Connecting 
   In order to remotely connect, first the user has to install git and git bash, which can be found at this link: 
   https://git-scm.com/download/win. Once downloaded, open the terminal in VSCode and toggle from powershell to bash 
   in the dropdown menu given in the terminal: 
   ![image](https://user-images.githubusercontent.com/112985603/212773349-25e86977-dcbf-4136-82e6-991c515bd4b5.png)
   Once in bash, enter the command ssh (cs 15l id here)@ieng6.ucsd.edu
   ![image](https://user-images.githubusercontent.com/112985603/212774264-cbb36d69-adef-4c21-904f-edc523bcc5d9.png)
   , which will then prompt you to enter your password. Once entered it should look something like this: 
   ![image](https://user-images.githubusercontent.com/112985603/212774443-a6a81039-7e90-4af0-ace4-cdac2cfac821.png)                                       
   , and congratulations! You have successfully remotely connected! 
  
3. Trying Some Commands 
   Once in the bash terminal, try running some commands! (ex: cd, pwd, cp, cat), like so: 
   ![image](https://user-images.githubusercontent.com/112985603/212774935-5aa14dd2-1eb3-45b4-ae9c-5597c6afdbf9.png)
   Once you are done, you can log out of the remote server in your terminal by typing the command exit. 
