Download Link: https://assignmentchef.com/product/solved-assignment-1-comp-202
<br>
<strong>Please read the entire PDF before starting. You must do this assignment individually.</strong>

Question 1:         50 points

Question 2:         50 points

100 points total

<strong>It is very important that you follow the directions as closely as possible. </strong>The directions, while perhaps tedious, are designed to make it as easy as possible for the TAs to mark the assignments by letting them run your assignment, in some cases through automated tests. While these tests will never be used to determine your entire grade, they speed up the process significantly, which allows the TAs to provide better feedback and not waste time on administrative details. Plus, if the TA is in a good mood while he or she is grading, then that increases the chance of them giving out partial marks. &#x1f642; <strong>To get full marks, you must:</strong>

<ul>

 <li>Follow all directions below</li>

 <li>Make sure that your code compiles

  <ul>

   <li>Non-compiling code will receive a very low mark</li>

  </ul></li>

 <li>Write your name and student name is written as a comment in all .java files you hand in</li>

 <li>Indent your code properly</li>

 <li>Name your variables appropriately

  <ul>

   <li>The purpose of each variable should be obvious from the name</li>

  </ul></li>

 <li>Comment your work

  <ul>

   <li>A comment every line is not needed, but there should be enough comments to fully understand your program</li>

  </ul></li>

</ul>

1

<h1>Part 1 (0 points): Warm-up</h1>

<em>Do </em><strong>NOT </strong><em>submit this part, as it will not be graded. However, doing these exercises might help you to do the second part of the assignment, which will be graded. If you have di culties with the questions of Part 1, then we suggest that you consult the TAs during their o ce hours; they can help you and work with you through the warm-up questions. You are responsible for knowing all of the material in these questions.</em>

<strong>Warm-up Question 1          </strong>(0 points)

Create a file called HelloWorld.java, and in this file, declare a class called HelloWorld. This class should define only one method called main(). In the body of this method, use System.out.println() to display “Hello world!”. You can find such a class in the lecture slides; make sure you can compile and run it properly.

<strong>Warm-up Question 2          </strong>(0 points)

Create a file called Diagram.java, and in this file, declare a class called Diagram. This class should define only one method called main(). In the body of this method, use five statements of System.out.println() to display the following pattern:

22

2  2

2

2

22222

Use Strings composed out of the space character and the character ‘2’. For extra practice, try to draw the pattern ‘202’.

<strong>Warm-up Question 3      </strong>(0 points) <strong>Practice with Binary</strong>:

We usually use base 10 in our daily lives, because we have ten fingers. When operating in base 10, numbers have a ones column, a tens column, a 100s column, etc. These are all the powers of 10.

There is nothing special about 10 though. This can in fact be done with any number. In base 2, we have each column representing (from right to left) 1,2,4,8,16,etc. In base 3, it would be 1,3,9,27, etc.

Answer the following short questions about number representation and counting.

<ol>

 <li>In base 10, what is the largest digit that you can put in each column? What about base 2? Base 3? Base n?</li>

 <li>Represent the number thirteen in base 5.</li>

 <li>Represent the number thirteen in base 2.</li>

 <li>What binary number is equal to the sum of these two binary numbers? 10101011 + 10010001</li>

 <li>What is the number from the previous part in base 10?</li>

 <li>What is the binary number for 11010010 + 11000101?</li>

 <li>And what is the number from the previous part in base 10?</li>

</ol>

<strong>Warm-up Question 4          </strong>(0 points)

Logic

<ol>

 <li>What does the following logical expression evaluate to?</li>

</ol>

(false or false) and (true and (not false))

<ol start="2">

 <li>Let <em>a </em>and <em>b </em>be boolean variables. Is it possible to set values for <em>a </em>and <em>b </em>to have the following expression evaluate as <em>false</em>?</li>

</ol>

b or (((not a) or (not a)) or (a or (not b)))

<h1>Part 2</h1>

<em>The questions in this part of the assignment will be graded.</em>

<strong>Question 1: Calculator Program             </strong>(50 points)

Attached to this assignment is a file called Calculator.java. Note that there is a marked section where your code must go. The code outside of this area must not be modified.

Write Java code in the marked area to print the following calculations:

<ol>

 <li>The sum of the <em>a </em>and <em>b </em>variables</li>

 <li>The product of the <em>a </em>and <em>b </em>variables</li>

 <li>The result of dividing <em>a </em>by <em>b</em></li>

 <li>The result of dividing <em>a </em>by <em>c</em></li>

 <li>A statement saying whether <em>a </em>is larger than <em>b</em></li>

 <li>A statement saying whether <em>a </em>an odd number. Use the mod operator <em>%</em>.</li>

