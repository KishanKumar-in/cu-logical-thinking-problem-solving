# Chapter 1.2 - All Lecture Slides Text


## 4 Structure of C program
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
- Chapter No.   2                                        Lecture No.5
- Topic :
- Structure of C program
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
- A C program is organized into different sections such as documentation, header files, global declarations, main() function, and user-defined functions.
- Header files are included using #include directives to access predefined library functions.
- The main() function acts as the entry point where program execution begins.
- Variable declarations, input/output statements, and executable instructions are written inside functions to perform specific tasks.
- User-defined functions help in modular programming, code reusability, and better program organization.

### Slide 5
- Structure of C program
- Compilation and Execution process
- Program demonstration
- 5
- CONTENTS

### Slide 6
- Structure of C program
- 6
- Structure of C program is defined by set of rules called protocol, to be followed by programmer while writing C program. All C programs are having sections/parts which are mentioned  here.

### Slide 7
- STRUCTURE OF C PROGRAM- EXAMPLE
- Sample text here (16)
- 7
- Figure 2.3. Program 1 (executed on Dev-C++ IDE)

### Slide 8
- STRUCTURE OF C PROGRAM- EXAMPLE
- 8
- Figure 2.4. Program 1 output (executed on Dev-C++ IDE)

### Slide 9
- ü
- Documentation Section
- The documentation section consists of a set of comment lines, giving the name of the program, the author and other details, which the programmer would like to use later. The comments can be written in two ways:
- a)      Multi-line comment
- /* This is a
- multi-line
- comment */
- Ex: /* Author : Aman
- Date:10/06/2020 */
- b)      Single-line comment
- // This is a single-line comment
- // Author: Aman
- 9

### Slide 10
- 10
- ü
- Link Section
- The link section provides instructions to the compiler to link functions from the system library.
- If we want to access the functions stored in the library, it is necessary to tell the compiler about the files to be accessed. This is achieved by using the preprocessor directive #include as follows:
- #include<filename>
- where
- filename is the name of the library file that contains the required function definition. Preprocessor directives are placed at the beginning of the program. Some of
- the
- examples are:
- #include<
- stdio.h
- >
- #include<
- conio.h
- >
- #include<
- math.h
- >

### Slide 11
- 11
- ü
- Definition Section
- The definition section defines all symbolic constants.
- A #define is a preprocessor compiler directive and not a statement. Therefore #define lines should not end with a semicolon.
- Symbolic constants are usually written in uppercase so that they are easily distinguished from lowercase variable names.
- e.g.   #define YEAR 2014
- #define  PI 3.14
- ü
- Global Declaration Section
- There are some variables that are used in more than one function. Such variables are called global variables and are declared in the global declaration section.
- This section also declares all the user-defined functions.

### Slide 12
- 12
- ü
- main( ) Function Section
- Every C program must have one main( ) function section. This section contains two parts, declaration part and executable part.
- The declaration part declares all the variables used in the executable part.
- These two parts must appear between the opening and the closing braces.
- The program execution begins at the opening brace and ends at the closing brace. The closing brace of the main function section is the logical end of the program.
- All the statements in the declaration and executable parts end with a semicolon (
- ;
- ).

### Slide 13
- ü
- Subprogram Section
- 13
- The subprogram section contains all the user-defined functions that are called in the main functions. User-defined functions are generally placed immediately after the main function, although they may appear in any order.

### Slide 14
- Rules to write c program
- All C statements must end with semicolon.
- C is case-sensitive. That is, upper case and lower case characters are different. Generally the statements are typed in lowercase.
- C statement can be written in one line or it can split into multiple lines.
- Braces must always match upon pairs, i.e., every opening brace { must have a matching closing brace }.
- Every C program starts with  main() function.
- 14

### Slide 15
- Documentation
- Pre-processor directive
- main function
- 15
- Main function body
- Begin
- End
- Statement
- First example program:

### Slide 16
- Need of compiler:
- 16

### Slide 17
- Compilation & Execution process
- 17
- File1.i
- File1.c
- File1.o or File1.obj
- File1.exe
- Final output

### Slide 18
- KEYWORDS IN C
- 18

### Slide 19
- 19
- Summary

