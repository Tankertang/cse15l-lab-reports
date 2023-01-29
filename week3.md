# Week 3 Lab Report
* Name: Tonghao Wu
* Date: 1/29/2023
* Section: B07
* PID: A16836645

***

# Part 1

***

# Part 2

`static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }'
  
  This code is a buggy code.
