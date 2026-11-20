# Chapter 1.3 - All Lecture Slides Text


## 10 Decision control structures in C
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
- R
- ecap
- of Previous Lecture
- An expression is a combination of variables, constants, and operators that produces a value after evaluation.
- C supports different types of expressions such as arithmetic, relational, logical, and assignment expressions.
- Operator precedence and associativity determine the order in which operations are evaluated.
- Type casting is the process of converting one data type into another to ensure proper computation and compatibility.

### Slide 4
- Decision  control statements
- if statement
- if-else statement
- if-else-if statement
- Nested if-else statement
- Switch statement
- 4
- CONTENTS

### Slide 5
- DECISION CONTROL STATEMENTS in C
- Instructions are executed in one of the two manners
- Sequential
- Branching
- C language supports the following decision control statements
- if statement
- if-else statement
- if-else-if statement
- Nested if-else statement
- Switch statement
- 5

### Slide 6
- CONTROL STATEMENTS
- Determines the order in which the statements are executed.
- Must specify that a statement, or a group of statements, is to be carried out conditionally, only if some condition is true.
- 6
- Figure  1. Types of Control statements

### Slide 7
- If statement
- The single if statement in C language is used to execute the code if a condition is true. It is also called
- one-way selection statement.
- The general form of if statement is
- 7
- Figure 2.  Flowchart of if statement
- if(expression)
- {
- //
- statement/statement(s)
- }

### Slide 8
- Example 1 : Write a program in C to check whether a given number is even or odd
- .
- 8
- Source Code
- Output -1
- Output -2

### Slide 9
- Example 2 :  Write a program  in C to print the square of a number if it is less than 10.
- Source Code
- Output -1
- Output -2

### Slide 10
- If-else statement
- 10
- The if-else statement in C language is used to execute the code if condition is true or false.
- .
- It is also called two-way selection statement.
- The general form of if-else statement is:
- if(expression)
- {
- //Statement/Statement(s);
- }
- else
- {
- //Statement/Statement(s);
- }
- Figure 3. Flowchart of  if-else  statement

### Slide 11
- Example 3- Write a program to check whether a given year is leap year or not
- .
- 11
- Source Code
- Output -1
- Output -2

### Slide 12
- Example 4- Write a program in C to find the maximum of the two given numbers.
- 12
- Source Code
- Output -1
- Output -2

### Slide 13
- if-else-if statement/if-else-if Ladder
- 13
- It is used when more than one condition is to be checked.
- A block of statement is enclosed inside if, else if and else part.
- If the condition is true, the statements inside that block are executed.
- If none of the conditions are true, the statements inside else block are executed.
- Else part is optional and may be present or absent.
- Figure  4. Flowchart of  if-else –if  statement

### Slide 14
- Syntax of
- if-else-if statement
- 14
- if(condition1)
- {
- //statement/statement(s);
- }
- else if(condition2)
- {
- //statement/statement(s);
- }
- else if(condition3)
- {
- //statement/statement(s);
- }
- else
- {
- //statement/statement(s);
- }

### Slide 15
- Example 5- Write a program in C to check whether a number is zero, positive or negative
- 15
- Source Code
- Output -1
- Output -2
- Output -3

### Slide 16
- Example 6- Write a program in C to check whether a given number is divisible by 5 and 8 both or only by either 5 or 8.
- 16
- Source Code
- Output -1
- Output -2
- Output -3
- Output -4

### Slide 17
- Nested if-else statement
- Consider a situation, where you want to execute a statement based on multiple levels of condition check. For example - At airport there are multi-levels of checking before boarding. First you go for basic security check, then ticket check. If you have valid ticket, then you go for passport check. If you have valid passport, then again you will go for security check. If all these steps are completed successfully, then only you can board otherwise actions are taken by the author
- ity.
- Figure 5.  Flowchart of  nested if-else statement