</ol>

For example, if the numbers entered are <em>5</em>, <em>5</em>, and <em>1</em>, the output should be:

Sum of a and b: 10

Product of a and b: 25

Dividing a by b: 1

Dividing a by c: 5.0

Is a larger than b: false Is a odd: true

Be sure to include the specified text on each output line. That is, concatenate a String literal with the value of a variable.

Note that this program is run by providing <em>input arguments</em>. For example, once this program is compiled, it can be run by typing the text run Calculator 5 5 1 in the Dr. Java <em>Interactions Pane </em>and pressing

Enter.

<strong>Question 2: Creating a Grading Program                </strong>(50 points)

The goal of this question is to write several <em>methods </em>to create a program for outputting student grades. All the code for this question must be placed in a file named GradingProgram.java. Note that this means the class must also be named GradingProgram.

<strong>2a)Void Method for Confirming Entry</strong>

Write a method printInput that takes as input three double arguments and <strong>prints </strong>these numbers. You must include all three numbers as part of a message, separated by commas. For example, your message could be “You entered 34.0, -12.2, and 4.0”.

Note that for full marks, this message <strong>must </strong>be written on one line. Research the + operator for Strings, or the System.out.print() and System.out.println() statements.

<strong>Hint: To test your method, create a main method. The main method will not be graded in GradingProgram.java, but without it, you won’t know whether or not your method works! Your main method should call this </strong>printInput <strong>method and verify the results. You should think of other cases to test!</strong>

<strong>2b)Methods for Calculations</strong>

To make the GradingProgram more interesting, we will write a division method and a maximum method.

Write a method divide inside of GradingProgram.java that takes as input two double values. This method should return the result of dividing the first method parameter by the second. The return value must be a double value.

Note that division doesn’t work if the second parameter is zero. Therefore, if the second parameter is zero, the method should print an appropriate error message, and then return zero. Your method must <strong>not </strong>print anything if the second parameter is not zero.

To test your divide method, you will need to call it from your main method. Think about how you can call the method and then display the answer.

As well, write another method getMax that takes two doubles values as input. getMax must returns the larger of the two input values, and the return type must be double. In the case of a tie, return either value. Don’t use the built-in <em>max </em>method.

<strong>2c)Method Calling</strong>

Now we will use the divide and getMax methods to calculate student grades.

Write a method finalGrade that takes as input three double values and returns the final percentage out of 100 for a COMP 202 student. The return value must also be a double.

<ul>

 <li>The first value corresponds to the total assignment grade out of 35.</li>

 <li>The second is the midterm mark out of 20.</li>

 <li>And the third is the final exam mark out of 45.</li>

</ul>

Recall that if the student does better on the final than on the midterm, the mark for the final replaces the mark for the midterm. Therefore, you will have to calculate which is greater:

<ol>

 <li>The assignment grade plus the midterm grade plus the final grade divided by 100 OR</li>

 <li>The assignment grade plus the final grade divided by 80</li>

</ol>

Note that you must use the divide method that you created earlier to divide the sums. Then you must use your getMax method to determine which percentage would be higher. Finally, the percentage will then be less than 1, so multiply the answer by 100 before returning it.

For example, a student might have 28 out of 35 for assignments, 18 on 20 for the midterm, and 30 on 45 for the final. The finalGrade method takes these numbers 28.0, 18.0, 30.0 as input, in order, and would output a final grade of 76 (to represent 76%).

A student who instead had marks of 28.0, 16.0, 38.0 would have a final grade of 82.5 (to represent 82.5%). In this case, the midterm grade is dropped, because the student’s performance in the course is higher using the alternate grading scheme.

<h1>What To Submit</h1>

You have to submit one zip file with all your files in it to myCourses under Assignment 1. If you do not know how to zip files, please ask any search engine or friends. Google will be your best friend with this, and a lot of di↵erent little problems as well.

These files should all be inside your zip. Do not submit any other files, especially .class files.

Calculator.java

GradingProgram.java

Confession.txt (optional) In this file, you can tell the TA about any issues you ran into doing this assignment. If you point out an error that you know occurs in your problem, it may lead the TA to give you more partial credit. On the other hand, it also may lead the TA to notice something that otherwise they would not.