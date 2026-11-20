# Chapter 2.3 - All Lecture Slides Text


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


## PPT 8 USER DEFINED FUNCTIONS
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
- • Functions are reusable blocks of code.
- • Used to perform specific tasks.
- • Improve readability and modular programming.
- • Main parts of a function:
- - Declaration
- - Definition
- - Function Call
- • Types of functions:
- - Library Functions
- - User Defined Functions

### Slide 4
- User Defined Functions and its types
- Parameter Types, Parameter Passing
- Calling a Function
- Examples
- 4
- CONTENTS

### Slide 5
- 5
- Recap of Previous Lecture
- • Functions are reusable blocks of code.
- • Used to simplify complex programs.
- • Improve readability and modularity.
- • Types of Functions:
- - Library Functions
- - User Defined Functions
- • Main Components:
- - Declaration
- - Definition
- - Function Call

### Slide 6
- USER DEFINED FUNCTION
- DEFINITION:
- A large C program is divided into basic building blocks called C function. C function contains set of instructions enclosed by “{  }” which performs specific operation in a C program. The main components of a function includes return type, function name and argument list.
- 6

### Slide 7
- USER DEFINED FUNCTION COMPONENTS
- Return-type:
- This specifies the data type of the value being returned by the function. A function may or may not return a value. If the function does not return a value, then the return type is void. In this case, the return value is an integer value c, which means the return type would be
- int
- .
- Parameter list:
- The list of formal parameters being passed onto the function. In this case, there are two parameters of type
- int
- passed to the function.
- Local variables or local declarations:
- The variables that are declared inside the function are called local variables. The scope of these variables lies within the function and they are not accessible outside the function.
- Function body:
- Comprised of everything inside the curly brackets { and } following the return type, function name and the parameter list.
- 7

### Slide 8
- USER DEFINED FUNCTION COMPONENTS
- Function name:
- The name of the function can be anything that you want. The standard is to make it something related to what it's supposed to do. The naming convention follows the same rule as that of variable naming convention in C.
- Function declaration:
- Tells the compiler all about the function. These include the function's name, the return type, and the number and types of parameters. The body of the function having the function definition can be defined somewhere else.
- 8

### Slide 9
- FUNCTION DECLARATION
- A function declaration has the following parts:
- return_type
- function_name
- ( parameter list );
- The example here can be declared as follows:
- int sum(int num1, int num2);
- OR
- return_type
- function_name
- (datatypes)
- int sum(
- int,int
- );
- 9

### Slide 10
- TYPES OF USER DEFINED FUNCTION
- There can be 4 different types of user-defined functions, they are:
- 1. Function with no arguments and no return value.
- 2. Function with no arguments and a return value
- 3. Function with arguments and no return value
- 4. Function with arguments and a return value
- 10

### Slide 11
- Function with no arguments and no return value
- Such functions can either be used to display information or they are completely dependent on user inputs.
- Example:
- It takes 2 numbers as input from user, and display which is the greater number.
- #include<stdio.h>
- void
- greatNum
- (); // function
- declarationint
- main()
- {
- greatNum
- ();        // function call
- return 0;
- }
- void
- greatNum
- () // function definition
- {
- int
- i
- , j;
- printf
- ("Enter 2 numbers that you want to compare...");
- scanf
- ("%
- d%d
- ", &
- i
- , &j);
- if(
- i
- > j)
- {
- printf
- ("The greater number is: %d",
- i
- );
- }
- else
- {
- printf
- ("The greater number is: %d", j);
- }
- }
- 11

### Slide 12
- Function
- with no arguments and a return value
- We have modified the above example to make the function
- greatNum
- () return the number which is greater amongst the 2 input numbers.
- #include<stdio.h>
- int
- greatNum
- ();       // function declaration
- int main()
- {
- int result;
- result =
- greatNum
- ();        // function call
- printf
- ("The greater number is: %d", result);
- return 0;}int
- greatNum
- ()        // function definition
- {
- int
- i
- , j,
- greaterNum
- ;
- printf
- ("Enter 2 numbers that you want to compare...");
- scanf
- ("%
- d%d
- ", &
- i
- , &j);    if(
- i
- > j)
- {
- greaterNum
- =
- i
- ;
- }
- else
- {
- greaterNum
- = j;
- }    // returning the result
- return
- greaterNum
- ;
- }
- 12