### Slide 18
- Syntax of Nested if-else statement
- 18
- if( expression )
- {
- if( expression1 )
- {
- statement-block1;
- }
- else
- {
- statement-block 2;
- }
- }
- else
- {
- statement-block 3;
- }

### Slide 19
- Example 7- Write a program in C to find the maximum of given three numbers.
- 19
- Source Code
- Output -1
- Output -2

### Slide 20
- Example 8-  Write a program in C to check if a number is less than 100 or not. If it is less than 100 then check if it is odd or even.
- 20
- Source Code
- Output -1
- Output -2

### Slide 21
- Switch Statement/Switch Case statement
- Switch statement acts as a substitute for a long if-else-if ladder that is used to test a list of cases.
- A switch statement contains one or more case labels which are tested against the switch expression.
- When the expression match to a case then the associated statements with that case would be executed.

### Slide 22
- Syntax of Switch Statement
- 22
- switch (variable or expression)
- {
- case value1:
- statement(s);
- break;
- case value2:
- statement(s);
- break;
- ...
- ... ...
- ... ... .
- case
- valueN
- :
- statement(s);
- break;
- default:
- statement(s);
- break;
- }
- Figure 6.  Flowchart of Switch Statement

### Slide 23
- Important Rules of using Switch Case statement
- Switch...case only works with integral, character or enumeration constant.
- Cases can be put in any order. However, it is recommended to put them in ascending order. It increases program readability.
- Any number of statements can be used for a specific case.
- The break statement transfers the control out of switch statement.
- The break statement is optional. It transfers program flow outside of switch...case.
- Case labels must be constants.
- Case labels must be unique.
- Case labels must end with a colon.
- 23

### Slide 24
- Example 9- Write a program in C to check whether the entered alphabet is vowel or consonant
- .
- 24
- Source Code
- Output -1
- Output -2

### Slide 25
- Example 10- Write a program in C to make a simple calculator
- 25
- Source Code
- Output -1
- Output -2

### Slide 26
- Switch vs. if else if
- The Switch statement is an extension of the if-else if statement. The switch makes one selection when there are several choices to be made.
- IF statement uses
- boolean
- expression to decide which alternative to be executed whereas SWITCH statement uses
- int
- /char expression to decide which alternative to be executed.
- IF statement increases the complexity of a program as alternatives increases.
- Speed: A switch statement might prove to be faster than ifs provided number of cases are good.
- 26

### Slide 27
- SUMMARY
- Use if...else...if statement when -
- There are conditions instead of list of choices.
- There are few number of conditions.
- Use switch...case when
- There is a list of choices, from which you need to take decision.
- Choices are in the form of integer, character or enumeration constant.
- Use if for single selection statement.
- Use if-else for two-way selection .
- 27
- Figure 7. Decision Control Structures

### Slide 28
- Concepts to be Covered
- Introduction to switch Statement
- Syntax of switch
- Working of case Labels
- Use of break Statement
- Role of default Case
- Flow of Control in switch
- Difference between if-else and switch
- Programs Based on Menu-Driven Operations
- Nested switch Statement
- Next Lecture

### Slide 29
- Practice Questions
- Q1. What will be the output of the following program?
- #
- include"stdio.h
- "
- int
- main()
- {
- int
- i
- ;
- if(
- i
- =0,2,3)
- printf
- ("
- Geeksforgeeks
- ");
- else
- printf
- ("Hello ");
- printf
- ("%d\
- n",i
- );
- }
- 29
- Options-
- a)Hello 3
- b)Hello 0
- c)
- Geeksforgeeks
- 0
- d)
- Geeksforgeeks
- 3

### Slide 30
- Practice Questions(contd.
- )
- 30
- Ans
- 1. (c)
- Geeksforgeeks
- 0
- Explanation :- At first zero will assign in ‘
- i
- ’ then comma operator returns the last value which is 3 and condition becomes true.

