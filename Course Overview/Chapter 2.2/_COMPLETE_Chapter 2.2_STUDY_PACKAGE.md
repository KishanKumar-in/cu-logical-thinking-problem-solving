# Chapter 2.2 - Complete Study Material


## 🖥️ PRESENTATION SLIDES


# Chapter 2.2 - All Lecture Slides Text


## PPT 4 Array
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
- Jump statements change the normal flow of execution.
- break exits a loop or switch statement.
- continue skips the current loop iteration.
- goto
- transfers control to a labeled statement.
- return exits a function and returns a value.
- Used for efficient program control and looping operations.

### Slide 4
- Scheme of Evaluation
- 4
- S. No.
- Direct Evaluation Instruments
- Weightage of actual conduct
- Assessment tool
- Frequency of
- Task
- Final Weightage in Internal Assessment
- 1
- Unit-1 Practical Evaluation
- 15 Marks
- Code-Blocks & Dev C
- 3
- 45
- 2
- Unit-2 Practical Evaluation
- 15 Marks
- Hacker Rank
- 3
- Unit-3 Practical Evaluation / Mini Project
- 15 Marks
- Code Fix problems
- 4
- Lab MST
- 15 Marks for one MST
- Online GDB compiler
- 1 per semester
- 15
- 5
- External Exam
- 40 Marks
- Hacker Rank
- 1 per semester
- 40
- 6
- Attendance
- NA
- NA
- NA
- NA

### Slide 5
- Array
- Types of Array
- Declaration of One Dimensional Array
- Initialization of One Dimensional Array
- Examples
- References
- 5
- CONTENTS

### Slide 6
- ARRAY
- In C programming, one of the frequently arising problem is to handle similar types of data.
- For example
- : If the user want to store marks of 100 students. This can be done by creating 100 variable individually but, this process is rather tedious and impracticable. These type of problem can be handled in C programming using arrays.
- An array is a sequence of data item of homogeneous value(same type).
- All the data items of an array  are stored in consecutive memory locations in RAM.
- The elements of an array are of same data type and each item can be accessed using the same name.
- 6

### Slide 7
- TYPES OF ARRAYS
- Array is of three types:
- 7

### Slide 8
- Declaration of 1-D Array
- Declaration of one-dimensional array:
- We know that all the variables are declared before they are used in the program. Similarly, an array must be declared before it is used.
- During declaration, the size of the array has to be specified. The size used during declaration of the array informs the compiler to allocate and reserve the specified memory locations.
- data_type
- array_name
- [
- array_size
- ];
- For example:
- int age[5];
- Here, the name of array is age. The size of array is 5,i.e., there are 5 items(elements) of array age. All element in an array are of the same type (int, in this case).
- 8

### Slide 9
- Array Elements
- Each element of array can be accessed and used by user according to the need of program
- .
- For example:
- int age[5];
- Note that, the first element is numbered 0 and so  on.
- Here, the size of array age is 5 times the size of int because there are 5 elements.
- Suppose, the starting address of age[0] is 2120d and the size of int be 4 bytes. Then, the next address (address of a[1]) will be 2124d, address of a[2] will be2128d and so on.
- 9

### Slide 10
- Initialization of 1-D Array
- Initialization of one-dimensional array
- :
- Arrays can be initialized at declaration time in  this source code as:
- int age[5]={2,4,34,3,4};
- It is not necessary to define the size of arrays during initialization.
- int age[]={2,4,34,3,4};
- In this case, the compiler determines the size of array by calculating the number of elements of an array
- 10

### Slide 11
- Example of 1-D Array
- Program to take 5 values from the user and store them in an array.
- #include<stdio.h>
- printf
- ("Displaying integers: ");
- int main()  {                                                               for(int
- i
- = 0;
- i
- < 5; ++
- i
- )
- int values[5];                                                                  {
- printf
- ("Enter 5 integers: ");
- printf
- ("%d\n", values[
- i
- ]);
- for(int
- i
- = 0;
- i
- < 5; ++
- i
- )                                                   }
- {                                                                              return 0;
- scanf
- ("%d", &values[
- i
- ]);                                              }
- }
- 11
- Here, we have used a for loop to take 5 inputs from the user and store them in an array. Then, using another for loop, these elements are displayed on the screen

