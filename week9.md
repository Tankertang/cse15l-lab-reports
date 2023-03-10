# Week 5 Lab Report
* Name: Tonghao Wu
* Date: 3/10/2023
* Section: B07
* PID: A16836645

***

I will be doing my lab report on ab report 3 (about find/grep etc). The reason why I chose this as my favorite lab is because how practical it is.
After finishing lab report and learning about how to use `find`and `grep` to find files and words in a file, I used what I learned to find files on my Mac  
latop.

For example, I had a file name `MyDeque.java` located within a folder in my download folder(`Download Folder` -> `Some Folder` ->`MyDeque.java`).
The thing is that there are many folders in the download folder and I don't know which folder for `MyDeque.java` is stored in. 

So I took what I learned for report 3 and applied it.

First I opened up terminal on the Mac. 

Then I typed out the command `find Downloads | grep "MyDeque.java"`. The `find` command basically list out every file within the Downloads folder and the `grep`
command find the `string` your look for in that folder. Below is a picture of me using the `find Downloads | grep "MyDeque.java"` command on my terminal

<img width="615" alt="Screen Shot 2023-03-10 at 8 35 41 AM" src="https://user-images.githubusercontent.com/61090478/224371711-3ba2a6a2-7d2e-46ac-a86a-057fff0c9a8a.png">


***

An alternative to `find` is `ls`. This command lists the contents of a directory, so it's useful for finding files in a specific directory. You can use the -l option to see more detailed information about each file.

An alternative to `grep` is `Tre-agrep`. `Tre-agrep`ter has all of grep's functionality but can also do ambiguous or fuzzy searches without deep knowledge of regular expressions. 
