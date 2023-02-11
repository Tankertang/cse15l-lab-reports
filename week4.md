
I will be doing my Week 4 lab on `grep`. The `grep` command can search for a string in groups of files. When it finds a pattern that matches in more than one file, it prints the name of the file, followed by a colon, then the line matching the pattern [grep Defintion](https://docs.oracle.com/cd/E19253-01/806-7612/filesearch-99633/index.html#:~:text=The%20grep%20command%20can%20search,the%20line%20matching%20the%20pattern.).

***

# Grep -r <string> <path or direction>
The `-r` syntax search allows the grep to recursivley search through every files starting from the current working directory to find the string that you are looking for, it then return every instance that the files has the `<string>` value stored, meaning if one file contains the `<string>` value more than once, it will display that file more than once.
  
* Example 1
  
<img width="910" alt="Screen Shot 2023-02-11 at 1 26 31 AM" src="https://user-images.githubusercontent.com/61090478/218250879-ceeef6e4-b560-41df-b141-9228ce45049a.png">
  
I used `grep -r "Lucayans" ./written_2` to search for files that contains the word "Lucayans" and then the terminal return the files that the word "Lucayans" was stored in. As you can see the Bahamas-History.txt files has two instance of the word "Lucayans" stored inside, therefore the terminal returns Bahamas-History.txt twice.
  
 * Example 2
  
Moreover you can pair the `-r` syntax with the `-l` syntax to be combined into `-rl`. As a result, when using `-rl` you will now only display the files once even if that file contains  the `<string>` value more than once in its file. 
  
<img width="586" alt="Screen Shot 2023-02-11 at 1 36 56 AM" src="https://user-images.githubusercontent.com/61090478/218251236-d8382067-a88b-4970-956f-00dcd425757e.png">
  
 As you can see now I used `gregrep -rl "Lucayans" ./written_2`, and now it only returns once instance of the Bahamas-History.txt files.
  
****
  
# grep '^b' list
  
A caret (^) metacharacter indicates the beginning of the line. The following command finds any line in the file list that starts with the letter b. [Source](https://docs.oracle.com/cd/E19253-01/806-7612/filesearch-99633/index.html#:~:text=The%20grep%20command%20can%20search,the%20line%20matching%20the%20pattern.).  


  
  
