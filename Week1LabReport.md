# Week 1 Lab Report
* Name: Tonghao Wu
* Date: 1/16/2023
* Section: B07
* PID: A16836645

***

We began the the lab by introducing ourself to the other group members.

***

After introducing ourself we install Visual Studio Code(VScode) corresponding to our operating system. In order you install VScode we use this [link](https://code.visualstudio.com/). 

Once you click the link you should see this as the webpage. <img width="1437" alt="Screen Shot 2023-01-25 at 4 26 01 AM" src="https://user-images.githubusercontent.com/61090478/214563206-aa82441a-88d8-4165-98cd-a18b2d6c2072.png">

Click on the big blue button near the center left captioned "Download Mac Universal". Once you click on that blue button a zip file should appear on the bottom of your screen. <img width="1317" alt="Screen Shot 2023-01-25 at 4 38 27 AM" src="https://user-images.githubusercontent.com/61090478/214571933-ec5ea5ae-c689-4a5b-9115-6f68f3b95de9.png">

Click on the zip file once it has finish downloading. After clicking on the zip file it will extract VS Code(the actual application) and it should appear on your finder(for mac) and file explorer(for window).

<img width="629" alt="Screen Shot 2023-01-25 at 4 30 36 AM" src="https://user-images.githubusercontent.com/61090478/214563890-b12b5a26-3229-43fe-ae2f-7fcf9c220494.png">

***

# Image of VScode once installed
<img width="1440" alt="Screen Shot 2023-01-12 at 4 19 34 PM 2" src="https://user-images.githubusercontent.com/61090478/212238589-8593b0ba-2ee8-44e7-9573-91a1f71103a9.png">

***

After installing VScode we had to setup VScode to use Git Bash. Since I was using MacOS my VScode came with bash. 
To switch to bash from the default zsh on terminal. First open up terminal using the Ctrl+ Backtick shortcut. After opening up terminal locate zsh on the bottom right and then to the right of zsh there will be a drop down sign and press that and change to bash.
<img width="1216" alt="Screen Shot 2023-01-15 at 11 01 28 PM" src="https://user-images.githubusercontent.com/61090478/212617968-6fcd2506-36c7-4203-9af2-dc30977bc337.png">


After switching to bash on terminal we use the command `ssh cs15lwi23zz@ieng6.ucsd.edu` to connect to CSE 15 account.

***

After Connectning we are greated with this line of code.
```
⤇ ssh cs15lwi23zz@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```
***

Then we type `yes` to connect 

***

After typing yes and putting in our we get this

***

![Screen Shot 2023-01-12 at 4 43 07 PM (1)](https://user-images.githubusercontent.com/61090478/212246364-380dfeda-1fa2-4cc9-9881-e430c75f2019.png)

***

Then we run some command such as 
* cd ~
* cd
* ls -lat
* ls -a
* ls <directory>
* cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
* cat /home/linux/ieng6/cs15lwi23/public/hello.txt
  
The `cd` linux command is to navigate through directories. The `ls` command in Linux is use to list directories. One interesting thing about the `ls` commmand is that on its own it lists all files in the current directory except for hidden files command. The `cp` command is use for copying file.
The `cat` command display the content of the file on the terminal.
  
***
  
Below are results after running in some of the mentioned commands
  
***
  
![Screen Shot 2023-01-12 at 4 55 51 PM](https://user-images.githubusercontent.com/61090478/212818516-8603c584-b872-4b20-bf59-c9e7500ced39.png)

  
***
  
To log out of the remote server in your terminal, you can use:
  
***
  
Ctrl-D or
Run the command `exit`
  
***
  
After finishing using the bash terminal, we made a GitHub account to document our work projects using MarkDown. [Here is a list of common MarkDown References](https://ucsd-cse15l-w23.github.io/week/week1/). Here is the [Link](yessir.md) to the website I made. 

  
