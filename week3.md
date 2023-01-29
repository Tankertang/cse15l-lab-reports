# Week 3 Lab Report
* Name: Tonghao Wu
* Date: 1/29/2023
* Section: B07
* PID: A16836645

***

# Part 1

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
  
  
 * First Test of failure-inducing input <img width="657" alt="Screen Shot 2023-01-26 at 5 49 24 PM" src="https://user-images.githubusercontent.com/61090478/215320049-f11130a0-623b-4d57-9ea3-1d7050323053.png">

  
 * Second Test of input that doesn't induce a failure <img width="660" alt="Screen Shot 2023-01-29 at 2 13 12 AM" src="https://user-images.githubusercontent.com/61090478/215319462-2d4bd246-5dcc-4bcc-96a8-f5003fc8e0f1.png">


Before: `static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  } `
  