### Slide 20
- Next Lecture
- Input and output functions are used to communicate between the user and the program.
- printf
- () is an output function used to display messages and results on the screen.
- scanf
- () is an input function used to accept data from the user during program execution.
- Format specifiers such as %d, %f, %c, and %s are used to read and display different data types.
- Input/output functions are available through the standard input-output header file
- stdio.h
- .

### Slide 21
- Frequently Asked question
- Q1
- Differentiate compiler and interpreter.
- Compiler
- transforms code written in a high-level programming language into the machine code, at once, before program runs, whereas an
- Interpreter
- coverts each high-level program statement, one by one, into the machine code, during program run. Compiled code runs faster while interpreted code runs slower.
- Q2 what is the need of preprocessing ?
- The C preprocessor is the
- macro preprocessor for the C programming language
- . The preprocessor provides the ability for the inclusion of header files, macro expansions, conditional compilation, and line control. In many C implementations, it is a separate program invoked by the compiler as the first part of translation.
- 21

### Slide 22
- Assessment Questions
- :
- Q Choose the correct option
- Q1 Role of Linker is:
- Link with compiler
- Link with system libraries
- Link with assembler
- generate output
- Q2 After compilation which file is created
- file.c
- file.obj
- file.exe
- file.I
- 22
- Q3 Which of the following is  type of an error:
- Syntax error
- Logic error
- Data error
- All above
- Q4 Correct documentation syntax is:
- / hello world program /
- // hello world program
- //* hello world program
- // hello world program //

### Slide 23
- 23
- Q5 Explain the role of pre-processor.
- Q6 What is the need of compilation?
- Q7 Design a program to display your details including name, Father’s name and grades in 12
- th
- .
- Q8 Discuss the need of main function in program.
- True/False
- Q9   Header file contains definition of predefined functions
- Q10 Termination symbol is optional for statements written in main()
- T/F

### Slide 24
- Discussion forum
- .
- Future Scope of C
- https://www.youtube.com/watch?v=5Kg4q0Vq5UU
- Students, have a look at this video and mention your views in
- BB classroom
- 24

### Slide 25
- REFERENCES
- Reference Books:
- [1] Programming in C by Reema
- Thareja
- .
- [2] Programming in ANSI C by E.
- Balaguruswamy
- , Tata McGraw Hill.
- [3] Programming with C (
- Schaum's
- Outline Series) by Byron Gottfried  Jitender Chhabra, Tata McGraw Hill.
- [4] The C Programming Language by Brian W. Kernighan, Dennis Ritchie, Pearson education.
- Website:
- https://www.youtube.com/watch?v=KnvbUiSxvbM&list=PL98qAXLA6aftD9ZlnjpLhdQAOFI8xIB6e
- GeeksforGeeks
- . C Language Introduction -
- GeeksforGeeks
- . [online] Available at:
- https://www.geeksforgeeks.org/c-language-set-1-introduction/
- Video Links:
- NPTEL https://www.youtube.com/watch?v=VSU7EaHMzl8&list=PLJvIzs_rP6R73WlvumJvCQJrOY3U5zq1j&index=5&t=615s
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
- Class-wise
- feedback
- 27


## 5 Input Output Functions
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.
- 1
- Chapter No.   2                                        Lecture
- No.6
- Topic :
- Input/Output Statement
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
- Recap of Previous Lecture

### Slide 5
- 5
- Contents

### Slide 6
- 6
- I/O Statements
- I/O
- Statements

### Slide 7
- 7
- I/O types
- I/O Types

### Slide 8
- 8
- Functions
- Description
- scanf()
- This is formatted input function used to read one or many Inputs from standard input device keyboard
- printf()
- This is formatted output function used to print one or many Values on  standard output device monitor .
- Formatted I/O Functions

### Slide 9
- 9
- Scanf
- ()
- scanf(<control string>, &address1,&address2, . .&
- addressn
- );
- & (ampersand) is used with each variable to access its address
- It is a formatted input function
- , format specifiers are provided in
- control string
- Scanf
- ()

### Slide 10
- 10
- Scanf
- ()
- printf
- (“   Text  ”);
- printf
- (“Text  <control string>  Text”,
- Variable_name
- );
- It is a formatted output function
- , format specifiers are provided in
- control string.
- printf
- ()

