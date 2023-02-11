
I will be doing my Week 4 lab on `grep`. The `grep` command can search for a string in groups of files. When it finds a pattern that matches in more than one file, it prints the name of the file, followed by a colon, then the line matching the pattern [grep Defintion](https://docs.oracle.com/cd/E19253-01/806-7612/filesearch-99633/index.html#:~:text=The%20grep%20command%20can%20search,the%20line%20matching%20the%20pattern.).

***

# grep -r <string> <path or direction>
The `-r` syntax search allows the grep to recursivley search through every files starting from the current working directory to find the string that you are looking for, it then return every instance that the files has the `<string>` value stored, meaning if one file contains the `<string>` value more than once, it will display that file more than once. [Source](https://phoenixnap.com/kb/grep-command-linux-unix-examples).
  
* Example 1
  
<img width="910" alt="Screen Shot 2023-02-11 at 1 26 31 AM" src="https://user-images.githubusercontent.com/61090478/218250879-ceeef6e4-b560-41df-b141-9228ce45049a.png">
  
I used `grep -r "Lucayans" ./written_2` to search for files that contains the word "Lucayans" and then the terminal return the files that the word "Lucayans" was stored in. As you can see the Bahamas-History.txt files has two instance of the word "Lucayans" stored inside, therefore the terminal returns Bahamas-History.txt twice.
  
 * Example 2
  
Moreover you can pair the `-r` syntax with the `-l` syntax to be combined into `-rl`. As a result, when using `-rl` you will now only display the files once even if that file contains  the `<string>` value more than once in its file. 
  
<img width="586" alt="Screen Shot 2023-02-11 at 1 36 56 AM" src="https://user-images.githubusercontent.com/61090478/218251236-d8382067-a88b-4970-956f-00dcd425757e.png">
  
 As you can see now I used `gregrep -rl "Lucayans" ./written_2`, and now it only returns once instance of the Bahamas-History.txt files.
  
***
  
# grep '^<string or character>' list
  
A caret (^) metacharacter indicates the beginning of the line. The following command finds any line in the file list that starts with the `<string or character>` . [Source](https://docs.oracle.com/cd/E19253-01/806-7612/filesearch-99633/index.html#:~:text=The%20grep%20command%20can%20search,the%20line%20matching%20the%20pattern.).  


* Example 1
  <img width="911" alt="Screen Shot 2023-02-11 at 1 58 07 AM" src="https://user-images.githubusercontent.com/61090478/218251955-b9e353f0-d6d4-4056-8a09-1b9294e8a656.png">
For this example I use `grep -r ^b ./written_2` to search for files that has lines that started with the letter "b".
  
 * Example 2
<img width="584" alt="Screen Shot 2023-02-11 at 2 00 55 AM" src="https://user-images.githubusercontent.com/61090478/218252096-1afbb955-e590-4920-9015-5db8be9b0dfc.png">

For example 2 I used `grep -r ^Years ./written_2` to find files with lines that started with the word 'Years'.
  
  
***

# grep '<string or character>$' list
  
A dollar-sign ($) metacharacter indicates the end of the line. The following command displays any line in which the '<string or character>' is the last character on the line. [Source](https://docs.oracle.com/cd/E19253-01/806-7612/filesearch-99633/index.html#:~:text=The%20grep%20command%20can%20search,the%20line%20matching%20the%20pattern.)


 ## Example 1 
  
<img width="922" alt="Screen Shot 2023-02-11 at 2 10 04 AM" src="https://user-images.githubusercontent.com/61090478/218252423-70619429-e398-439c-ab4d-ca4688539de8.png">
  
I used `grep -r b$ ./written_2` to display lines that end with the letter "b"  
  
## Example 2
  
 <img width="905" alt="Screen Shot 2023-02-11 at 2 11 22 AM" src="https://user-images.githubusercontent.com/61090478/218252470-86db619b-a1f4-4f14-b4c6-e7d3c69ad1d3.png">
I used `grep -r arbb$ ./written_2` to display lines that end with the word "arab"  
  
###  
To search multiple files with the grep command, insert the filenames you want to search, separated with a space character.

In our case, the grep command to match the word phoenix in three files sample, sample2, and sample3 looks like this example:


 
