# Chapter 2.1 - Complete Study Material


## 🖥️ PRESENTATION SLIDES


# Chapter 2.1 - All Lecture Slides Text


## PPT 1 Looping
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.   2                           Chapter No.   1                                        Lecture No.1
- Topic : Loops
- Faculty Name-Dr. Sheenam
- E_Code - E6717
- Designation-Assistant Professor

### Slide 2
- Logical Thinking & Problem Solving
- Course Objectives
- The course aims to provide a strong foundation in problem-solving using the C programming language.
- It enhances students' programming skills by developing logical thinking and algorithmic problem-solving abilities
- By mastering C programming concepts, students will be able to design and implement efficient solutions for real-world problems

### Slide 3
- 3
- Course Outcomes
- CO No
- Statement
- CO1
- To remember the concepts related to fundamentals of C language, Algorithm/ pseudocode, Flowcharts and Problem solving
- CO2
- To understand the way of execution and debug programs in C language.
- CO3
- To apply various constructs, loops, functions to solve mathematical and scientific problem.
- CO4
- To analyse the dynamic behaviour of memory by the use of pointers.
- CO5
- To design and develop modular programs for real world problems using control structure and selection structure.

### Slide 4
- Recap
- of
- Previous
- Lecture
- The switch statement is used for multi-way decision making.
- It allows execution of different blocks based on the value of an expression.
- The
- case labels represent different possible values.
- break statement is used to stop execution after a matching case.
- The default case executes when no case matches.
- It is an alternative to multiple if-else statements.
- The expression in switch must be of integer or character type.

### Slide 5
- Loops
- Types of Loops
- Examples
- CONTENTS

### Slide 6
- Types of Looping statements
- Entry controlled loop or Pre-Test Loop: In the entry controlled loop or Pre-Test loop, the condition is checked before we start and at the beginning of each iteration of the loop. If the condition is true, we execute body of loop; if the control expression is false, we terminate the loop. Examples:  while statement and for statement.
- Exit controlled loop or Post-Test Loop: In the exit controlled loop or Post-Test loop, the condition is checked after or at the end of each iteration of the loop. If the condition is true, we repeat body of loop; if the condition is false, we terminate the loop. Examples: do…while statement

### Slide 7
- Iterative Statements
- Iterative statements are used to repeat the execution of a list of statements, depending on the value of an integer expression. In this section, we will discuss all these statements.
- While loop
- Do-while loop
- For loop

### Slide 8
- WHILE LOOP
- A loop within another loop is called nested loop. C programming language supports nesting of one loop inside another. We can define any number of loops inside another loop. And also have any number of nesting level.
- Put any type of loop in another type.
- Write for loop inside while loop, while inside another while etc. A programmer nest up to 3 loops. But there is no limit of nesting in C.

### Slide 9
- WHILE LOOP
- Syntax
- while (condition)
- {
- statement_block
- ;
- }
- statement x;

### Slide 10
- DO WHILE LOOP
- The do-while loop is similar to the while loop. The only difference is that in a do-while loop, the test condition is tested at the end of the loop.
- The body of the loop gets executed at least one time (even if the condition is false).
- The do while loop continues to execute whilst a condition is true. There is no choice whether to execute the loop or not. Hence, entry in the loop is automatic there is only a choice to continue it further or not.
- The major disadvantage of using a do while loop is that it always executes at least once, so even if the user enters some invalid data, the loop will execute.
- Do-while loops are widely used to print a list of options for a menu driven program.

### Slide 11
- DO WHILE LOOP
- Syntax
- Statement x;
- do
- {
- statement_block
- ;
- } while (condition);
- statement y;

