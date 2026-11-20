# Description & Learning Outcomes - Complete Study Material


## 🖥️ PRESENTATION SLIDES


# Description & Learning Outcomes - All Lecture Slides Text


## 7 Operators
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester
- Jul-Dec 2026
- Unit No.
- 1
- Chapter No.   2                                        Lecture No.8
- Topic : Working with Operators
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
- 4
- Naming Variables
- Data types
- Variables
- Constants
- Defining constants
- Are used to declare variables .It specifies range , format specifier and memory space required by corresponding  variable
- Are names given to memory where value can be manipulated during program execution
- It can include alphabets , digits or underscore only
- Are quantities that do not change its value during program execution.
- Constants can be defined  either by macros or by using const keyword
- Recap of Previous Lecture

### Slide 5
- Space for visual (size 24)
- Arithmetic Operator
- Relational Operator
- Logical Operator
- Assignment Operator
- Increment and Decrement Operator
- Conditional Operator
- Misc Operator
- 5
- CONTENTS
- 11-08-2026

### Slide 6
- An operator is a symbol that tells the compiler to perform certain mathematical or logical manipulations.
- Operators are used in program to manipulate data and variables. The data items that operators act upon are called operands.
- Some operators require two operands, while others act upon only one operand. The operators are classified into unary, binary and ternary depending on whether they operate on one, two or three operands respectively
- .
- 11-08-2026
- Operators
- 6

### Slide 7
- Arithmetic Operators
- Relational Operators
- Logical Operators
- Assignment Operators
- Increment and Decrement Operator
- Bitwise Operators
- Conditional Operators
- Some Special Operators
- 11-08-2026
- Types of Operators
- 7

### Slide 8
- C programming language provides all basic arithmetic operators: +, -, *, / and %.
- 11-08-2026
- Arithmetic Operator
- 8
- Operator
- Meaning
- +
- Addition on unary plus
- -
- Subtraction or unary minus
- *
- Multiplication
- /
- Division
- %
- Modulo

### Slide 9
- #include<
- stdio.h
- >
- int
- main()
- {
- int
- a,b
- ;
- printf
- ("enter the value of a and b");
- scanf
- ("%d %
- d",&a,&b
- );                      //Input the value of a and b
- printf
- ("Result of
- a+b
- is %d\
- n",a+b
- );   //Addition of a and b
- printf
- ("Result of a-b is %d\
- n",a
- -b);    //
- Substraction
- of  and b
- printf
- ("Result of a*b is %d\
- n",a
- *b);   //Multiplication of a and b
- printf
- ("Result of a/b is %d\
- n",a
- /b);    // Division of A/B
- printf
- ("Result of
- a%b
- is %d\
- n",a%b
- ); //Remainder of division
- return 0;
- }
- 11-08-2026
- Arithmetic Operator
- 9

### Slide 10
- Relational operator compares between two operands and returns in true and false.
- Operators are as follows:
- 11-08-2026
- Relational Operator
- 10
- Operator
- Meaning
- >
- Greater then
- <
- Less then
- >=
- Greater then equal to
- <=
- Less then
- equal to
- ==
- Equal to
- !=
- Not equal
- to

