# Four-threads-for-different-string-functions
Created four threads Input, Reverse, Capital and Shift for their respective functions on an input string.


## Creating Threads
First, I initialized an empty global string variable in which the string will be stored and passed as an argument to different functions (threads).

Thread 1 => `Input Thread`

Thread 2 => `Reverse Thread`

Thread 3 => `Capital Thread`

Thread 4 => `Shift Thread`

![image](https://user-images.githubusercontent.com/91841622/210602441-d5e8028a-f3eb-4728-8662-8e40bf55b055.png)

## Working of Code

Input thread will take string input from user, reverse thread will reverse the string and output it, 
capital thread will capitalize the characters of string and output it and shift thread will shift each 
characters of the string two time (e.g. a will become c) and output it. All the threads wait for input 
thread when input thread finishes his task all the waiting thread start their work simultaneously. 

## Exception Handling

Exception is handled on input thread. The input taken from user should be Alphabets and not any integers, if any number is entered then user is requested again to enter valid string.

#### To use without Exception uncomment the first `input` function.

## Working of Threads

Thread 1 (Input thread) will start and take input from the user and store the string in the global variable and then we end thread 1 with join() function. Now the input string is stored in the global variable.

After this, the remaining threads 2, 3, and 4 will be started.
 
![image](https://user-images.githubusercontent.com/91841622/210603065-7cb0a8f9-dff6-42d4-a53c-4ff8cd2f7847.png)

Now thread 2 will be doing reverse function and the string stored in the global variable is passed into the function and the required reversed output is stored in a different variable and displayed.

Similarly, thread 3 will take the input string and give us the CAPITAL output of the string and thread 4 (shifting thread) will first remove the spaces from the input string and then it will shift the input string by passing the input string to the shift function and it will also ask for how many characters you want to shift, if entered 2 then will shift each character of the string two times (e.g. a will become c) and will display the output of shifted string.