### Slide 11
- 11
- Functions
- Description
- %d and  %u
- Used for signed and unsigned int variables respectively
- %ld and %
- lu
- Used for signed and unsigned long
- variables respectively
- %c
- and %s
- Used for character and string variables respectively
- %lf and %Lf
- Used for double
- and
- long
- double
- variables respectively
- Format Specifiers

### Slide 12
- 12
- #include <
- stdio.h
- > // header file used for standard I/O
- int main()
- {
- int age; //Integer variable to store age of student
- int roll; // Integer variable to store roll number of student
- printf
- ("Enter the data");
- scanf
- ("%
- d%d
- ", &age, &roll); //format specifier
- printf
- ("Age=%d\
- n",age
- ); // Print age on standard Output
- printf
- ("Roll No.=%d\
- n",roll
- ); // Print Roll. No. on standard Output
- return 0; // return to C system from where main() was called
- }
- Example1- Use Of
- printf
- () and
- scanf
- ()

### Slide 13
- 13
- Indentation in programming is used to make program easier to read and understand .
- Indentation In C
- #include <
- stdio.h
- >
- int main()
- {
- printf
- ("Hello World");
- return 0;
- }
- #include <
- stdio.h
- >
- int main()
- {
- printf
- ("Hello World");
- return 0;
- }

### Slide 14
- 14
- Header file is that which consists of functions , macros and variable declarations .
- It is stored with .h extension .
- Every program includes at least one header file named <stdio.h> it includes declarations of standard input and output functions scanf() and printf()
- Header Files

### Slide 15
- 15
- predefined header files : are those which are inbuilt into C system like stdio.h. Inbuilt header files are included in < > pair as :
- #include<stdio.h>
- User Defined Header Files : User can write their own header files and can include into C programs . The user defined header files are included in “ “  (Double quotes).
- Types Of Header Files

### Slide 16
- 16
- Functions
- Description
- getchar()
- This function is used to read a single character from keyboard .
- putchar()
- This function is used to print a single character on
- standard O/P screen
- .
- gets()
- It
- can be used to read  strings .
- scanf
- () is not capable to read spaces but gets() can
- puts()
- string read by gets () can be printed using puts() function .
- Unformatted I/O Functions

### Slide 17
- 17
- #include <
- stdio.h
- >
- int main()
- { char
- ch
- ;
- printf
- ("\n press y /Y for yes or n/N for no ");
- ch
- =
- getchar
- (); // Read single char from keyboard
- //
- scanf
- (
- "%c"
- ,&
- ch
- );
- putchar
- (
- ch
- );
- printf
- ("\n");
- //
- printf
- (
- "%c"
- ,
- ch
- );
- return 0;
- }
- Use Of
- getchar
- () and
- putchar
- ()

### Slide 18
- 18
- #include <
- stdio.h
- >
- int main()
- {
- int x; float y; char z;
- scanf
- ("%3d%4f", &x, &y);
- printf
- ("%3d\n%.2f",x,y);
- return 0;
- }
- Role of Format specifiers in reading

### Slide 19
- 19
- #include <stdio.h>
- main()
- {
- float a = 987.361;
- printf("/%f/\n", a);
- printf("/%12f/\n", a);
- printf("/%-12f/\n", a);
- printf("/%4f/\n", a);
- printf("/%.4f/\n", a);
- printf("/%.2f/\n", a);
- }
- Output:
- /987.361000/	    //when no precision is specified,the default precision is 6
- places after decimal
- /   987.361000/       // 2 blank spaces introduced before the output
- because space is of 12 chars
- /987.361000 /        // 2 blank spaces introduced after the output
- /987.361000/	 // The width specifier 4 is ignored because chars
- are more
- /987.3610/           // precision is controlled to 4 , default of 6 is overridden
- /987.4/	              // when precision is overridden rounding of value will occur
- Role of Format
- specifiers
- in printing

### Slide 20
- 20
- #include <
- stdio.h
- >
- int main()
- {
- char str[81];
- puts("Enter a line of text:\n");
- gets(str);
- puts("You entered:\n");
- //
- printf
- ("%
- s",str
- );
- puts(str);
- }
- Use Of gets() and puts()

### Slide 21
- 21
- Format specifiers
- I/O Statements
- Formatted and Unformatted I/O
- Indentation
- Header Files
- Are used to read values from keyboard and write values on standard O/P screen.
- Format specifiers are allowed in formatted I/O but not in unformatted I/O
- Are used to format input and output according to user requirements
- Makes program easier to read and understand
- Are used include functions, macros and variable declarations
- Summary

### Slide 22
- 22

### Slide 23
- 23

### Slide 24
- 24
- Test
- Yourself

### Slide 25
- Next Lecture
- A C program is organized into different sections such as documentation, header files, global declarations, main() function, and user-defined functions.
- Header files are included using #include directives to access predefined library functions.
- The main() function acts as the entry point where program execution begins.
- Variable declarations, input/output statements, and executable instructions are written inside functions to perform specific tasks.
- User-defined functions help in modular programming, code reusability, and better program organization.

### Slide 26
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

### Slide 27
- References
- S.No
- Title
- Content link
- 8
- Weblink
- https://www.studytonight.com/c/
- 9
- Weblink
- https://en.cppreference.com/index.php?title=c/language/expressions&utm_source=chatgpt.com#Operators
- 10
- Video Link
- https://www.youtube.com/watch?v=cEfuwpbGi1k
- 11
- Video Link
- https://www.youtube.com/watch?v=qmd5sVFOgpg
- 12
- Online Course Link
- https://www.coursera.org/

### Slide 28
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 29
- Class-wise
- feedback
- 29

### Slide 30
- THANK YOU


## 6 Data Types and variables
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
- Format specifiers
- I/O Statements
- Formatted and Unformatted I/O
- Indentation
- Header Files
- Are used to read values from keyboard and write values on standard O/P screen.
- Format specifiers are allowed in formatted I/O but not in unformatted I/O
- Are used to format input and output according to user requirements
- Makes program easier to read and understand
- Are used include functions, macros and variable declarations
- Recap of previous Lecture

### Slide 4
- 4
- C0NTENTS
- Contents

### Slide 5
- 5
- Data Types
- Data
- types

### Slide 6
- 6
- Data
- T
- ypes
- - Categories
- Data
- types

### Slide 7
- 7
- Data
- types

### Slide 8
- 8
- Data Type
- Memory Space
- Range Of Values
- Format Specifiers
- Signed char
- 1 Byte
- -128 To +127
- %c
- Unsigned char
- 1 Byte
- 0 To 255
- %c
- signed
- int
- 2 Bytes
- -32768 to +32767
- %d
- unsigned int
- 2 Bytes
- 0 to 65535
- %u
- signed long
- 4 Bytes
- -2147483648
- To
- 2147483647
- %ld
- unsigned long
- 4 Bytes
- 0 To 4294967295
- %
- lu
- Data
- types Size Chart

### Slide 9
- 9
- Data Type
- Memory Space
- Range Of Values
- Format
- Specifiers
- signed long
- long
- int
- 8 Bytes
- -9223372036854775808
- To
- 9223372036854775807
- %
- lld
- unsigned long
- long
- int
- 8 Bytes
- 0
- To
- 18446744073709551615
- %
- llu
- float
- 4 Bytes
- -3.4 E38
- To
- +3.4E38
- %f
- double
- 8 Bytes
- -1.7E308
- To
- +1.7E308
- %lf
- Data
- types Size Chart

### Slide 10
- 10
- Data
- types
- Steps to remember

### Slide 11
- 11
- Constants
- Constants are the quantities that do not change their value
- during execution of the program .
- Constants

### Slide 12
- 12
- Integer Constants

### Slide 13
- 13
- Real Constants

### Slide 14
- 14
- Character Constant
- Character Constants

### Slide 15
- 15
- String  Constant
- String Constants

### Slide 16
- 16
- How to Define Constants ?

### Slide 17
- 17
- How to Define Constants ?

### Slide 18
- 18
- Variables
- Variables

### Slide 19
- 19
- Naming The Variables

### Slide 20
- 20
- Lva
- Lvalue
- Rvalue

### Slide 21
- 21
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
- Summary

### Slide 22
- Next Lecture
- Expressions in C
- Types of expressions
- Operator precedence
- Associativity rules
- Evaluation of expressions
- Type conversion and casting
- Practice problems on expression evaluation

### Slide 23
- 23

### Slide 24
- 24

### Slide 25
- 25
- Test
- Yourself

### Slide 26
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

### Slide 27
- References
- S.No
- Title
- Content link
- 8
- Weblink
- https://www.studytonight.com/c/
- 10
- Video Link
- https://www.youtube.com/watch?v=OSyjOvFbAGI
- 11
- Video Link
- https://www.youtube.com/watch?v=d7tdL-ZEWdE

### Slide 28
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 29
- Class-wise
- feedback
- 29

### Slide 30
- THANK YOU


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


## 8 Bitwise operator and typecasting
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Unit No.
- 1
- Chapter No.
- 2
- Lecture No.
- 9
- Topic :
- Bitwise Operator
- Faculty Name-Dr. Sheenam
- E_Code
- - E6717                                                                                                      Designation-Assistant Professor

### Slide 2
- INSTITUTE - UIE
- Department of
- Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester
- Jul-Dec 2026
- Unit No.
- 1
- Chapter No.   1                                        Lecture No.1
- Topic : H
- ands on session on Flowcharts
- Faculty Name-Dr. Sheenam
- E_Code
- - E6717
- Designation-Assistant Professor

### Slide 3
- Logical Thinking & Problem Solving
- Course Objectives
- 3
- The course aims to provide a strong foundation in problem-solving using the C programming language.
- It enhances students' programming skills by developing logical thinking and algorithmic problem-solving abilities
- By mastering C programming concepts, students will be able to design and implement efficient solutions for real-world problems

### Slide 4
- 4
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

### Slide 5
- Recap of Previous Lecture
- Important points to remember:
- C operators operates on one or more operands to produce a value.
- The operators that take one operand are called unary operators.
- The operators that require two operands are called binary operators.
- The operator that accepts three operands is called ternary operator. C  has only one ternary operator.

### Slide 6
- Space for visual (size 24)
- Bitwise operator
- Type Casting/ Type Conversion
- 6
- CONTENTS
- 11-08-2026

### Slide 7
- An operator is a symbol that tells the compiler to perform certain mathematical or logical manipulations.
- Operators are used in program to manipulate data and variables. The data items that operators act upon are called operands.
- Some operators require two operands, while others act upon only one operand. The operators are classified into unary, binary and ternary depending on whether they operate on one, two or three operands respectively
- .
- 11-08-2026
- Operators
- 7

### Slide 8
- In arithmetic-logic unit (which is within the CPU), mathematical operations like: addition, subtraction, multiplication and division are done in bit-level.
- Decimal values are converted into binary values which are the sequence of bits and bit wise operators work on these bits.
- Table1: Truth table of Bitwise operations
- 11-08-2026
- Bitwise Operator
- 8
- X
- Y
- X|Y
- X&Y
- X^Y
- 0
- 0
- 0
- 0
- 0
- 0
- 1
- 1
- 0
- 1
- 1
- 0
- 1
- 0
- 1
- 1
- 1
- 1
- 1
- 0

### Slide 9
- Bitwise operators are as follows:
- 11-08-2026
- Bitwise Operator
- 9
- Operator
- Meaning of operator
- &
- Bitwise And
- |
- Bitwise Or
- ^
- Bitwise XOR
- ~
- Bitwise Compliment
- <<
- Left Shift
- >>
- Right
- Shift

### Slide 10
- Bitwise AND
- 12 = 00001100 (In Binary)
- 25 = 00011001 (In Binary)
- Bit Operation of 12 and 25
- 00001100
- & 00011001
- ________
- 00001000  = 8 (In decimal)
- 11-08-2026
- Bitwise Operator
- 10

### Slide 11
- Bitwise OR
- 12 = 00001100 (In Binary)
- 25 = 00011001 (In Binary)
- Bitwise OR Operation of 12 and 25
- 00001100
- | 00011001
- ________
- 00011101  = 29 (In decimal)
- 11-08-2026
- Bitwise Operator
- 11

### Slide 12
- Bitwise XOR
- 12 = 00001100 (In Binary)
- 25 = 00011001 (In Binary)
- Bitwise XOR Operation of 12 and 25
- 00001100
- ^ 00011001
- ________
- 00010101  = 21 (In decimal)
- 11-08-2026
- Bitwise Operator
- 12

### Slide 13
- Bitwise Compliment
- 35 = 00100011 (In Binary)
- Bitwise complement Operation of 35
- ~ 00100011
- ________
- 11011100  = 220 (In decimal)
- 11-08-2026
- Bitwise Operator
- 13

### Slide 14
- Bitwise Right shift
- 212 = 11010100 (In binary)
- 212>>2 = 00110101 (In binary) [Right shift by two bits]
- 212>>7 = 00000001 (In binary)
- 212>>8 = 00000000
- 212>>0 = 11010100 (No Shift)
- 11-08-2026
- Bitwise Operator
- 14

### Slide 15
- Bitwise Left shift
- 212 = 11010100 (In binary)
- 212<<1 = 110101000 (In binary) [Left shift by one bit]
- 212<<0 =11010100 (Shift by 0)
- 212<<4 = 110101000000 (In binary) =3392(In decimal)
- 11-08-2026
- Bitwise Operator
- 15

### Slide 16
- #include <
- stdio.h
- >
- int main()
- {
- int a = 12, b = 25; //12=00001100,25=00011001
- printf
- ("Output = %d\n",
- a&b
- ); // &=00001000=8
- printf
- ("Output = %d\n",
- a|b
- ); // |=00011101=29
- printf
- ("Output = %d\n",
- a^b
- ); // ^=00010101=21
- printf
- ("Output = %d\n", ~a); //~a=11110011=243=-(2's complement of 243)=-13
- printf
- ("Output = %d\n", a>>4); //00000000
- printf
- ("Output = %d", a<<4); //11000000
- return 0;
- }
- 11-08-2026
- Bitwise Operator
- 16

### Slide 17
- What will be the output of the C program?
- #include<
- stdio.h
- >
- int
- main()
- {
- int
- a = 4, b = 2;
- printf
- ("
- a^b
- = %d",
- a^b
- );
- return 0;
- }
- A. 12
- B. 10
- C. 8
- D. 6
- 11-08-2026
- TRY IT
- 17

### Slide 18
- The type conversion process in C is basically converting one type of data type to other to perform some operation.
- The conversion is done only between those
- datatypes
- wherein the conversion is possible ex – char to
- int
- and vice versa.
- It’s of two types
- 
- Implicit Type Conversion
- Ex
- plicit Type Conversion
- 18
- Type-Casting/Type-Conversion
- 11-08-2026

### Slide 19
- 
- Implicit Type Conversion
- This type of conversion is usually performed by the compiler when necessary without any commands by the user. Thus it is also called "Automatic Type Conversion".
- The compiler usually performs this type of conversion when a particular expression contains more than one data type. In such cases either type promotion or demotion takes place.
- 19
- Type-Casting/Type-Conversion
- 11-08-2026

### Slide 20
- 
- Implicit Type Conversion
- 20
- Type-Casting/Type-Conversion
- 11-08-2026

### Slide 21
- Rules:
- char or short type operands will be converted to
- int
- during an operation and the outcome data type will also be int.
- If an operand of type long double is present in the expression, then the corresponding operand will also be converted to long double same for the double data type.
- If an operand of float type is present then the corresponding operand in the expression will also be converted to float type and the final result will also be float type.
- If an operand of unsigned long
- int
- is present then the other operand will be converted to unsigned long
- int
- and the final result will also be unsigned long int.
- If an operand of long
- int
- is present then the other operand will be converted to long
- int
- and the final result will also be long int.
- If an operand of unsigned
- int
- is present then the other operand will be converted to unsigned
- int
- and the final result will also be unsigned int.
- 21
- Type-Casting/Type-Conversion
- 11-08-2026

### Slide 22
- 
- Implicit Type Conversion
- Example 1
- int
- a = 20;
- double b = 20.5;
- a + b;
- Here, first operand is
- int
- type and other is of type double. So, as per rule 2, the variable a will be converted to double. Therefore, the final answer is double a + b = 40.500000.
- Example 2
- char
- ch
- ='a';
- int
- a =13;
- a +
- ch
- ;
- Here, first operand is char type and other is of type int. So, as per rule 1, the char variable will be converted to
- int
- type during the operation and the final answer will be of type int. We know the ASCII value for
- ch
- is 97. Therefore, final answer is a +
- ch
- = 97 + 13 = 110.
- 22
- Type-Casting/Type-Conversion
- 11-08-2026

### Slide 23
- 
- Ex
- plicit Type Conversion
- Explicit type conversion rules out the use of compiler for converting one data type to another instead the user explicitly defines within the program the
- datatype
- of the operands in the expression.
- 23
- Type-Casting/Type-Conversion
- 11-08-2026

### Slide 24
- 
- Ex
- plicit Type Conversion
- 24
- Type-Casting/Type-Conversion
- 11-08-2026

### Slide 25
- Ex
- plicit Type Conversion Example:
- Example:
- double
- da
- = 4.5;
- double db = 4.6;
- double dc = 4.9;
- //explicitly defined by user
- int
- result = (
- int
- )
- da
- + (
- int
- )db + (
- int
- )dc;
- printf
- ("result = %d", result);
- Output
- result = 12
- 25
- Type-Casting/Type-Conversion
- 11-08-2026

### Slide 26
- Summary
- Keep in mind the following rules for programming practice when dealing with different data type to prevent from data loss :
- Integers types should be converted to float.
- Float types should be converted to double.
- Character types should be converted to integer.

### Slide 27
- N
- ext
- Lecture
- Operator Precedence
- Associativity Rules
- Evaluation of Expressions
- Type Conversion in Expressions
- Practice Problems and Output Prediction

### Slide 28
- Q1.  Compute the sign of an integer?
- Q2.  Detect if two integers have opposite signs?
- Q3.  Write a program to check an integer is a power of 2?
- Q4.  How to set a particular bit in C?
- Q5. When should a type cast not be used?
- 11-08-2026
- FAQ’s
- 28

### Slide 29
- Q1. WAP to clear a bit.
- Q2. We define S  to be a sequence of distinct sequential integers from 1 to n ; in other words S={1,2,3,….n}, .  We want to know the maximum bitwise AND value of any two integers,  a and b (where a<b ), in sequence S  that is also less than a given integer, k . Complete the function in the editor so that given n  and k , it returns the maximum
- a&b
- <k .
- Note: The  &symbol represents the bitwise AND operator.
- Sample Input 0
- 3
- 5 2
- 8 5
- 2 2
- Sample Output 0
- 1
- 4
- 0
- Write the code of the above scenario that satisfies the above situation.
- 11-08-2026
- Assessment
- 29

### Slide 30
- Q 3. What will be the output of the C program?
- #include<
- stdio.h
- >
- int
- main()
- {
- int
- a = 4, b = 2;
- printf
- ("
- a^b
- = %d",
- a^b
- );
- return 0;
- }
- A. 12
- B. 10
- C. 8
- D. 6
- 11-08-2026
- Assessment
- 30

### Slide 31
- Q4. What will be the output of the C program?
- #include<
- stdio.h
- >
- int
- main()
- {
- int
- a = 4, b = 2;
- printf
- ("
- a^b
- = %d",
- a^b
- );
- return 0;
- }
- A. 12
- B. 10
- C. 8
- D. 6
- Q5. [
- &
- ] is the symbol
- of Bitwise
- And.
- Q6. [float to char pointer] type of conversion is NOT accepted.
- 11-08-2026
- Assessment
- 31

### Slide 32
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

### Slide 33
- References
- S.No
- Title
- Content link
- 8
- Weblink
- https://www.studytonight.com/c/
- 10
- Video Link
- https://www.youtube.com/watch?v=MyxVAq9MifI
- 11
- Video Link
- https://www.youtube.com/watch?v=xXBitioUzf8

### Slide 34
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 35
- Class-wise
- feedback
- 35

### Slide 36
- THANK YOU


## 9 Expressions.
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.   1                           Chapter No.   2                                        Lecture No.10
- Topic : Expressions
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
- R
- ecap
- of Previous Lecture
- Operators in C are used to perform arithmetic, logical, relational, assignment, and bitwise operations on data and variables
- Different operators help in calculations, comparisons, decision-making, and efficient data manipulation.
- Bitwise operators perform operations at the binary level and are useful in low-level programming and optimization.
- Type casting is the process of converting one data type into another to ensure proper computation and compatibility.

### Slide 5
- EXPRESSIONS & THEIR EVALUATION
- IN
- C PROGRAMMING

### Slide 6
- What is an Expression ?
- The symbols which are used to perform logical and mathematical operations are called  operators.
- These C operators join individual constants and variables to form expressions.
- Operators, functions, constants and variables are combined to form expressions
- .
- Expression                                                           A + B * 5
- Operators                                                               +, *
- Variables                                                              A, B
- Constant                                                                    5

### Slide 7
- Expression
- Examples
- Expression could as simple as :
- sum = num1 + num2
- Example to convert mathematical equations to C expression,
- 𝐴
- =
- 𝜋
- 𝑟
- 2
- 3.14*r*r
- 1
- 𝑥
- 2
- +
- 𝑦
- 2
- 1 / ((x*x) + (y*y))
- 𝑥
- =
- 𝑏
- 2
- −4
- 𝑎𝑐
- 1 / (pow(x, 2) + pow(y, 2))
- x = sqrt((b*b) – 4*a*c)
- or

### Slide 8
- LET’S LEARN……
- EXPRESSION EVALUATION

### Slide 9
- Precedence & Associativity
- The precedence of operators determines which operator is executed first if there is more than one operator in an expression
- .
- Let us consider an example:
- Int x = 35 – 5 * 6
- First, 5 * 6 will execute as precedence of “*” is higher than “–” operator
- 5 * 6 = 30
- After multiplication, the result will be used for subtraction
- 35 – 30 = 5
- Final output : 5

### Slide 10
- Precedence
- &
- Associativity

### Slide 11
- Associativity of Operators
- If two operators of the same precedence (priority) are present, associativity determines the direction in which they execute.
- Int x
- = 2 * 4 + 5 % 1
- First, precedence of “*” and “%” is higher than “+” operator. Which operator you will choose ?
- Confused ? let’s check associativity now, it says move from left to right.
- 1.
- First
- “*”
- 2.
- Second “%” than
- “+”
- Output
- 
- 2 * 4 = 8
-  8 + 5 % 1  8 + 0  8

### Slide 12
- Let’s try another    example ….

### Slide 14
- In a nutshell….. Let’s summarize
- We learned about writing expressions in c language
- Precedence and associativity rules for solving expressions
- Implementation examples of expressions in c
- 1
- 3
- 2

### Slide 15
- Concepts to be Covered
- Introduction to Decision Making
- if Statement
- if-else Statement
- Nested if Statement
- else-if Ladder
- switch Statement
- Conditional (Ternary) Operator
- Difference between if-else and switch
- Programs Based on Decision Control
- Next Lecture

### Slide 16
- FAQs
- Try practicing these frequently asked questions based on the knowledge received from expression solving in c language…..
- Solve all these expressions…..
- 1.    What number will
- z
- in the sample code given below?
- int z, x=5, y= -10, a=4, b=2;
- z=x++ - --y *b/a;
- 2.    let x=1, y=2, z=3
- z *= ++y + 5;
- 3.  a) ((
- a+b
- ) * c)/d;     for all take a=20, b=10, c=15, d=5
- b) (
- a+b
- )*(c/d);
- c) a + (b*c)/d;

### Slide 17
- Assessment
- Try practicing these frequently asked questions based on the knowledge received from expression solving in c language…..
- Write down the output …….
- #include <
- stdio.h
- >
- int main()
- {
- int x, y = 5, z = 5;
- x = y == z;
- printf
- ("%d", x);
- return 0;
- }

### Slide 18
- Assessment
- Try practicing these frequently asked questions based on the knowledge received from expression solving in c language…..
- Write down the output …….
- #include <
- stdio.h
- >
- int main()
- {
- int
- i
- = 5, j = 10, k = 15;
- printf
- ("%d ",
- sizeof
- (k /=
- i
- + j));
- printf
- ("%d", k);
- return 0;
- }

### Slide 19
- DISCUSION FORUM
- There are three kinds of associativity
- 1.The Associative property in mathematics
- 2.Order of Operations in programming languages
- 3. Associativity in CPU caches.
- All these types implies the same meaning like what you have studied? What you think ?

### Slide 20
- References
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
- [1] https://www.tutorialspoint.com/article/what-is-c-operator-precedence-and-associativity

### Slide 21
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 22
- Class-wise
- feedback
- 22

### Slide 23
- THANK YOU