### Slide 13
- Function with arguments and no return value
- We are using the same function as example again and again, to demonstrate that to solve a problem there can be many different ways.
- This time, we have modified the above example to make the function
- greatNum
- () take two int values as arguments, but it will not be returning anything.
- #include<stdio.h>
- void
- greatNum
- (int a, int b);       // function
- declarationint
- main()
- {
- int
- i
- , j;
- printf
- ("Enter 2 numbers that you want to compare...");
- scanf
- ("%
- d%d
- ", &
- i
- , &j);
- greatNum
- (
- i
- , j);        // function call
- return 0;
- }
- void
- greatNum
- (int x, int y)        // function definition
- {
- if(x > y)
- {
- printf
- ("The greater number is: %d", x);
- }
- else
- {
- printf
- ("The greater number is: %d", y);
- }
- 13

### Slide 14
- Function with arguments and a return value
- It makes the function completely independent of inputs and outputs, and only the logic is defined inside the function body.
- #include<stdio.h>
- int
- greatNum
- (int a, int b);       // function declaration
- int main()
- {
- int
- i
- , j, result;
- printf
- ("Enter 2 numbers that you want to compare...");
- scanf
- ("%
- d%d
- ", &
- i
- , &j);
- result =
- greatNum
- (
- i
- , j); // function call
- printf
- ("The greater number is: %d", result);
- return 0;
- }
- int
- greatNum
- (int x, int y)        // function definition
- {
- if(x > y)
- {
- return x;
- }
- else {
- return y;    }
- }
- 14

### Slide 15
- Passing Parameters
- Parameter Passing Techniques in C:
- There are different ways in which parameter
- d
- ata can be passed into and out of methods and functions.
- Formal Parameter :
- A variable and its type as they appear in the prototype of the function or method.
- Actual Parameter :
- The variable or expression corresponding to a formal parameter that appears in the function or method call in the calling environment.

### Slide 16
- Examples of Parameter Passing
- 16
- EXAMPLE: Program to find square of a number
- #include<stdio.h>
- float square ( float x );  //function declaration
- int main( )
- {
- float m, n ;
- printf
- ( "\
- nEnter
- some number for finding square \n");
- scanf
- ( "%f", &m ) ;
- n = square ( m ) ;   // function call
- printf
- ( "\
- nSquare
- of the given number %f is %f”,
- m,n
- );
- }
- float square ( float x )   // function definition
- {
- float p ;
- p = x * x ;
- return ( p ) ;
- }

### Slide 17
- How to Call C Functions in a Program
- There are two ways that a C function can be called from a program. F
- unctions can be invoked in two ways:
- Call by Value
- Call by Reference
- .
- These two ways are generally differentiated by the type of values passed to them as parameters.
- Call By Value
- : In this parameter passing method, values of actual parameters are copied to function’s formal parameters and the two types of parameters are stored in different memory locations. So any changes made inside functions are not reflected in actual parameters of caller.
- Call by Reference
- : Both the actual and formal parameters refer to same locations, so any changes made inside the function are actually reflected in actual parameters of caller.
- 17

### Slide 18
- CALL BY VALUE EXAMPLE
- Example: Swap two numbers using
- Call by Value
- #include <
- stdio.h
- >
- void swap(int x, int y);
- int main()
- {
- int a = 2, b = 3;
- swap(a, b);
- printf
- ("a=%d b=%d\n", a, b);
- return 0;
- }
- void swap(int x, int y)
- {
- int  t;
- t = x;
- x = y;
- y = t;
- printf
- ("x=%d y=%d\n", x, y);
- }
- 18

### Slide 19
- CALL BY REFERENCE EXAMPLE
- Example: Swap two numbers using Call by Reference
- #include <
- stdio.h
- >
- void swap(int*, int*);
- int main()
- {
- int a =2, b = 3;
- swap(&a, &b);
- printf
- ("a=%d b=%d\n", a, b);
- return 0;
- }
- void swap(int* c, int* d)
- {
- int  t;
- t = *x;
- *x = *y;
- *y = t;
- printf
- ("x=%d y=%d\n", *x, *y);
- }
- 19

### Slide 20
- SUMMARY
- We have learned the following topics:-
- User- defined Functions
- Parameter Passing
- Call by Value and Call by Reference
- 20

### Slide 21
- Next Lecture
- • Introduction to Recursive Functions
- • Working of Recursion
- • Base Case and Recursive Case
- • Advantages and Limitations of Recursion
- • Programs using Recursive Functions:
- - Factorial
- - Fibonacci Series
- - Sum of Numbers

### Slide 22
- FREQUENTLY ASKED QUESTIONS
- PROGRAMS
- 1.
- Write a program in C to check a given number is even or odd using the function.
- 2. Write a program in C to check whether a number is a prime number or not using the function.
- 3. Write a program in C to check
- armstrong
- numbers using the function.
- 4. Write a program in C to find the sum of the series 1!/1+2!/2+3!/3+4!/4+5!/5 using the   function.
- 5. Write a program to display
- fibonacci
- series
- upto
- user required number using function.
- 22

### Slide 23
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- 1. Choose correct statement about Functions in C Language.
- A) A Function is a group of c statements which can be reused any number of times.
- B) Every Function has a return type.
- C) Every Function may no may not return a value.
- D) All the above.
- 2
- What is the output of C Program with functions.? void show(); int main() { show();
- printf
- ("ARGENTINA "); return 0; } void show() {
- printf
- ("AFRICA "); }
- A) ARGENTINA AFRICA
- B) AFRICA ARGENTINA
- C) ARGENTINA
- D) Compiler error
- 3) How many values can a C Function return at a time.?
- A) Only One Value
- B) Maximum of two values
- C) Maximum of three values
- D) Maximum of 8 values
- 23