### Slide 12
- // PROGRAM TO PRINT NUMBERS FROM 0 TO 10 USING WHILE LOOP
- #include<stdio.h>
- int main()
- {
- int
- i
- = 0;
- while(
- i
- <=10)
- {
- printf
- (“\n %d”,
- i
- );
- i
- =
- i
- + 1;             // condition updated
- }
- return 0;
- }
- // PROGRAM TO PRINT NUMBERS FROM 0-10 USING DO-WHILE LOOP
- #include<stdio.h>
- int main()
- {
- int
- i
- = 0;
- do
- {
- printf
- (“\n %d”,
- i
- );
- i
- =
- i
- + 1;
- } while(
- i
- <=10);
- return 0;
- }
- Program to demonstrate the use of while loop and do while loop
- Program based on While Loop
- Program based on Do While Loop

### Slide 13
- FOR LOOP
- When a for loop is used, the loop variable is initialized only once.
- With every iteration of the loop, the value of the loop variable is updated and the condition is checked. If the condition is true, the statement block of the loop is executed else, the statements comprising the statement block of the for loop are skipped and the control jumps to the immediate statement following the for loop body.
- Updating the loop variable may include incrementing the loop variable, decrementing the loop variable or setting it to some other value like,
- i
- +=2, where
- i
- is the loop variable.

### Slide 14
- FOR LOOP
- Syntax
- for (initialization; condition; increment/decrement/update)
- {
- statement block;
- }
- Statement Y;

### Slide 15
- Program For For-loop
- Look at the code given below which print first n numbers using a for loop.
- #include<stdio.h>
- int main()
- {
- int
- i
- , n;
- printf
- (“\n Enter the value of n :”);
- scanf
- (“%d”, &n);
- for(
- i
- =0;
- i
- <= n;
- i
- ++)
- printf
- (“\n %d”,
- i
- );
- return 0;
- }

### Slide 16
- Summary
- For
- It continues to process a block of code until a statement becomes false, and everything is defined in single line
- While
- It has one control condition, and executes as long the condition is true.
- Do-while
- It always executes the code block at least once and furthermore as long as the condition remains true

### Slide 17
- University
- Institute
- of
- Engineering
- (UIE)
- Next
- Lecture
- Nested loops are loops placed inside another loop.
- They are used when a task requires repeated execution within another repetition.
- The outer loop controls the number of times the inner loop runs.
- Nested loops are widely used in pattern printing, arrays, and matrix operations.
- C programming supports nesting of for, while, and do-while loops.
- Proper use of nested loops helps in solving complex iterative problems efficiently
- .

### Slide 18
- FAQ
- Feature
- while
- Loop
- Do-while
- Loop
- Condition Checking
- Condition is checked before the loop body     executes.
- Condition is checked after the loop body executes.
- Minimum Execution
- May not execute even once if the condition is false.
- Executes at least once, even if the condition is false.
- Syntax
- while(condition) { // code }
- do { // code } while(condition);
- Use Case
- When loop should run only if the condition is true.
- When loop must run at least once before checking condition.
- Control Flow
- Entry-controlled loop
- Exit-controlled loop
- Example
- while(i < 5) { printf("%d", i); i++; }
- do {
- printf
- ("%d",
- i
- );
- i
- ++; } while(
- i
- < 5);
- Q1. What is the difference between while loop and do-while loop?

### Slide 19
- FAQ
- Q2 Write a program to print table of a number enter by user.
- #include <
- stdio.h
- >
- void main()
- {
- int
- j,n
- ;
- printf
- ("Input the number (Table to be calculated) : ");
- scanf
- ("%
- d",&n
- );
- printf
- ("\n");
- for(j=1;j<=10;j++)
- {
- printf
- ("%d X %d = %d \n",
- n,j,n
- *j);
- }
- }

### Slide 20
- Assessment Questions
- 1. Program to check Armstrong number.
- 2. Write a c program to check a number is prime number or not.
- 3. Write  programs for the following :
- a) program to read 10 numbers from keyboard and find their sum and average.
- b) to calculate the simple interest.
- 4. do-while loop terminates when conditional expression returns?
- A One
- B ZERO
- C NON-ZERO
- D NONE OF THE ABOVE

### Slide 21
- Q& A
- Program takes an integer from the user and calculates the number of digits.
- For example: If the user enters 231967, the output of the program will be 6.

