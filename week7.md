# Week 7 Lab Report
* Name: Tonghao Wu
* Date: 2/25/2023
* Section: B07
* PID: A16836645

***

* Step 1
  For step 1 we had to delete any existing forks of the repository you have on your account. 
  In order to delete existing forks on you press settings button, then on the general tab scroll all the way to the bottom until see a section titled danger zone, press delete repository to delete repositorty.
  ![Screenshot 2023-02-24 202708](https://user-images.githubusercontent.com/61090478/221338006-56c8003a-05d6-4039-979b-39774c410edc.png)

* Step 2
  For step 2 we have to fork the repository. In order to fork the repository, click the fork icon on the top right of the page, then click the green fork button to fork it to your account.
  ![Screenshot 2023-02-24 202958](https://user-images.githubusercontent.com/61090478/221338239-570d2ef5-9d49-4c8b-a2c7-050a819d32ae.png)

* Step 3
  For step 3 I started a timer on my phone to time my progress. No Screenshot.
  
 * Step 4
  For step 4 we to login into our ieng6 account. 1) To login to our ieng6 account we have to type `ssh cse15lwizz@ieng6.ucsd.edu`, after typing that command into the terminal we are prompted with a respone to type in our coruse password which I typed in. (Hint) --> You can make this process faster and not have to type by Generating SSH Keys for ieng6. Generating SSH key are key pairs that are used for automating logins, single sign-on, and for authenticating hosts.
    ![Screenshot 2023-02-24 203926](https://user-images.githubusercontent.com/61090478/221338545-0809c3ef-2305-4c54-9838-df22fd9ea276.png)
    
##  Generating SSH Keys step for ieng6
 In your local terminal, run `ssh-keygen`
Keep entering ` <Enter> ` until the program shows some text it calles the “randomart image”.
  
Note the path where the public key is saved (underlined below).
  
Now, log into your remote course specific account on `ieng6`
  
Run `mkdir .ssh` in the terminal
  
Logout of your remote account
  
Now, we want to copy the public SSH key you created onto your remote account, specifically inside the .ssh directory you just created, in a file called authorized_keys.
  
Scroll up a bit to where you were creating the SSH key, find the line where it says: Your public key has been saved in: <path to your public SSH key>, copy the path. Make sure you get the public key file, ending in .pub, here, not the private file.
  
From your local computer, run scp <path to your public SSH key> cs15lwi23__@ieng6.ucsd.edu:~/.ssh/authorized_keys
  
Enter password when prompted (this will be the last time you have to type it!)
  
Try to log onto your remote account again, you shouldn’t be prompted for a password anymore.
    
    
 * Step 5
   For step 5 we had to clone your fork of the repository from your Github account, into to clone the repo into our terminal we have to get the url from that repo then type in the command `git clone <repo-url>`.
![Screenshot 2023-02-24 204232](https://user-images.githubusercontent.com/61090478/221338626-6cf2eb7c-afa9-4888-8223-8ca1c2d38c5a.png)

* Step 6
  For step 6 we had to run the tests, demonstrating that they fail. In order to that first I had to `cd lab7` (change directory into the repo). Then compile the java files with `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` and then run the test with the command `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore`.
![Screenshot 2023-02-24 204659](https://user-images.githubusercontent.com/61090478/221338822-02120120-07e5-4114-8949-89bc1d3e77f0.png)

* Step 7 
  For step 7 we had edit the code file to fix the failing test. To edit the code I use `nano ListExamples.java` which pulls up this page 
![Screenshot 2023-02-24 205044](https://user-images.githubusercontent.com/61090478/221338922-4faa013a-4ce2-4855-8d70-f071654e5e4d.png)


After getting that page I went to fix the bug which a typo.
First I used my mousepad and scroll down to `line 43`. After getting to `line 43` I pressed the `<Right Arrow>` key 12 times to get to the `1` in `index1`. Then I pressed `<Backspace>` to delete the `1` and change it `2` by pressing the `<2>` button on the numberpad. Before the code was `index1 +=1;` but after the change it should should be `index2 +=1;` because we are indexing the second array. 
Then after fixing the bug I press `<Ctrl-X>` to exit and then `<y>` to save and then `<enter>` to comfirm the process.

* Step 8
  For step 8 we had to run the tests, demonstrating that they now succeed. I press the `<up>` arrow three time to get to `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` to recompile, then I press the `<arrow>` arrow three times again to get `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore` to retest it to make sure the bug was fixed(which it was).
![Screenshot 2023-02-24 205401](https://user-images.githubusercontent.com/61090478/221339098-bc361708-5807-44ab-a565-721ccb8ded92.png)

* Step 9
 For step 9 we had Commit and push the resulting change to your Github account. First I began with `git add .` to stage all changes in the current directory and its subdirectories for the next commit. Then I used `git commit -m <message>` to create a new commit in my Git repository with message of the change. Then I use `git push` to push it to the repository in the Github account.
![Screenshot 2023-02-24 210640](https://user-images.githubusercontent.com/61090478/221339457-a12ebc7c-558a-4816-9b8c-b5035daaf432.png)