### Slide 31
- Practice Questions(contd.)
- Q2. What will be the output of the following program?
- #
- include"stdio.h
- "
- int
- main()
- {
- int
- i
- ;
- if(
- i
- =(2,1,0))
- printf
- ("
- Geeksforgeeks
- ");
- else
- printf
- ("Hello ");
- printf
- ("%d\
- n",i
- );
- }
- 31
- Options
- a)Hello 3
- b)
- Geeksforgeeks
- 0
- c)Hello 0
- d)
- Geeksforgeeks
- 3

### Slide 32
- Practice Questions(contd.)
- Ans
- 2. (c) Hello 0
- Explanation:
- Priority of parenthesis bracket is greater than equal to(=) operator , So at first comma operator return the last value which is zero(0) and then equal to(=) operator assign 0 to ‘
- i
- ’ and condition becomes false.
- 32

### Slide 33
- Practice Questions(contd.)
- Q3. What will be the output of the following program?
- 33
- #include <
- stdio.h
- >
- int
- main()
- {
- int
- num = 2;
- switch (num + 2)
- {
- case 1:
- printf
- ("Case 1: ");
- case 2:
- printf
- ("Case 2: ");
- case 3:
- printf
- ("Case 3: ");
- default:
- printf
- ("Default: ");
- }
- return 0;
- }

### Slide 34
- Practice Questions(contd.)
- Ans
- 3. Default
- Explanation :-  In switch, an expression “num+2” where num value is 2 and after addition the expression result is 4. Since there is no case defined with value 4 the default case got executed.
- 34

### Slide 35
- Discussion/Self- Practice Questions
- 35
- 1. Write a C program to find the roots of quadratic equation.
- 2. Write a C program to input month number and number of days in a month.
- 3. Given a positive integer denoting  n, do the following:
- If  1<=n<= 9 ,then print the lowercase English word corresponding to the number (e.g., one for 1 , two for 2 , etc.).
- If  n> 9 print Greater than 9.

### Slide 36
- REFERENCES
- Reference Books
- [1]
- Kanetkar
- , Y. (2010). Let us C. 15th ed.
- [2]
- Thareja
- Reema (2014) Programming in C. 2
- nd
- ed.
- [3]  Zed A. Shaw,
- Learn C the Hard Way’
- Reference Website
- [4]
- https://www.dotnettricks.com/learn/c/conditional-statements-if-else-switch-ladder
- [5]
- https://www.geeksforgeeks.org/output-c-programs-set-30-switch-case/
- [6] https://www.geeksforgeeks.org/output-c-programs-set-63-2/?ref=rp
- [7]
- https://codeforwin.org/2017/08/if-else-statement-c.html
- 36

### Slide 37
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 38
- Class-wise
- feedback
- 38

### Slide 39
- THANK YOU


## 11 Switch statemnet
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.   1                           Chapter No.   3                                        Lecture No.
- 2
- Topic : Switch Statement
- Faculty Name-Dr. Sheenam
- E_Code
- - E6717                                                                                                      Designation-Assistant Professor

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
- Recap of previous Lecture
- Use if...else...if statement when -
- There are conditions instead of list of choices.
- There are few number of conditions.
- Use switch...case when
- There is a list of choices, from which you need to take decision.
- Choices are in the form of integer, character or enumeration constant.
- Use if for single selection statement.
- Use if-else for two-way selection .
- 4
- Figure 7. Decision Control Structures

### Slide 5
- SWITCH
- STATEMENT
- Let’s cover the why and when of switch
- Sometimes we work with different options
- Based on those different options there are
- multiple tasks
- Thus, switch statement can be used where multiple tasks are  involved
- It takes a variable and test the value of that variable with the
- multiple cases
- There are 4 switch cases and suppose I gave value 4, the value will matched with each switch case and the matching case will execute ( which is case 4)
- Switch case 1
- Switch case 4
- Switch case 2
- Switch case 3

