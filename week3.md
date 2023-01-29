# Week 3 Lab Report
* Name: Tonghao Wu
* Date: 1/29/2023
* Section: B07
* PID: A16836645

***

# Part 1

public String handleRequest(URI url) {
        
        if (url.getPath().equals("/")) {
            return String.format("%s", string);
        } else if (url.getPath().equals("/increment")) {
            num += 1;
            return String.format("Number incremented!");
        } else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-message")) {
                size++;
                String[] parameters = new String[size];
                String [] store = url.getQuery().split("=");
                
                if (store[0].equals("s")) {
                    string = string+store[1]+"\n";
                    parameters[i] = string; 
                    return String.format("%s\n", string);
                }
            }
            return "404 Not Found!";
        }
    } 
 
    
 

***

# Part 2

  
 Below is the failure-inducing input for the buggy program in JUnits test
 `@Test
  public void testReversed() {
    int [] input2 = {2,4,6};
    assertArrayEquals(new int[]{6,4,2}, ArrayExamples.reversed(input2));
}`
 
 Below is an input that doesn’t induce a failure, as a JUnit test
 
 `@Test
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }`
  
  
 * First Test of failure-inducing input <img width="933" alt="Screen Shot 2023-01-29 at 2 11 14 AM" src="https://user-images.githubusercontent.com/61090478/215320326-f015af4b-2faf-46d3-9bbb-0f7b7adb9f6f.png">


  
 * Second Test of input that doesn't induce a failure <img width="660" alt="Screen Shot 2023-01-29 at 2 13 12 AM" src="https://user-images.githubusercontent.com/61090478/215319462-2d4bd246-5dcc-4bcc-96a8-f5003fc8e0f1.png">


Before: `static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  } `
  
  
  After: `static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  } `

In summary, before it we set arr[i] to equal to newArray[arr.length - i -1], and we set newArray[i] equal to arr[arr.length - i -1]) then return newArray instead of arr. These fixes addresses the issue because, before we set the orignal array to equal to a new array that did not have any element inside. So every time the for loop is run, we are basically setting the original array element that the current index to 0, which is by default what java set the element of an array with no arguement passed in. After switching new array to equal tot the original array, we are able to set the element from the original array into the new array from the last index to the first index and then return that new array, which is the reserve order of the original array.

***

# Part 3
Something I learned from week 2 lab was the parseInteger function. I learned that the parseInteger allow the user to change a number in a string format to an integer format so that it can be used as an integer.