### Slide 24
- UTILIZE YOUR KNOWLEDGE TO ANSWER(CONTD.)
- 4 What are types of Functions in C Language.?
- A) Library Functions
- B) User Defined Functions
- C) Both Library and User Defined
- D) None of the above
- 5. Which of the following statement is true about a function with an argument?
- A. No value is pass to the function during function call.
- B. function with an argument must not have return type
- C. function with an argument is declared and define with parameter list
- D. none of the above
- 24

### Slide 25
- REFERENCES
- Video Lectures:
- 1
- .https://www.youtube.com/watch?v=4-xX9vmPDsc
- 2
- .https://www.youtube.com/watch?v=Dt9q3qiaqiA
- Websites:
- 1.https://www.tutorialspoint.com/cprogramming/c_functions.htm
- 2
- .
- https://beginnersbook.com/2014/01/c-function-call-by-value-example/
- 25

### Slide 26
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 27
- Class-wise feedback

### Slide 28
- THANK YOU


## PPT 9 RECURSIVE FUNCTIONS
### Slide 1
- Logical Thinking & Problem Solving
- Course Objectives
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
- • Functions are reusable blocks of code.
- • Used to perform specific tasks.
- • Help in modular and structured programming.
- • Main components:
- - Function Declaration
- - Function Definition
- - Function Call
- • Types:
- - Library Functions
- - User Defined Functions

### Slide 4
- Recursive Functions
- Examples of Recursive Functions
- Macros
- References
- 4
- CONTENTS

### Slide 5
- RECURSIVE FUNCTION
- Definition:
- The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily.
- 5

### Slide 6
- EXAMPLE 1 RECURSIVE FUNCTION
- Example1: Program to find factorial of a number.
- #include <
- stdio.h
- >
- int factorial(int number);
- int main()
- {
- int x = 9;
- printf
- ("The factorial of %d is %d\n", x, factorial(x));
- return 0;
- }
- int factorial(int number)
- {
- if (number == 1)
- return (1); /* exiting condition */
- else
- return (number * factorial(number - 1));
- }
- 6