### Slide 22
- References
- Book References:
- [1] Programming in C by Reema Thareja.
- [2] Programming in AN[SI C by E.
- Balaguruswamy
- , Tata McGraw Hill.
- [3] Programming with C (Schaum's Outline Series) by Byron Gottfried  Jitender Chhabra, Tata McGraw Hill.
- [4] The C Programming Language by Brian W. Kernighan, Dennis Ritchie, Pearson education.
- Video Lecture:
- https://www.studytonight.com/c/loops-in-c.php
- Websites:
- https://www.programiz.com/c-programming/c-for-loop
- https://study.com/academy/lesson/nesting-loops-statements-in-c-programming.html

### Slide 23
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 24
- Class-wise feedback

### Slide 25
- THANK YOU


## PPT 2 Nested Loop
### Slide 1
- Logical Thinking & Problem Solving
- Course Objectives
- 1
- The course aims to provide a strong foundation in problem-solving using the C programming language.
- It enhances students' programming skills by developing logical thinking and algorithmic problem-solving abilities
- By mastering C programming concepts, students will be able to design and implement efficient solutions for real-world problems

### Slide 2
- 2
- Course Outcomes
- CO No
- Statement
- CO1
- To remember the concepts related to fundamentals of C language, Algorithm/ pseudocode, Flowcharts and Problem solving
- CO2
- To understand the way of execution and debug programs in C language.
- CO3
- To apply various constructs, loops, functions to solve mathematical and scientific problem.
- CO4
- To analyse the dynamic behaviour of memory by the use of pointers.
- CO5
- To design and develop modular programs for real world problems using control structure and selection structure.

### Slide 3
- 3
- Recap of Previous Lecture
- Loops are used to execute statements repeatedly.
- C provides three types of loops: for, while, and do-while.
- for loop is suitable when the number of iterations is known.
- while loop is used when the condition is checked before execution.
- do-while loop executes at least once.
- Nested loops are loops inside another loop.
- break terminates the loop immediately.
- continue skips the current iteration and moves to the next one.
- Infinite loops occur when the terminating condition is never met.
- Loops improve code efficiency and reduce repetition.

### Slide 4
- Nested Loops
- Types of Nested Loops
- Examples
- CONTENTS

### Slide 5
- NESTED LOOP
- The while loop is used to repeat one or more statements while a particular condition is true.
- In the while loop, the condition is tested before any of the statements in the statement block is executed.
- If the condition is true, only then the statements will be executed otherwise the control will jump to the immediate statement outside the while loop block.
- We must constantly update the condition of the while loop.

### Slide 6
- NESTED LOOP SYNTAX
- Syntax
- outer_loop
- {
- inner_loop
- {
- // Inner loop statement/s
- }
- // Outer loop statement/s
- }

### Slide 7
- Working of Nested  Loop
- T
- here are two conditions that are given.
- The inner loop condition gets executed only when the outer loop condition gives the Boolean output as True. Else the flow control directly goes out of both the loops.
- Now coming into the execution of the inner loop, If the loop condition gives a true result, then the block of statements under that loop and the incremental condition gets executed.
- And in turn, if the condition gives a Boolean condition as False, then the inner loop gives its control back to the outer loop and again same conditions/loops gets executed/repeated.

### Slide 8
- Program 1 of Nested  do-while loop
- #include <
- stdio.h
- >
- int main()
- {
- int
- i
- =1;
- do           // outer loop
- {
- int j=1;
- do       // inner loop
- {
- printf
- ("*");
- j++
- ;
- }while(j<=8);
- printf
- ("\n");
- i
- ++;
- }while(
- i
- <=4);
- }
- Explanation:
- First, we initialize the outer loop counter variable, i.e., '
- i
- ' by 1.
- As we know that the
- do..while
- loop executes once without checking the condition, so the inner loop is executed without checking the condition in the outer loop.
- After the execution of the inner loop, the control moves to the update of the
- i
- ++.
- When the loop counter value is incremented, the condition is checked. If the condition in the outer loop is true, then the inner loop is executed.
- This process will continue until the condition in the outer loop is true

### Slide 9
- Program 2 of Nested  for loop

### Slide 10
- Summary
- A loop within another loop is called nested loop. C programming language supports nesting of one loop inside another.
- We can define any number of loops inside another loop. And also have any number of nesting level.
- Write for loop inside while loop, while inside another while etc. A programmer nest up to 3 loops. But there is no limit of nesting in C.
- It always executes the code block at least once and furthermore as long as the condition remains true

### Slide 11
- Next Lecture
- Jump statements are used to alter the normal flow of program execution.
- They transfer control from one part of the program to another.
- C provides four jump statements:
- break
- continue
- goto
- return
- break is used to terminate loops or switch statements.
- continue skips the current iteration of a loop.
- goto
- transfers control to a labeled statement.
- return exits from a function and may return a value.

### Slide 12
- Department
- of
- Computer
- Science
- and
- Engineering
- (CSE)
- University
- Institute
- of
- Engineering
- (UIE)
- Next
- Lecture
- Jump statements are used to alter the normal flow of program execution.
- They transfer control from one part of the program to another.
- C provides four jump statements:
- break
- continue
- goto
- return
- break is used to terminate loops or switch statements.
- continue skips the current iteration of a loop.
- goto
- transfers control to a labeled statement.
- return exits from a function and may return a value.
- Jump statements help in controlling loops and function execution efficiently.

### Slide 13
- FAQ
- Q1 Print the pattern
- #include<stdio.h>
- int main()
- {
- int
- i,j
- ;
- for(j=1;j<=5;j++)
- {
- for(
- i
- =1;i<=
- j;i
- ++)
- printf
- ("%5d",i);
- printf
- ("\n\n");
- }
- for(j=4;j>=1;j--)
- {
- for(
- i
- =1;i<=
- j;i
- ++)
- printf
- ("%5d",i);
- printf
- ("\n\n");
- }
- return 0;
- }

### Slide 14
- FAQ
- Q2  Print the reverse pattern
- #include<stdio.h>
- int main()
- {
- int
- i,j
- ;
- for(j=5;j>=1;j--)
- {
- for(
- i
- =
- j;i
- >=1;i--)
- printf
- ("%5d",i);
- printf
- ("\n\n");
- }
- return 0;
- }

### Slide 15
- References
- Book References:
- [1] Programming in C by Reema Thareja.
- [2] Programming in ANSI C by E.
- Balaguruswamy
- , Tata McGraw Hill.
- [3] Programming with C (Schaum's Outline Series) by Byron Gottfried  Jitender Chhabra, Tata McGraw Hill.
- [4] The C Programming Language by Brian W. Kernighan, Dennis Ritchie, Pearson education.
- Video Lecture:
- https://www.youtube.com/watch?v=mZqo8KDR37U
- Websites:
- 1. https://www.geeksforgeeks.org/c/nested-loops-in-programming/

### Slide 16
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 17
- Class-wise feedback

### Slide 18
- THANK YOU


## PPT 3 Jump statements
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.   2                           Chapter No.   1                                        Lecture No.3
- Topic : Loops
- Faculty Name-Dr. Sheenam
- E_Code
- - E6717
- Designation-Assistant Professor

### Slide 2
- Logical Thinking & Problem Solving
- Course Objectives
- 2
- The course aims to provide a strong foundation in problem-solving using the C programming language.
- It enhances students' programming skills by developing logical thinking and algorithmic problem-solving abilities
- By mastering C programming concepts, students will be able to design and implement efficient solutions for real-world problems

### Slide 3
- 3
- Course Outcomes
- CO No
- Statement
- CO1
- To remember the concepts related to fundamentals of C language, Algorithm/ pseudocode, Flowcharts and Problem solving
- CO2
- To understand the way of execution and debug programs in C language.
- CO3
- To apply various constructs, loops, functions to solve mathematical and scientific problem.
- CO4
- To analyse the dynamic behaviour of memory by the use of pointers.
- CO5
- To design and develop modular programs for real world problems using control structure and selection structure.

### Slide 4
- 4
- Recap of Previous Lecture

### Slide 5
- Break
- Continue
- Goto
- Return
- Examples
- CONTENTS

### Slide 6
- Jump Statements
- Jump statements can be used to modify the behavior of conditional and iterative statements
- They allow you to exit a loop, start the next iteration of a loop, or explicitly transfer program control to a specified location in your program.

### Slide 7
- Types of Jump statements
- They are of four types:-
- Break
- Continue
- goto
- Return

### Slide 8
- Break statement
- The break statement is used to terminate the loop or statement in which it present. After that, the control will pass to the statements that present after the break statement, if available. If the break statement present in the nested loop, then it terminates only those loops which contains break statement.
- Flowchart of break statement

### Slide 9
- Example 1: Program to print first 15 natural numbers
- #include <
- stdio.h
- >
- int
- main()
- {
- int
- i
- ;
- for
- (
- i
- =1;i<=15;i++)
- {
- printf
- ("%d\n",
- i
- );
- if
- (
- i
- ==10)
- break
- ;
- }
- return
- 0;
- }
- Example

### Slide 10
- Continue statement
- This statement is used to skip over the execution part of the loop on a certain condition. After that, it transfers the control to the beginning of the loop. Basically, it skips its following statements and continues with the next iteration of the loop.
- Flowchart of continue statement

### Slide 11
- Write a c program to print numbers
- #include <
- stdio.h
- >
- int main()
- {
- int
- i,j
- ;
- for
- (
- i
- =1;i<3;i++)
- {
- for
- (j=1;j<5;j++)
- {
- if
- (j==2)
- continue
- ;
- printf
- ("%d\
- n",j
- );
- }
- }
- return
- 0;
- }
- Explanation: In this program, we see that the
- printf
- ()
- instruction for the condition
- j=2
- is skipped each time during the execution because of
- continue
- . We also see that only the condition
- j=2
- gets affected by the
- continue
- . The outer loop runs without any disruption in its iteration.
- Example

### Slide 12
- Goto statement
- This statement is used to transfer control to the labeled statement in the program. The label is the valid identifier and placed just before the statement from where the control is transferred.
- Flowchart of Goto statement

### Slide 13
- Example:
- #include <
- stdio.h
- >
- int
- main()
- {
- int
- i,j
- ;
- for
- (
- i
- =1;i<5;i++)
- {
- if
- (
- i
- ==2)
- goto
- there;
- printf
- ("%d\n",
- i
- );
- }
- there:
- printf
- ("Two");
- return
- 0;
- }
- In this program, we see that when the control goes to the
- goto
- there
- ; statement when
- i
- becomes equal to
- 2
- then the control next goes out of the loop to the
- label
- (
- there
- : ) and prints
- Two
- .
- Example

### Slide 14
- Return statement
- This statement terminates the execution of the method and returns the control to the calling method. It returns an optional value. If the type of method is void, then the return statement can be excluded.
- Flowchart of return statement

### Slide 15
- Example:
- #include <
- stdio.h
- >
- char
- func
- (
- int
- ascii)
- {
- return
- ((
- char
- )ascii);
- }
- int
- main()
- {
- int
- ascii;
- char
- ch
- ;
- printf
- ("Enter any ascii value in decimal: \n");
- scanf
- ("%
- d",&ascii
- );
- ch
- =
- func
- (ascii);
- printf
- ("The character is : %c",
- ch
- );
- return
- 0;
- }
- In this program we have two functions that have a return type but only one function is returning a value [
- func
- ()] and the other is just used to terminate the function[main()].
- The function
- func
- () is returning the character value of the given number(here 110). We also see that return type of
- func
- () is char because it is returning a character value.
- The return in main() function returns zero because it is necessary to have a return value here because main has been given the return type int.
- Example

### Slide 16
- Summary
- Goto
- break
- continue
- return
- It is used to skip over the execution part of the loop on a certain condition.
- It terminates the execution of the method and returns the control to the calling method
- .
- It terminate the loop or statement in which it present.
- It transfer control to the labeled statement in the program.

### Slide 17
- Next Lecture
- An array is a collection of similar data elements stored in contiguous memory locations.
- Arrays are used to store multiple values using a single variable name.
- Each element in an array is accessed using an index value.
- Array indexing in C starts from 0.
- Arrays can store data of types such as int, float, char, etc.
- Arrays improve program efficiency by simplifying data handling.
- C supports one-dimensional and multidimensional arrays.
- Arrays are widely used in searching, sorting, and matrix operations.

### Slide 18
- FAQ
- Q1 Write a program in C to display the sum of the numbers enter by a user and stop taking input when user enter zero.
- #include<stdio.h>
- void main()
- {
- int
- num
- , sum=0,
- i,n
- ;
- printf
- ("Enter Number of inputs\n");
- scanf
- ("%
- d",&n
- );
- for(
- i
- =1;i<=n;++
- i
- )
- {
- printf
- ("Enter
- num%d
- : ",
- i
- );
- scanf
- ("%d",&
- num
- );
- if(
- num
- ==0)
- {
- break;      /*this breaks loop if
- num
- == 0 */
- printf
- ("Loop
- Breaked
- \n");
- }
- sum=
- sum+num
- ;
- }
- printf
- ("Total is %
- d",sum
- );
- getch
- ();}

### Slide 19
- FAQ
- Q2 Write a program to check if a number is even or not and print using the
- goto
- statement.
- #include <
- stdio.h
- >
- int main()
- {
- int num;
- printf
- ("Enter a number: ");
- scanf
- ("%
- d",&num
- );
- if (num % 2==0)
- goto
- even;
- else
- goto
- odd;
- even:
- printf
- ("even Number");
- Odd:
- printf
- ("odd Number");
- return 0;
- }

### Slide 20
- Assessment Questions
- 1.
- #include<
- stdio.h
- >
- int
- main()
- {
- int
- x;
- for(x=1;x<=10;x++)
- {
- if(x%2==1)
- continue;
- printf
- ("\
- t%d",x
- );
- }
- return 0;
- }
- 2.
- #include<
- stdio.h
- >
- int
- main()
- {
- int
- x=1;
- for(;;)
- {
- if(x>5)
- break;
- printf
- ("\
- t%d",x
- ++);
- }
- return 0;
- }
- 3.
- The break statement is used in?
- a) for loop
- b)switch statement
- c) while loop
- d)None of the above
- 4
- .
- #include <
- stdio.h
- >"
- int
- main()
- {
- int
- i
- ;
- goto
- LOOP;
- for (
- i
- = 0 ;
- i
- < 10 ;
- i
- ++)
- {
- printf
- ("
- GeeksQuizn
- ");
- LOOP:
- break;
- }
- return 0;
- }

### Slide 21
- References
- Book References:
- 1] Programming in C by Reema Thareja.
- [2] Programming in ANSI C by E.
- Balaguruswamy
- , Tata McGraw Hill.
- [3] Programming with C (Schaum's Outline Series) by Byron Gottfried  Jitender Chhabra, Tata McGraw Hill.
- [4] The C Programming Language by Brian W. Kernighan, Dennis Ritchie, Pearson education.
- Video Lecture:
- http://www.digimat.in/nptel/courses/video/106104128/L17.html
- https://spoken-tutorial.org/watch/C+and+Cpp/Loops/English/
- https://www.youtube.com/watch?v=67TlTBT68LE
- https://www.youtube.com/watch?v=Bv1LcqhqnZs
- Websites:
- https://www.cs.auckland.ac.nz/references/unix/digital/AQTLTBTE/DOCU_075.HTM
- https://www.programiz.com/c-programming/c-goto-statement
- https://www.geeksforgeeks.org/c-sharp-jump-statements-break-continue-goto-return-and-throw/

### Slide 22
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 23
- Class-wise feedback

### Slide 24
- THANK YOU
- 24


---