### Slide 12
- Example of 1-D Array
- Program to find the average of n numbers using arrays
- #include<stdio.h>                                                    average = sum/n;
- int main()  {
- printf
- ("Average = %d", average);
- int marks[10],
- i
- , n, sum = 0, average                       }
- printf
- ("Enter number of elements: ");                             return 0;
- scanf
- ("%d", &n);     for(
- i
- =0;
- i
- <n; ++
- i
- )                                      }
- {
- printf
- ("Enter
- number%d
- : ",i+1);
- scanf
- ("%d", &marks[
- i
- ]);
- sum += marks[
- i
- ];
- }
- 12
- Here, we have computed the average of n numbers entered by the user.

### Slide 13
- Summary
- Array is defined as an  ordered set of similar data items
- During declaration of an array
- the size of the array has to be  specified.
- Arrays can be initialized at declaration time in  this source code
- 13

### Slide 14
- Next Lecture
- A 2-D array stores data in rows and columns.
- It is also called a matrix array.
- Used to represent tabular data.
- Declared using two dimensions.
- Elements are accessed using row and column indices.
- Memory is allocated in contiguous locations.
- Commonly used in matrix operations and tables.

### Slide 15
- Quiz
- A one-dimensional array stores:
- a) Characters only
- b) Different data types
- c) Elements of same data type
- d) Floating values only
- Answer:
- C
- What is the last index of an array of size 5?
- a) 5
- b) 4
- c) 0
- d) 6
- Answer:
- B
- What is the index of the first element in an array?
- a) 1
- b) 0
- c) -1
- d) Depends on compiler
- Answer:
- B
- Arrays are stored in:
- a) Random memory locations
- b) Contiguous memory locations
- c) Stack only
- d) Heap only
- Answer:
- B

### Slide 16
- FREQUENTLY ASKED QUESTIONS
- Write a C Program to  Addition of All Elements of the Array
- Write a C Program to insert an element in an array.
- Write a C Find Smallest Element in Array .
- Write a C program to reversing an element in an array.
- C program to find the sum and calculate percentage of marks of n students using arrays
- 16

### Slide 17
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- 1.What is the right way to initialize an array?
- A.int num[6] = { 2, 4, 12, 5, 45, 5 };
- B.int n{} = { 2, 4, 12, 5, 45, 5 };
- C.int n{6} = { 2, 4, 12 };
- D.int n(6) = { 2, 4, 12, 5, 45, 5 };
- 2.  An array element is always stored in …………………..memory location?
- A. Sequential
- B. Random
- C. Sequential and Random
- D. None of the above
- 17

### Slide 18
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- 3. Size of an array need not be specified, when
- A. Initialization is a part of definition
- B. It is a
- declaratrion
- C. It is a formal parameter
- D. All of these
- 18

### Slide 19
- REFERENCES
- Video Lectures
- https://www.youtube.com/watch?v=XZGZm-0wUC0
- Websites:
- https://www.cs.swarthmore.edu/~newhall/unixhelp/C_arrays.html
- https://study.com/academy/lesson/declaring-one-dimensional-arrays-definition-example.html
- 19

### Slide 20
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 21
- Class-wise feedback

### Slide 22
- THANK YOU


## PPT 5 2D Array
### Slide 1
- INSTITUTE - UIE
- DEPARTMENT- ACADEMIC UNITS
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.   2                           Chapter No.   2                                        Lecture No.2
- Topic : Loops
- Faculty Name-Dr. Sheenam
- E_Code
- - E6717
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
- 4
- Recap of Previous Lecture
- A 1-D array stores multiple elements of the same data type.
- Elements are stored in contiguous memory locations.
- Array indexing starts from 0 in C.
- Arrays are declared using square brackets [ ].
- Elements are accessed using index values.
- Loops are commonly used to traverse arrays.
- 1-D arrays simplify handling large amounts of similar data.

### Slide 5
- Content
- Two-Dimensional Array
- Initialization of Two-Dimensional Array
- Memory Representation of 2D Array
- Examples
- References
- 5

### Slide 6
- 2-Dimensional Array
- A two-dimensional array is an array where its elements are selected (identified) using two indices. In 2-D array, to declare and access elements of a 2-D array we use 2 subscripts instead of 1.
- Syntax:
- data_type
- array_name
- [ROW][COL];
- The total number of elements in a 2-D array is ROW*COL.
- Example:
- int a[m][n];
- In rectangular 2-dimensional arrays, m number of rows and n number of columns in the array has the same number of array elements.
- 6
- A conceptual representation of 2D array