### Slide 6
- SWITCH
- STUCTURE
- Let’s go through the Structure of switch statement
- switch (expression)
- ​                  {
- case value1:
- // statements
- break;
- case value2:
- // statements
- break;
- .
- .
- .
- default:
- // default statements
- }
- Default statement is optional

### Slide 7
- switch (exp)              let int exp = 2
- ​                  {
- case 1:
- // statement 1
- break;
- case 2:
- // statements 2
- break;
- case 3:
- //statement 3
- default:
- statements
- }
- switch (exp)              let int exp = 2
- ​                  {
- case 1:
- // statement 1
- case 2:
- // statements 2
- case 3:
- //statement 3
- default:
- statements
- }
- Break will stop the control after case 2 & statement 2 will be printed only
- WITH BREAK
- All cases will execute after the matching case
- Why break ?

### Slide 8
- int n=2;
- switch(n+2)
- {
- case 1:
- printf("Case1: Value is: %d", n);
- case 2:
- printf("Case1: Value is: %d", n);
- case 3:
- printf("Case1: Value is: %d", n);
- default:
- printf("Default: Value is: %d", n);
- }
- Output:
- Default: value is: 2
- Explanation:
- Since in the above program example user gave value of n as 2 but the expression inside switch is evaluated to 4 (n+2) so, default case executed.
- LET’S LEARN EXAMPLE EXECUTION

### Slide 9
- char c='b';
- switch (c)
- {
- case 'd':
- printf ("Case D ");
- break;
- case 'b':
- printf ("Case B");
- break;
- case 'c':
- printf ("Case C");
- break;
- case 'z':
- printf ("Case Z ");
- break;
- default:
- printf ("Default ");
- }
- Output:
- Case B
- A case can be written with characters as well, like
- case ‘a’
- or
- case ‘A’
- is valid
- An expression inside switch can be a integer value or a character value

### Slide 10
- SUMMARY…..
- We covered how and why of switch statement
- Example executions of switch statement to gain better insight of concept
- The structure of switch through its syntax and its building cases components

### Slide 11
- Concepts to be Covered
- Introduction to goto Statement
- Syntax of goto
- Use of Labels in C
- Working of Control Transfer
- Advantages and Limitations of goto
- Difference between goto and Looping Statements
- Programs Using goto
- Best Practices and Avoiding Spaghetti Code
- Next Lecture

### Slide 12
- FREQUENTLY
- ASKED
- QUESTIONS
- THINK AND ANSWER BELOW QUESTIONS
- Why switch statement is required ?
- Is it necessary to have a default statement inside switch ?
- Why is the use of break ?
- Can you design a menu driven program using switch ?
- PROGRAMS
- C program to read weekday number and print weekday name using switch.
- C program to check whether a character is VOWEL or CONSONANT using switch statement.
- C program to design calculator with basic operations using switch
- .
- C program to check whether number is EVEN or ODD using switch.
- 5.  Write a menu driven C program that will build a calculator
- .

### Slide 13
- UTILISE YOUR KNOWLEDGE TO ANSWER
- Let us see how much you have learned from the lecture and how effectively you can apply your knowledge…!!
- 1.  Which of the following cannot be checked in a switch-case
- (C programming)
- A. Character
- B. Integer
- C. Float
- D. enum
- 2.  What will be the output of following program?
- #include <stdio.h>
- void main ()
- {
- int a=10;
- switch(a) {
- case 5+5:
- printf("Hello\n");
- default:
- printf("OK\n");
- }
- }

### Slide 14
- UTILISE YOUR KNOWLEDGE TO ANSWER
- Let us see how much you have learned from the lecture and how effectively you can apply your knowledge…!!
- 3.
- Can we use string value/variable in switch test condition?
- switch(test_expression)
- {
- case VALUE1:
- case VALUE2:
- case VALUE3:
- /*statements block 1*/
- break;
- case VALUE4:
- case VALUE5:
- /*statements block 2*/
- break;
- }
- A. Yes
- B. No

