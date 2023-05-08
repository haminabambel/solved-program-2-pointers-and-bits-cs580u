Download Link: https://assignmentchef.com/product/solved-program-2-pointers-and-bits-cs580u
<br>
<u style="font-size: 1.618em;">Driver Code and Test Input Files</u>

<h3>●      Driver Code</h3>

<ul>

 <li>c //Driver Code get this from the Git classroom repo

  <ul>

   <li><em>Include the driver code with your submission, but do not alter it.</em></li>

  </ul></li>

</ul>

<h3><u>Grading Rubric</u></h3>

<strong><em>TOTAL: 20 points</em></strong>

<h2>●       Part 1: (12 points)</h2>

<ul>

 <li>myStrStr function works with all test cases (12 points / 2 for each case)</li>

</ul>

<h2>●       Part 2 (7 points):</h2>

<ul>

 <li>Passes Counting 1’s test (2 points) (must pass all tests)</li>

 <li>Passes Binary Tests (5 points total / 1 point each)</li>

</ul>

<h2>●       Style Guidelines (1 point)</h2>

<ul>

 <li>Follows requested program structure and submission format</li>

 <li>Follows <a href="https://drive.google.com/open?id=1PyRZpBay-PZ8CzQRDAaz2Oke0K0T1rIBHMKNzZWjgbI">formatting guidelines</a></li>

</ul>

<h3><u>Guidelines</u></h3>

This is an individual assignment. You must do the vast majority of the work on your own. It is permissible to consult with classmates to ask general questions about the assignment, to help discover and fix specific bugs, and to talk about high level approaches in general terms. It is not permissible to give or receive answers or solution details from fellow students.




You may research online for additional resources; however, you may not use code that was written specifically <em>to</em> solve the problem you have been given, and you may not have anyone else help you write the code or solve the problem. You may use code snippets found online, providing that they are appropriately and clearly cited, within your submitted code.




<em>By submitting this assignment, you agree that you have followed the above guidelines regarding collaboration and research.</em>




<em> </em>

Part 1 — String Manipulations




In the second program you will create a library file containing 4 functions. I have provided driver code that runs and tests your library code. You will need to create a <strong>second</strong> file that can be included in the driver code so the compiler can link them into an executable.




To include a file in c, you should use the preprocessing statement #include and the name of the file as a string at the top of your code. I have included a file called “mylib.h” in the driver code provided. This means you must write all of your code in a file called “mylib.h” and place it in the same directory as the provided driver code for the program to compile.




<ul>

 <li>For this part of the program you will implement your own version of the library function <a href="http://www.cplusplus.com/reference/cstring/strstr/">strstr()</a>, with the following function interface:<em>int myStrStr (char * haystack, char * needle, char * buffer);</em>

  <ul>

   <li>Your function will take 3 strings, a ‘haystack’ string, a ‘needle’ string, and a buffer string. You will search the haystack string for a sequence matching the needle string, and copy the found result (the entire substring) from the haystack string into the buffer (do not copy the needle string).</li>

   <li>You will return a 1 if the matching sequence in the haystack is found and a 0 if the needle is not found.</li>

   <li><em>You may </em><em>not</em><em> use the library strstr() function in your implementation. It is only for reference.</em></li>

  </ul></li>

 <li>I will test your function with the following hardcoded strings. <strong>Do not ask for user input. </strong>

  <ul>

   <li>haystack=”chocolate”, needle=”choc”</li>

   <li>haystack=”vanilla”, needle=”lla”</li>

   <li>haystack=”caramel”, needle=”am”</li>

   <li>haystack=”strawberry”, needle=”strawberry”</li>

   <li>haystack=”banana”, needle=”na”</li>

   <li>haystack=”cherry”, needle=”terrible”</li>

  </ul></li>

</ul>




Part 2 – Bits and Bytes




In Part 2 you are going to work with binary in a couple different ways.




<ul>

 <li>First you will write a function that counts the number of 1’s in the binary representation of an integer passed as a parameter to a function called countOnes() (see driver code for exact interface). You should return the number of 1s in the function’s parameter as an unsigned int.</li>

</ul>




<ul>

 <li>Next you will write a looping binary interpreter that creates an array representation of a binary value.

  <ul>

   <li>Write a function that uses bit shifting to store the binary representation of an integer in an array passed as a parameter. You will be given the size of the array and should make sure you fill out all elements in the array. To generate the array of values, you will need to use a bit mask and <a href="https://www.tutorialspoint.com/cprogramming/c_bitwise_operators.htm">bitwise right shift</a>.

    <ul>

     <li>8 would store the following value in your array

      <ul>

       <li>0000 0000 0000 0000 0000 0000 0000 1000</li>

      </ul></li>

     <li>The provided driver code (main) which calls your binaryArray function with each of the below values and an array buffer to print the binary representation (from right to left) for each one:</li>

     <li>2</li>

     <li>255</li>

     <li>-1</li>

     <li>INT_MAX</li>

     <li>INT_MIN

      <ul>

       <li>The driver code includes the library &lt;limits.h&gt; at the top of the main source code file so you can use the global constant INT_MAX and INT_MIN</li>

      </ul></li>

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li>You can use the following website to check your results: <a href="http://www.binaryhexconverter.com/binary-to-decimal-converter">http://www.binaryhexconverter.com/binary-to-decimal-converter</a></li>

</ul>







Part 3 – Submission

You must use any driver code as I have given you. DO NOT change it to take user input, different output, etc.




<ul>

 <li>Required code organization:

  <ul>

   <li><strong>&lt;user_id&gt;_</strong>c //Driver Code</li>

   <li>h

    <ul>

     <li>Any additional files should be included in your project2.zip submission</li>

    </ul></li>

   <li><span style="text-decoration: line-through;">While inside your program2 folder, create a zip archive with the following command </span>

    <ul>

     <li><span style="text-decoration: line-through;">zip -r <strong>&lt;user_id&gt;_program2</strong> &lt;user_id&gt;_program2.c mylib.h</span>

      <ul>

       <li><span style="text-decoration: line-through;">This creates an archive of all file and folders in the current directory called<strong> &lt;user_id&gt;_program2.zip</strong></span></li>

       <li><strong><span style="text-decoration: line-through;">Do not zip the folder itself, only the files required for the program</span></strong></li>

      </ul></li>

     <li><span style="text-decoration: line-through;">Upload the archive to Blackboard under Program 2.</span></li>

    </ul></li>

  </ul></li>

</ul>