### Slide 7
- Initialization of 2-D Array
- Initialization of 2-D array is similar to a 1-D array.
- Example:
- 7
- After this initialization, each element is as follows:
- temp[0][0] : 1
- temp[0][1] : 2
- temp[0][2] : 3
- temp[1][0] : 11
- temp[1][1] : 22
- temp[1][2] : 33

### Slide 8
- Memory Representation 2-D Array
- The compiler will allocate the memory for two dimensional array
- row-wise
- meaning the first element of the second row will be placed after the last element of the first row.
- 8

### Slide 9
- Memory Representation 2-D Array
- And if we assume that the first element of the array is at address 1000 and the size of type
- int
- is 2 bytes then the elements of the array will get the following allocated memory locations
- .
- 9

### Slide 10
- Example of 2-D Array
- Program to store the elements from the user and store them in an 2D array.
- #include<stdio.h>
- int main()
- {
- int
- disp
- [2][3],
- i
- , j;
- for(
- i
- =0;
- i
- <2;
- i
- ++)
- {
- for(j=0;j<3;j++)
- {
- printf
- ("Enter value for
- disp
- [%d][%d]:",
- i
- , j);
- scanf
- ("%d", &
- disp
- [
- i
- ][j]);
- }
- }
- 10
- printf
- ("Two Dimensional array elements:\n");
- for(
- i
- =0;
- i
- <2;
- i
- ++)
- {
- for(j=0;j<3;j++)
- {
- printf
- ("%d ",
- disp
- [
- i
- ][j]);
- if(j==2){
- printf
- ("\n");
- }
- }
- }
- return 0;
- }

### Slide 11
- Example of 2-D Array
- Program to sum of even and odd of 2D array.
- #include<stdio.h>
- int main()
- {
- int
- i
- =0,j=0;
- int
- arr
- [3][4]={{1,2,3,4},{2,3,4,5},{3,4,5,6}};
- int even=0;int odd=0;
- for(
- i
- =0;i<3;i++)
- {
- for(j=0;j<4;j++)
- {
- if(
- arr
- [
- i
- ][j]%2==0)
- {
- 11
- even=
- even+arr
- [
- i
- ][j];
- }
- else
- {
- odd=
- odd+arr
- [
- i
- ][j];
- }
- }
- }
- printf
- ("Sum of even =%d \
- n",even
- );
- printf
- ("Sum of odd =%
- d",odd
- );
- return 0;
- }

### Slide 12
- Summary
- In 2-D array, to declare and access elements of a 2-D array we use 2 subscripts instead of 1.
- In rectangular 2-dimensional arrays, m number of rows and n number of columns in the array has the same number of array elements.
- The compiler will allocate the memory for two dimensional array
- row-wise
- meaning the first element of the second row will be placed after the last element of the first row.
- 12

### Slide 13
- Next Lecture
- A string is a collection of characters enclosed in double quotes.
- In C, strings are stored in character arrays.
- A string always ends with a special character '\0' (null character).
- Strings are used to store names, words, and sentences.

### Slide 14
- Quiz
- Which loop structure is suitable for 2-D arrays?
- a) Single for loop
- b) if-else
- c) Nested loops
- d) switch
- Answer:
- C
- 3
- .
- Which operator is used to access elements in a 2-D array?
- a) {}
- b) ()
- c) [][]
- d) <>
- Answer. C
- 4
- . 2-D arrays are commonly used for:
- a) Storing text only
- b) Matrix operations
- c) Function calls
- d) Pointer arithmetic only
- Answer: b) Matrix operations
- 1.
- A two-dimensional array is also called a:
- A) Linear array
- B) Matrix
- C) Pointer
- D) Function
- Answer.B

### Slide 15
- FREQUENTLY ASKED QUESTIONS
- Write a C Program to  addition of two matrices.
- Write a program in C to calculate determinant of a 3 x 3 matrix.
- Write a program in C to accept two matrices and check whether they are equal.
- Write a C program to transpose of two matrices.
- Program to multiply two matrices.
- 15