### Slide 7
- EXPLANATION OF EXAMPLE 1
- 7
- We declare our recursive factorial function which takes an integer parameter and returns the factorial of this parameter. This function will call itself and decrease the number until the exiting, or the base condition is reached. When the condition is true, the previously generated values will be multiplied by each other, and the final factorial value is returned.
- 2. We declare and initialize an integer variable with value"6" and then print its factorial value by calling our factorial function.

### Slide 8
- EXAMPLE 2 RECURSIVE FUNCTION
- Example2: Write a program in C to print first 50 natural numbers using recursion
- .
- #include<stdio.h>
- int
- numPrint
- (int);
- int main()
- {
- int n = 1;
- printf
- ("\n\n Recursion : print first 50 natural numbers :\n");
- printf
- ("-------------------------------------------------\n");
- printf
- (" The natural numbers are :");
- numPrint
- (n);
- printf
- ("\n\n");
- return 0;
- }
- int
- numPrint
- (int n)
- {
- if(n<=50)
- {
- printf
- (" %d ",n);
- numPrint
- (n+1);
- }
- }
- 8

### Slide 9
- EXPLANATION OF EXAMPLE 2 USING FLOWCHART
- 9

### Slide 10
- MACROS
- Macros:
- They are basically a fragment of the code that has been given a name. The name is replaced by the contents of the macro, whenever the name is used.
- A macro is an operation defined in #define preprocessor directive. As with symbolic constants, the macro-identifier is replaced in the program with the replacement-text before the program is compiled.
- Macros may be defined with or without arguments. - A macro without arguments is processed like a symbolic constant while a macro with arguments, the arguments are substituted in the replacement text, then the macro is expanded, that is the replacement-text replaces the identifier and argument list in the program
- 10

### Slide 11
- EXAMPLE OF MACROS
- Example: Program to calculate area of circle using macros.
- #include
- #define PI 3.1415
- int main()
- {
- float
- radius,area
- ;
- printf
- ("
- Plese
- Enter the radius ");
- scanf
- ("%f", &radius);
- //Here used the value  of PI
- area = PI*radius*radius;
- printf
- ("Area=%.2f",area);
- return 0;
- }
- 11

### Slide 12
- SUMMARY
- We have learned the following topics:-
- Recursive Functions
- Macros
- 12

### Slide 13
- Next Lecture
- • Introduction to Pointers
- • Declaration and Initialization
- • Address and Dereference Operators
- • Pointer Arithmetic
- • Relationship between Arrays and Pointers
- • Programs using Pointers

### Slide 14
- FREQUENTLY ASKED QUESTIONS
- PROGRAMS
- 1.
- Write a program in C to calculate the sum of numbers from 1 to n using recursion.
- 2. Program
- of
- fibonacci
- program using recursion
- 3.
- C program to calculate length of the string using recursion
- 4.
- Program to count digits in C using recursion
- 14

### Slide 15
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- 1. What will be the value retuned by the following function, when it is called with a value 11?
- recur(int num)
- if ( ( num/2) !=0 )
- return ( recur(num/2 ) * 10+num%2 );
- else return 1;
- Function does not return any value, because it goes into an infinite loop
- B.11
- C.1011
- D. None of the above
- 15

### Slide 16
- UTILIZE YOUR KNOWLEDGE TO ANSWER(Contd.)
- 2
- . In the absence of a exit condition in a recursive function, the following error is given __________
- a) Compile time error
- b) Run time error
- c) Logical error
- d) No error
- 3
- . Iteration requires more system memory than recursion.
- a) True
- b) False
- 16

### Slide 17
- REFERENCES
- Video Lectures
- 1. https://beginnersbook.com/2014/01/c-strings-string-functions/
- Websites:
- 1.
- https://www.programiz.com/c-programming/c-recursion
- 2.https://www.cprogramming.com/tutorial/c/lesson16.html
- 3
- .https://www.tutorialspoint.com/macros-and-preprocessors-in-c
- 17

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
- THANK YOU