### Slide 11
- #include <
- stdio.h
- >
- int
- main(void)
- {
- int
- a,b,c
- ;
- printf
- ("enter the value of
- a,b
- and c");
- scanf
- ("%d %d %
- d",&a,&b
- , &c);
- printf
- ("%d == %d is %d \n", a, b, a == b);
- printf
- ("%d == %d is %d \n", a, c, a == c);
- printf
- ("%d > %d is %d \n", a, b, a > b);
- printf
- ("%d > %d is %d \n", a, c, a > c);
- printf
- ("%d < %d is %d \n", a, b, a < b);
- 11-08-2026
- Relational Operator
- 11

### Slide 12
- printf
- ("%d < %d is %d \n", a, c, a < c);
- printf
- ("%d != %d is %d \n", a, b, a != b);
- printf
- ("%d != %d is %d \n", a, c, a != c);
- printf
- ("%d >= %d is %d \n", a, b, a >= b);
- printf
- ("%d >= %d is %d \n", a, c, a >= c);
- printf
- ("%d <= %d is %d \n", a, b, a <= b);
- printf
- ("%d <= %d is %d \n", a, c, a <= c);
- return 0;
- }
- 11-08-2026
- Relational Operator
- 12

### Slide 13
- Logical operator is used to compare or evaluate logical and relational expressions.
- Operators are as follows:
- 11-08-2026
- Logical Operator
- 13
- Operator
- Meaning
- &&
- Logical
- AND
- ||
- Logical OR
- !
- Logical NOT

### Slide 14
- #include <
- stdio.h
- >
- int
- main()
- {
- int
- a,b,c
- , result;
- printf
- ("enter the value of
- a,b
- and c");
- scanf
- ("%d %d %
- d",&a,&b
- , &c);
- result = (a == b) && (c > b);
- printf
- ("(a == b) && (c > b) is %d \n", result);
- result = (a == b) && (c < b);
- printf
- ("(a == b) && (c < b) is %d \n", result);
- result = (a == b) || (c < b);
- 11-08-2026
- Logical Operator
- 14

### Slide 15
- printf
- ("(a == b) || (c < b) is %d \n", result);
- result = (a != b) || (c < b);
- printf
- ("(a != b) || (c < b) is %d \n", result);
- result = !(a != b);
- printf
- ("!(a != b) is %d \n", result);
- result = !(a == b);
- printf
- ("!(a == b) is %d \n", result);
- return 0;
- }
- 11-08-2026
- Logical Operator
- 15

### Slide 16
- Assignment operators are used to assign result of an expression to a variable.
- ‘=’ is the assignment operator in C.
- You can use assignment operator for multiple assignments as follows:
- x=y=z=2;
- 11-08-2026
- Assignment Operator
- 16

### Slide 17
- #include <
- stdio.h
- >
- int
- main()
- {
- int
- a , c;
- printf
- ("Enter the value of a");
- scanf
- ("%
- d",&a
- );
- c = a;
- printf
- ("c = %d\n", c);
- c += a;
- printf
- ("c = %d\n", c);
- 11-08-2026
- Assignment Operator
- 17

### Slide 18
- c -= a;
- printf
- ("c = %d\n", c);
- c *= a;
- printf
- ("c = %d\n", c);
- c /= a;
- printf
- ("c = %d\n", c);
- c %= a;
- printf
- ("c = %d\n", c);
- return 0;
- }
- 11-08-2026
- Assignment Operator
- 18

### Slide 19
- Increment operator(++)
- The increment operator ++ adds 1 to the operand.
- Increment operator are of two types:
- Pre increment
- For example x=10; ++x; 11
- Post increment
- For example x=10; x++; 10
- 11-08-2026
- Increment and Decrement Operator
- 19

### Slide 20
- #include <
- stdio.h
- >
- int
- main()
- {
- int
- a, b;
- printf
- ("enter the value of
- a,b
- ");
- scanf
- ("%d %
- d",&a,&b
- );
- printf
- ("++a = %d \n", ++a);
- printf
- ("--b = %d \n", --b);
- return 0;
- }
- 11-08-2026
- Pre-Increment & Pre-Decrement
- 20

### Slide 21
- Decrement operator(--)
- The decrement operator -- subtracts 1 from the operand.
- Decrement
- operator are of two types:
- Pre
- decrement
- For example x=10; --x; 9
- Post
- decrement
- For example x=10; x--; 10
- 11-08-2026
- Increment and Decrement Operator
- 21

### Slide 22
- #include <
- stdio.h
- >
- int
- main()
- {
- int
- a, b;
- printf
- ("enter the value of
- a,b
- ");
- scanf
- ("%d %
- d",&a,&b
- );
- printf
- ("a++ = %d \n", a++);
- printf
- ("b-- = %d \n", b--);
- return 0;
- }
- 11-08-2026
- Post-Increment & Post-Decrement
- 22

### Slide 23
- Main features of Conditional operator are as follows:
- There are three operands
- It works from left to right.
- The operator pair “?” and “:” is known as conditional operator.
- Syntax:
- expression1 ? expression2 : expression3 ;
- Condition? True part: False part
- Example:
- a = 3 ; b = 5 ;
- x = (a > b) ? a : b ;
- 11-08-2026
- Conditional Operator
- 23

### Slide 24
- #include <
- stdio.h
- >
- int main()
- {
- int year;
- printf
- ("Enter a year to check if it is a leap year or not \n");
- scanf
- ("%d", &year);
- (year%4==0 && year%100!=0) ?
- printf
- ("Leap year") :
- ((year%400 ==0 ) ?
- printf
- ("Leap Year") :
- printf
- ("not a leap year"));
- }
- 11-08-2026
- Conditional Operator
- 24

### Slide 25
- Use conditional operator to find greatest among three numbers
- 11-08-2026
- Conditional Operator
- 25

### Slide 26
- C programming supports special operators like comma operator,
- sizeof
- operator, pointer operators (& and *) and member selection operators (. and ->). We will discuss Comma operator and
- sizeof
- operator in Unit-1.
- 11-08-2026
- Special Operator
- 26

### Slide 27
- The comma operator can be used to link the related expressions together
- Evaluation of comma operator is from left to right.
- For example:
- x = (a = 2, b = 4,
- a+b
- )
- 11-08-2026
- Comma Operator
- 27

### Slide 28
- Example1:
- #include<
- stdio.h
- >
- int
- main()
- {
- int
- i
- ;
- i
- = 1,2,3;
- printf
- ("
- i
- :%d\
- n",i
- );
- return 0;
- }
- Output:1
- 11-08-2026
- Comma
- Operator
- 28

### Slide 29
- Example2:
- #include<
- stdio.h
- >
- int
- main()
- {
- int
- i
- ;
- i
- = (1,2,3);
- printf
- ("
- i
- :%d\
- n",i
- );
- return 0;
- }
- Output: 3
- 11-08-2026
- Comma
- Operator
- 29

### Slide 30
- The
- sizeof
- operator is usually used with an operand which may be variable, constant or a data type qualifier.
- It calculates the size of data
- ie
- . how many bit a specific data is having.
- Syntax:
- sizeof
- (<variable>);
- Example: x =
- sizeof
- (a);
- 11-08-2026
- S
- izeof
- Operator
- 30

### Slide 31
- #include <
- stdio.h
- >
- int
- main()
- {
- int
- a;
- float b;
- double c;
- char d;
- printf
- ("Size of
- int
- =%
- lu
- bytes\
- n",sizeof
- (a));
- printf
- ("Size of float=%
- lu
- bytes\
- n",sizeof
- (b));
- printf
- ("Size of double=%
- lu
- bytes\
- n",sizeof
- (c));
- printf
- ("Size of char=%
- lu
- byte\
- n",sizeof
- (d));
- return 0;
- }
- 11-08-2026
- Sizeof
- Operator
- 31

### Slide 32
- Summary
- Important points to remember:
- C operators operates on one or more operands to produce a value.
- The operators that take one operand are called unary operators.
- The operators that require two operands are called binary operators.
- The operator that accepts three operands is called ternary operator. C  has only one ternary operator.

### Slide 33
- Q1. Can math operations be performed on a void pointer?
- Q2. Why n++ executes faster than n+1?
- Q3. What is a modulus Operators in C?
- Q4. What are the restrictions of a modulus operator in C?
- Q5. How can we find size of a variable without using
- sizeof
- () operator?
- Q6. How can we add two numbers in C language without using Arithmetic operators?
- 11-08-2026
- FAQ’s
- 33

### Slide 34
- Q1. Predict the output
- int
- main()
- {
- int
- x;
- x=10,20,30;
- printf
- ("%
- d",x
- );
- return 0;
- }
- (A) 10
- (B) 20
- (C) 30
- (D) Compilation Error
- 11-08-2026
- Assessment
- 34

### Slide 35
- Q2.  [
- Postfix
- ] operator has the highest precedence.
- Q3. What will be the output of the C program?
- #include<
- stdio.h
- >
- int
- main()
- {
- int
- x = 2;
- (x & 1) ?
- printf
- ("true") :
- printf
- ("false");
- return 0;
- }
- A. Compilation error
- B. true
- C. false
- D. Runtime error
- 11-08-2026
- Assessment
- 35

### Slide 36
- Q4. Print the output of the program
- #include <
- iostream
- >
- using namespace std;
- int
- main ()
- {
- int
- x, y;
- x = 2;
- y = ++x * ++x;
- cout
- << x << y;
- x = 2;
- y = x++ * ++x;
- cout
- << x << y;
- return 0;
- }
- Ans
- : 41649
- 11-08-2026
- Assessment
- 36

### Slide 37
- Q5. Your task is to take two numbers of
- int
- data type, two numbers of float data type as input and output their
- sum:Declare
- variables: two of type
- int
- and two of type
- float.Read
- lines of input from
- stdin
- (according to the sequence given in the 'Input Format' section below) and initialize your
- variables.Use
- the  and  operator to perform the following operations: Print the sum and difference of two
- int
- variable on a new
- line.Print
- the sum and difference of two float variable rounded to one decimal place on a new line.
- Sample Input
- 10 4
- 4.0 2.0
- Sample Output
- 14 6
- 6.0 2.0
- Solve the above problem in c.
- 11-08-2026
- Assessment
- 37

### Slide 38
- Next Lecture
- Concepts to be Covered
- Introduction to Bitwise Operators
- Bitwise AND (&)
- Bitwise OR (|)
- Bitwise XOR (^)
- Bitwise NOT (~)
- Left Shift (<<) and Right Shift (>>)
- Applications of Bitwise Operators
- Introduction to Type Casting
- Implicit and Explicit Type Casting
- Data Type Conversion Examples

### Slide 39
- References
- S.No
- Title
- Content link
- 1
- Book
- Programming in C by
- Reema
- Thareja
- .
- 2
- Book
- Programming with C (
- Schaum's
- Outline Series) by Byron Gottfried
- Jitender
- Chhabra
- , Tata McGraw Hill.
- 3
- Book
- The C Programming Language by Brian W. Kernighan, Dennis Ritchie, Pearson education.
- 4
- Book
- Programming in ANSI C by E.
- Balaguruswamy
- , Tata McGraw Hill.
- 5
- Weblink
- https://www.tutorialspoint.com/cprogramming/c_operators.htm
- 6
- Weblink
- https://www.programiz.com/c-programming

### Slide 40
- References
- S.No
- Title
- Content link
- 8
- Weblink
- https://www.studytonight.com/c/
- 9
- Video Link
- https://www.youtube.com/watch?v=t9WKOcRB63Q&list=PLJ5C_6qdAvBFzL9su5J-FX8x80BMhkPy1

### Slide 41
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 42
- Class-wise
- feedback
- 42

### Slide 43
- THANK YOU


## PPT 7 Functions
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.   2                           Chapter No.
- 3
- Lecture No.1
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
- • Strings are collection of characters.
- • Strings in C are stored in character arrays.
- • Each string ends with a null character (\0).
- • Common string operations:
- - Input and Output
- - String Length
- - String Copy
- - String Concatenation
- - String Comparison
- • Header file used:
- string.h

### Slide 5
- Function
- and its types
- Predefined Library Functions
- Built-in String Functions
- Examples
- 5
- CONTENTS

### Slide 6
- CONCEPT OF FUNCTION
- A function is a block of code that performs a specific task.
- Suppose, you need to create a program to create a circle and color it. You can create two functions to solve this problem:
- create a circle function
- create a color function
- Dividing a complex problem into smaller chunks makes our program easy to understand and reuse
- .
- 6

### Slide 7
- TYPES OF FUNCTION
- There are 2 types of functions in C programming:-
- User-Defined Functions
- Built-In or Pre-defined functions
- In this lecture , we discuss
- only Predefined
- functions. User defined functions will be
- discussed in next lecture.
- 7

### Slide 8
- Predefined Library Functions
- They are inbuilt functions in C programming. The prototype and data definitions of these functions are present in their respective header files. To use these functions we need to include the header file in our  program.
- Example: If you want to use the
- printf
- function, the file header  <
- stdio.h
- > should be included.
- #include <
- stdio.h
- >
- int main()
- {
- printf
- ("Hello");
- }
- If you try to use
- printf
- without including the
- stdio.h
- header file, you will get an error.
- 8

### Slide 9
- Advantages of Using C Library Function
- 1. They are simple because they work
- One of the most important reasons you should use library functions is simply because they work. These functions have gone through multiple rigorous testing and are easy to use.
- 2. The functions are optimized for performance
- Since, the functions are "standard library" functions, a dedicated group of developers constantly make them better. In the process, they are able to create the most efficient code optimized for maximum performance.
- 3. It saves considerable development time
- Since the general functions like printing to a screen, calculating the square root, and many more are already written. You shouldn't worry about creating them once again.
- 4. The functions are portable
- With ever-changing real-world needs, your application is expected to work every time, everywhere. And, these library functions help you in that they do the same thing on every computer.
- 9

### Slide 10
- Example of Library Function
- Example: Write a program in C to find square root of a number.
- You can compute the square root of a number, you can use the sqrt() library function. The function is defined in the <
- math.h
- > header file
- #include <
- stdio.h
- >
- #include <
- math.h
- >
- int main()
- {
- float num, root;
- printf
- ("Enter a number: ");
- scanf
- ("%f", &num);
- root = sqrt(num);
- printf
- ("Square root of %.2f = %.2f", num, root);
- return 0;
- }
- 10

### Slide 11
- C Header Files
- <
- assert.h
- >                                     Program assertion functions
- <
- ctype.h
- >                                      Character type functions
- <
- locale.h
- >                                      Localization functions
- <
- math.h
- >                                       Mathematics functions
- <
- setjmp.h
- >                                    Jump functions
- <
- signal.h
- >                                      Signal handling functions
- <
- stdio.h
- >                                       Standard Input/output functions
- <
- stdlib.h
- >                                      Standard Utility functions
- <
- String.h
- >                                      String handling functions
- <
- time.h
- >                                        Date time functions
- 11

### Slide 12
- Built-In String Functions
- C programming language provides a set of pre-defined functions called
- string handling functions
- to work with string values. The header file called
- string.h
- is used, whenever we want to use any string handling function
- Example: P
- rogram to compare two strings by using
- strcmp
- ()
- function.
- #include<stdio.h>
- #include<string.h>
- int main()
- {
- char a[100], b[100];
- printf
- ("Enter the first string\n");
- gets(a);
- printf
- ("Enter the second string\n");
- gets(b);
- if(
- strcmp
- (
- a,b
- ) == 0 )
- printf
- ("Entered strings are equal.\n");
- else
- printf
- ("Entered strings are not equal.\n");
- return 0;
- }
- 12

### Slide 13
- String Handling Functions
- 13

### Slide 14
- String Handling Functions(contd.)
- 14

### Slide 15
- SUMMARY
- We covered the following topics:-
- Functions and its types
- Library Functions
- Built-In String Functions
- 15

### Slide 16
- Next Lecture
- A flowchart is a graphical representation of an algorithm or process using symbols and arrows.
- It uses standard symbols such as oval (Start/End), rectangle (Process), parallelogram (Input/Output), and diamond (Decision).
- Flowcharts help in understanding program logic, problem analysis, and debugging easily.
- They provide a step-by-step visual flow of the solution before actual coding implementation.

### Slide 17
- FREQUENTLY ASKED QUESTIONS
- PROGRAMS
- 1. Write a program to reverse a string “Hello” using
- strrev
- ( ) function.
- 2.Write a program to concatenate using
- strcat
- () function.
- 3. Write a program to calculate Power of a number Using pow() Function
- 4. Program to calculate the time taken to add two numbers program.
- 5. Program to calculate the length of a string entered by a user
- 17

### Slide 18
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- 1. Which standard library function will you use to find the last
- occurance
- of a character in a string in C?
- A.
- strnchar
- ()
- B.
- strchar
- ()
- C.
- strrchar
- ()
- D.
- strrchr
- ()
- 2. Input/output function prototypes and macros are defined in which header file?
- A.
- conio.h
- B.
- stdlib.h
- C.
- stdio.h
- D.
- dos.h
- 3.
- What is stderr ?
- A.
- standard error
- B.
- standard error types
- C.
- standard error streams
- D.
- standard error definitions
- 18

### Slide 19
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- (contd.)
- 4.
- What will be the output of the following C code?
- void main()
- div_t
- res;
- res = div(34, 4);
- printf
- ("quotient part = %d
- \n
- ",
- res.quot
- );
- printf
- ("remainder part = %d
- \n
- ",
- res.rem
- );
- }
- a) quotient part=0
- remainder part=4
- b) quotient part=8
- remainder part=2
- c) quotient part=4
- remainder part=0
- d) quotient part=2
- remainder part=8
- 19

### Slide 20
- Next Lecture
- Topics to be Coverer
- Introduction to User Defined Functions
- Syntax and Structure
- Function Declaration & Definition
- Calling a Function
- Types of User Defined Functions

### Slide 21
- REFERENCES
- Video lectures:
- https://www.youtube.com/watch?v=7Bq87y7eJEg
- https://www.youtube.com/watch?v=K4MA1Hkwj0s
- Weblinks:
- 1.https://www.tutorialspoint.com/cprogramming/c_functions.htm
- 3
- . https://beginnersbook.com/2014/01/c-functions-examples/
- 21

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
- 23

### Slide 24
- THANK YOU


---