### Slide 16
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- 1.Which of the following is true about arrays in C.
- (A)
- For every type T, there can be an array of T.
- (B)
- For every type T except void and function type, there can be an array of T.
- (C)
- When an array is passed to a function, C compiler creates a copy of array.
- (D)
- 2D arrays are stored in column major form
- 2. What will be the output of the following C code?
- #include <
- stdio.h
- >
- void f(int a[][3])
- {
- a[0][1] = 3;
- int
- i
- = 0, j = 0;
- for (
- i
- = 0;
- i
- < 2;
- i
- ++)
- 16
- for (j = 0; j < 3;
- j++
- )
- printf
- ("%d", a[
- i
- ][j]);
- }
- void main()
- {
- int a[2][3] = {0};
- f(a);
- }
- a) 0 3 0 0 0 0
- b) Junk 3 junk
- junk
- junk
- junk
- c) Compile time error
- d) All junk values

### Slide 17
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- 3What will be the output of the following C code?
- #include <
- stdio.h
- >
- void main()
- {
- int a[2][3] = {1, 2, 3, 4, 5};
- int
- i
- = 0, j = 0;
- for (
- i
- = 0;
- i
- < 2;
- i
- ++)
- for (j = 0; j < 3;
- j++
- )
- printf
- ("%d", a[
- i
- ][j]);
- }
- 17
- a) 1 2 3 4 5 0
- b) 1 2 3 4 5 junk
- c) 1 2 3 4 5 5
- d) Run time error

### Slide 18
- Books Recommended
- Programming in C by Reema Thareja.
- Programming in ANSI C by E.
- Balaguruswamy
- , Tata McGraw Hill.
- Programming with C (Schaum's Outline Series) by Byron Gottfried  Jitender Chhabra, Tata McGraw Hill.
- The C Programming Language by Brian W. Kernighan, Dennis Ritchie, Pearson education.

### Slide 19
- REFERENCES
- Video Lectures
- https://www.youtube.com/watch?v=KDQXUysHLL8
- Websites:
- https://beginnersbook.com/2014/01/2d-arrays-in-c-example/
- https://processing.org/tutorials/2darray/
- https://www.programiz.com/c-programming/c-multi-dimensional-arrays
- 19

### Slide 20
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 21
- Class-wise feedback

### Slide 22
- THANK YOU


## PPT 6 String
### Slide 1
- INSTITUTE - UIE
- DEPARTMENT- ACADEMIC UNITS
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.   2                           Chapter No.   2                                        Lecture No.3
- Topic : Loops
- Faculty Name-Dr. Sheenam
- E_Code
- - E6717
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
- 4
- Recap of Previous Lecture
- A 2-D array is an array of arrays used to store data in rows and columns.
- It is useful for representing matrices and tables.
- Declaration syntax:
- data_type
- array_name
- [row][column];
- Elements are accessed using row and column indices.
- Indexing starts from 0 in C programming.
- Memory is allocated in contiguous locations.

### Slide 5
- String Definition
- Initialization of string
- Memory Representation of String
- String I/O functions
- Examples
- References
- 5
- CONTENTS

### Slide 6
- STRING
- A string in C is simply an array of characters ended with null character (‘\0’) This null character indicates the end of the string.
- Strings are always enclosed by double quotes. Whereas, character is enclosed by single   quotes in C.
- Initialization of STRING:
- char string[10] = {‘h’, ’e’, ‘l’, ‘l’, ‘o’, ‘\0’};
- (or)
- char string[10] = “Hello”;
- (or)
- char string []    = “Hello”;
- Difference between above declarations are, when we declare char as “string[10]”, 10 bytes of memory space is allocated for holding the string value. When we declare char as “string[]”, memory space will be allocated as per the requirement during execution of the program.
- 6

### Slide 7
- Memory Representation in Strings
- Let’s take an example for Memory representation of string:
- char string[10]=”Hello”
- 7
- If you do not place null character at the end of string, the C compiler automatically places the '\0' at the end of the string when it initializes the array.

### Slide 8
- Memory Representation in Strings
- #include <
- stdio.h
- >
- int main ()
- {
- char string[10] = {'H', 'e', 'l', 'l', 'o', '\0'};
- printf
- ("Message is: %s\n", string);
- return 0;
- }
- 8

### Slide 9
- String Input And Output Functions
- Input function
- scanf
- () can be used with
- %s
- format specifier to read a string input from the terminal. But there is one problem with
- scanf
- () function, it terminates its input on the first  white space it encounters. Therefore if you try to read an input string "Hello World“ using
- scanf
- () function, it will only read
- Hello
- and terminate after encountering white spaces.
- 9

### Slide 10
- How to read a line of text
- You can use the gets() function to read a line of string. And, you can use puts() to display the string.
- Example1 : gets() and puts()
- #include <
- stdio.h
- >
- int main()
- {
- char name[30];
- printf
- ("Enter name: ");
- gets(name,
- sizeof
- (name), stdin);  // read string
- printf
- ("Name: ");
- puts(name);    // display string
- return 0;
- }
- 10

### Slide 11
- Example of String
- Example2: Concatenate Two Strings
- #include <
- stdio.h
- >
- int main()
- {
- char s1[100] = "programming ", s2[] = "is awesome";
- int length, j;   // store length of s1 in the length variable length = 0;
- while (s1[length] != '\0')
- {
- ++length;
- }   // concatenate s2 to s1
- for (j = 0; s2[j] != '\0'; ++j, ++length)
- {
- s1[length] = s2[j];
- }   // terminating the s1 string
- s1[length] = '\0';
- printf
- ("After concatenation: ");
- puts(s1);
- return 0;
- }
- 11
- Here, two strings s1 and s2 and concatenated and the result is stored in s1.
- It's important to note that the length of s1 should be sufficient to hold the string after concatenation.

### Slide 12
- SUMMARY
- A string in C is simply an array of characters ended with null character (‘\0’) This null character indicates the end of the string.
- Strings are always enclosed by double quotes. Whereas, character is enclosed by single   quotes in C.
- Use gets and puts functions for input  a string
- 12

### Slide 13
- Next Lecture
- A function is a block of code designed to perform a specific task.
- Functions help in dividing a program into smaller and manageable parts.
- They improve program readability and reusability.
- A function can be called multiple times in a program.
- Functions reduce code repetition and complexity.
- Every C program contains a main
- function (main()).
- Functions may accept input values called parameters or arguments.
- A function can return a value to the calling program.
- Functions are classified as library functions and user-defined functions.

### Slide 14
- Quiz
- A string in C is stored as:
- a) Integer array
- b) Float array
- c) Character array
- d) Structure
- Answer:
- C
- 3
- .
- Which symbol is used to terminate a
- string?a
- )\t
- b)\n
- c)\0
- d)\b
- Answer. C
- What is the index of first character in a string?
- a)
- 0
- b)1
- c)-1
- d2
- Answer:
- A
- 4.Which function is commonly used to read a string with spaces?
- a)
- scanf
- ()
- b)
- printf
- ()
- c) gets()
- d)
- putchar
- ()
- Answer. C