### Slide 15
- DISCUSSION FORUM
- Utilize your knowledge and think of a real-world application that you can build using a switch case and also that can contribute something good to the towards the real-world problem solving.
- We have used and studied else if ladder which is also a multiway decision maker than what u think why switch? what other pros we can have with using a switch statement?

### Slide 16
- Reference Books
- [1]
- Kanetkar
- , Y. (2010). Let us C. 15th ed.
- [2]
- Thareja
- Reema (2014) Programming in C. 2
- nd
- ed.
- [3]  Zed A. Shaw,
- Learn C the Hard Way’
- Reference Website
- [1]   https://www.guru99.com/c-switch-case-statement.html
- [2] https://www.programiz.com/c-programming/c-switch-case-statement
- REFERENCES
- BOOKS
- WEBSITES

### Slide 17
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 18
- Class-wise feedback
- 18

### Slide 19
- THANK YOU….


## 12 Goto
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor
- of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:25CSH-107
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.   1                           Chapter No.   1                                        Lecture
- No.3
- Topic :
- Goto statement
- Faculty Name-Dr. Sheenam
- E_Code
- - E6717                                                                                                      Designation-Assistant Professor

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
- RESOURCES & LEARNING DIRECTIONS
- FUTURE DIRECTIONS
- Students would be able to apply their
- Knowledge into maintaining the control of program in  efficient manner and to make better performance through optimization of code
- A WALKTHROUGH
- To what is goto statement
- To the syntax of goto statement
- To the structure execution of goto
- To what is conditional operator
- To why conditional and its structure
- To execution of conditional operator

### Slide 4
- Recap of previous Lecture
- The switch statement is a multi-way decision-making statement used to execute one block of code among multiple choices.
- It evaluates an expression and matches its value with corresponding case labels.
- The break statement is used to terminate a case and prevent fall-through execution.
- The default case executes when none of the specified cases match the expression.
- 4
- Figure 7. Decision Control Structures

### Slide 5
- GOTO STATEMENT
- Goto statements are useful when a programmer wants to change the flow of program
- Or if you want to alter the working of a desired code
- Whenever the compiler will reach a goto statement, program control will shift in either forward direction or backward where the goto label is defined
- FORWARD JUMP
- BACKWARD JUMP
- goto Label
- ……….
- ……….
- Label:
- Statements;
- Label:
- Statements;
- ………..
- ………..
- goto Label

### Slide 6
- int Totalmarks = 70 ;
- if (Totalmarks >= 50)
- {
- goto Pass;
- }
- else
- goto Fail;
- Pass:
- printf (" \n Congratulation! You made it \n");
- Fail:
- printf (" \n Better Luck Next Time \n");
- For Totalmarks 70, we will move inside if as 70>50 and execute goto and try to find pass label and shift the control to pass label.
- So the output will be,
- Congratulation! You made it
- EXAMPLE EXECUTION…..
- Forward jump

### Slide 7
- int num, i=1;
- printf ("Enter the number whose table you want to print?");
- scanf ("%d", &num);
- table:
- printf ("%d x %d = %d\n", num, i, num*i);
- i++;
- if(i<=10)
- goto table;
- So the output will be,
- Enter the number whose table you want to print? 10
- 10 x 1 = 10
- 10 x 2 = 20
- 10 x 3 = 30
- 10 x 4 = 40
- 10 x 5 = 50
- 10 x 6 = 60
- 10 x 7 = 70
- 10 x 8 = 80
- 10 x 9 = 90
- 10 x 10 = 100
- EXAMPLE EXECUTION…..
- Backward jump

### Slide 8
- CONDITIONAL OPERATOR
- The conditional operator is kind of similar to the if else statement
- it does follow the same algorithm as of if else statement but the conditional operator takes less space
- Helps to write the if-else statements in the shortest way
- Also called as ternary operator