### Slide 15
- FREQUENTLY ASKED QUESTIONS
- PROGRAMS
- Q1 Write a C program to count no of lines, words and characters in a given text.
- Q2 C program to print all VOWEL and CONSONANT characters separately
- Q3
- C program to count upper case, lower case and special characters in a string.
- Q4
- C program to print following pattern.
- H
- He
- Hel
- Hell
- Hello
- 15

### Slide 16
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- 1.
- 1
- What is the Format specifier used to print a String or Character array in C
- Printf
- or
- Scanf
- function.?
- A) %c
- B) %C
- C) %s
- D) %w
- 16
- 2.
- What is the output of C Program with Strings.?
- int main()
- {
- char
- ary
- []="Discovery Channel";
- printf
- ("%s",
- ary
- );
- return 0;
- }
- A) D
- B) Discovery Channel
- C) Discovery
- D) Compiler error

### Slide 17
- UTILIZE YOUR KNOWLEDGE TO ANSWER
- 3
- What is the output of C Program with Strings.?
- {
- char str[]={'
- g','l','o','b','e
- '};
- printf
- ("%
- s",str
- );
- return 0;
- }
- A) g
- B) globe
- C) globe\0
- D) None of the above
- 17
- 4. What is the output of C Program.?
- int main()
- { int str[]={'
- g','l','o','b','y
- '};
- printf
- ("
- A%c
- ",str);
- printf
- ("A%s ",str);
- printf
- ("
- A%c
- ",str[0]);
- return 0;
- }
- A) A
- A
- A
- B) A Ag
- Ag
- C) A*
- randomchar
- * Ag
- Ag
- D) Compiler error

### Slide 18
- REFERENCES
- Video Lectures
- https://www.youtube.com/watch?v=_3CmPbInJJs
- Websites:
- https://www.tutorialspoint.com/objective_c/objective_c_strings.htm
- https://www.programiz.com/c-programming/c-strings
- 18

### Slide 19
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 20
- Class-wise feedback
- 20

### Slide 21
- THANK YOU


---