### Slide 9
- int num1, num2, max;
- printf("Enter two numbers: ");
- scanf("%d %d", &num1, &num2);
- max = (num1 > num2) ? num1 : num2;
- printf("Maximum between %d and %d is %d", num1, num2, max);
- So the output will be,
- Enter two numbers :
- 3 7
- Maximum between 3 and 7 is 7
- EXAMPLE EXECUTION…..

### Slide 10
- So the output will be,
- Enter three numbers :
- 3 7  9
- Maximum between 3 ,7 and 9 = 9
- EXAMPLE EXECUTION…..
- int num1, num2, num3, max;
- printf("Enter three numbers: ");
- scanf("%d %d %d", &num1, &num2, &num3);
- max = (num1 > num2 && num1 > num3) ? num1 :
- (num2 > num3) ? num2 : num3;
- printf("\n Maximum between %d, %d and %d = %d", num1, num2, num3, max);

### Slide 11
- SUMMARY…..
- In a nutshell we can say, the lecture provided deeper insight into the concept of goto and conditional operator, through their structure and implementation examples the idea about how to program them into changing the flow control of the code and it’s optimization got clear

### Slide 12
- Concepts to be Covered
- Introduction to goto Statement
- Syntax of goto
- Use of Labels in C
- Working of Control Transfer
- Advantages and Limitations of goto
- Difference between goto and Looping Statements
- Programs Using goto
- Best Practices and Avoiding Spaghetti Code
- Next Lecture

### Slide 13
- FREQUENTLY
- ASKED
- QUESTIONS
- C program to check whether entered number by the user is prime using goto.
- C program to find the factorial of a number entered by the user using goto
- .
- C program to find the sum of first N natural numbers using goto.
- C program to print Fibonacci series up to user specifies limit using goto.
- C program to check whether a number is palindrome or not using goto.
- To find maximum among four numbers using ternary operator c program.
- To check the person is eligible for vote or not using conditional operator.
- To find maximum among five numbers using ternary operator

### Slide 14
- UTILISE YOUR KNOWLEDGE TO ANSWER
- 1. What is the output of the C Program.?
- int main ()
- {
- int a=0;
- a = (5>2)?: 8;
- printf("%d", a);
- return 0; }
- 2. goto can be used to jump from main to within a function?
- A. True
- B. False
- 3. What is the output of C Program.?
- int main ()
- {
- int a=0, b;
- a = (5>2)? b=6: b=8;
- printf ("%d %d", a, b);
- return 0;
- }

### Slide 15
- UTILISE YOUR KNOWLEDGE TO ANSWER
- 4.
- Choose a syntax for C Ternary Operator from the list.
- A) condition ? expression1 : expression2
- B) condition : expression1 ? expression2
- C) condition ? expression1 < expression2
- D) condition < expression1 ? Expression2
- 5.
- What is the output of this C code?
- int main ()
- {
- int x = 2, y = 0;
- int z = (y++) ? y == 1 && x : 0;
- printf ("%d\n", z);
- return 0;

### Slide 16
- While executing goto statement what do you feel? does it require extra time for carrying a jump either forward or backward by the compiler while executing the code.
- DISCUSSION
- FORUM
- Think about a situation where you got a project and it requires branching procedures. You are given an option of choosing between if-else and conditional operator, which one you will choose and tell why?

### Slide 17
- sources
- Links/description
- Reference Book
- [1]
- Kanetkar
- , Y. (2010). Let us C. 15th ed.
- [2]
- Thareja
- Reema (2014) Programming in C. 2
- nd
- ed.
- [3]  Zed A. Shaw,
- Learn C the Hard Way’
- Reference Website
- [1] https://www.geeksforgeeks.org/c/goto-statement-in-c/
- References

### Slide 18
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 19
- Class-wise feedback
- 19

### Slide 20
- THANK YOU…
