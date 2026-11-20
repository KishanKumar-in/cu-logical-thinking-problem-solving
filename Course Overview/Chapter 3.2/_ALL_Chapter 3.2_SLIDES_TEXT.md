# Chapter 3.2 - All Lecture Slides Text


## Chapter 8 Structure Part 1
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
- Space for visual (size 24)
- Introduction to Structure
- How to access structure members
- 3
- Syllabus/Topics To be Covered

### Slide 4
- Recap of Previous Lecture
- • Pointers are variables that store memory addresses.
- • The address-of operator (&) is used to obtain an address.
- • The dereference operator (*) is used to access the value at an address.
- • Pointers can be used with arrays and functions.
- • Pointer arithmetic enables efficient memory traversal.
- • Pointers improve program efficiency and flexibility.

### Slide 5
- 5
- Structure
- is a user-defined datatype in C language which allows us to combine data of different types together.
- Structure
- helps to construct a complex data type which is more meaningful.
- It is somewhat similar to an Array, but an array holds data of similar type only. But structure on the other hand, can store data of any type, which is practical more useful.
- For example
- : If I have to write a program to store Student information, which will have Student's name, age, branch, permanent address, father's name etc, which included string values, integer values etc, how can I use arrays for this problem, I will require something which can hold data of different types together. In structure, data is stored in form of records.
- Introduction

### Slide 6
- Defining a Structure
- struct
- keyword is used to define a structure. struct defines a new data type which is a collection of primary and derived datatypes.
- Syntax
- :
- struct [
- structure_tag
- ]
- {
- //member variable 1
- //member variable 2
- ...
- }[
- structure_variables
- ];
- Note
- : The closing curly brace in the structure type declaration must be followed by a semicolon(;).
- 6

### Slide 7
- Example:
- struct Student
- {
- char name[25];
- int age;
- char branch[10];
- // F for female and M for male
- char gender;
- };
- Here struct Student declares a structure to hold the details of a student which consists of 4 data fields, namely name, age, branch and gender. These fields are called structure elements or members.
- Each member can have different datatype, like in this case, name is an array of char type and age is of int type etc. Student is the name of the structure and is called as the structure tag.
- 7

### Slide 8
- Declaring Structure Variables
- It is possible to declare variables of a structure, either along with structure definition or after the structure is defined.
- Structure variable declaration is similar to the declaration of any normal variable of any other datatype.
- Structure variables can be declared in following two ways:
- Declaring Structure variables separately
- Declaring Structure variables with structure definition
- 8

### Slide 9
- Declaring Structure variables separately
- struct Student
- {
- char name[25];
- int age;
- char branch[10];
- //F for female and M for male
- char gender;
- };
- struct Student S1, S2;      //declaring variables of struct Student
- 9

### Slide 10
- Declaring Structure variables with structure definition
- struct Student
- {
- char name[25];
- int age;
- char branch[10];
- //F for female and M for male
- char gender;
- }S1, S2;
- Here S1 and S2 are variables of structure Student.
- 10

### Slide 11
- Initializing structure members
- Structure members cannot be initialized with declaration. For example the following C program fails in compilation.
- struct Point
- {
- int x = 0;  // COMPILER ERROR:  cannot initialize members here
- int y = 0;  // COMPILER ERROR:  cannot initialize members here
- };
- The reason for above error is simple, when a datatype is declared, no memory is allocated for it. Memory is allocated only when variables are created.
- 11

### Slide 12
- Structure members can be initialized using curly braces ‘{}’. For example, following is a valid initialization.
- struct Point
- {
- int x, y;
- };
- int main()
- {
- // A valid initialization. member x gets value 0 and y
- // gets value 1.  The order of declaration is followed.
- struct Point p1 = {0, 1};
- }
- 12

### Slide 13
- Computing Size of Structure without
- sizeof
- ()
- We can calculate the size of structure using pointers. Below is the implementation.
- #include<stdio.h>
- struct
- MySize
- {
- int a;
- int b;
- };
- int main()
- {
- struct
- MySize
- *
- Msz
- =0;
- int size = ((char*)(Msz+1))-((char *)(
- Msz
- ));
- printf
- ("\n Structure Size :[%d]", size);
- return 0;
- }
- Output:
- Structure Size :[8]
- 13

### Slide 14
- Structure
- Padding
- The
- sizeof
- for a struct is not always equal to the sum of
- sizeof
- of each individual member.
- This is because of the padding added by the compiler to avoid alignment issues.
- Padding is only added when a structure member is followed by a member with a larger size or at the end of the structure.
- Different compilers might have different alignment constraints as C standards state that alignment of structure totally depends on the implementation.
- 14

### Slide 15
- Let’s take a look at the following examples for better understanding:
- Case 1:
- // C program to illustrate
- // size of struct
- #include <
- stdio.h
- >
- int main()
- {
- struct A {
- //
- sizeof
- (int) = 4
- int x;
- // Padding of 4 bytes
- //
- sizeof
- (double) = 8
- double z;
- //
- sizeof
- (short int) = 2
- short int y;
- // Padding of 6 bytes
- };
- printf
- ("Size of struct: %
- ld
- ",
- sizeof
- (struct A));
- return 0;
- }
- Output:
- Size of struct: 24
- 15
- The red portion represents the padding added for data alignment and the green portion represents the struct members. In this case, x (int) is followed by z (double), which is larger in size as compared to x. Hence padding is added after x. Also, padding is needed at the end for data alignment.

### Slide 16
- Case 2:
- // C program to illustrate
- // size of struct
- #include <
- stdio.h
- >
- int main()
- {
- struct B {
- //
- sizeof
- (double) = 8
- double z;
- //
- sizeof
- (int) = 4
- int x;
- //
- sizeof
- (short int) = 2
- short int y;
- // Padding of 2 bytes
- };
- printf
- ("Size of struct: %
- ld
- ",
- sizeof
- (struct B));
- return 0;
- }
- Output:
- Size of struct: 16
- 16
- In this case, the members of the structure are sorted in decreasing order of their sizes. Hence padding is required only at the end.

### Slide 17
- Case 3:
- // C program to illustrate
- // size of struct
- #include <stdio.h>
- int main()
- {
- struct C {
- // sizeof(double) = 8
- double z;
- // sizeof(short int) = 2
- short int y;
- // Padding of 2 bytes
- // sizeof(int) = 4
- int x;
- };
- printf("Size of struct: %ld", sizeof(struct C));
- return 0;
- }
- Output:
- Size of struct: 16
- 17
- In this case, y (short int) is followed by x (int) and hence padding is required after y. No padding is needed at the end in this case for data alignment.
- C language doesn’t allow the compilers to reorder the struct members to reduce the amount of padding. In order to minimize the amount of padding, the struct members must be sorted in a descending order (similar to the case 2).

### Slide 18
- Accessing Structure Members
- Structure members can be accessed and assigned values in a number of ways.
- Structure members have no meaning individually without the structure.
- There are two types of operators used for accessing members of a structure.
- .  Member operator
- -> -Structure pointer operator
- 18

### Slide 19
- Example:
- #include<stdio.h>
- struct Point
- {
- int x, y;
- };
- int main()
- {
- struct Point p1 = {0, 1};
- // Accessing members of point p1
- p1.x = 20;
- printf
- ("x = %d, y = %d", p1.x, p1.y);
- return 0;
- }
- Output:
- x = 20, y = 1
- 19
- Accessing Structure Members by Dot Operator

### Slide 20
- Example:
- #include<stdio.h>
- struct Point
- {
- int x, y;
- };
- int main()
- {
- struct Point p1 = {1, 2};
- // p2 is a pointer to structure p1
- struct Point *p2 = &p1;
- // Accessing structure members using structure pointer
- printf
- ("%d %d", p2->x, p2->y);
- return 0;
- }
- Output:
- 1 2
- 20
- Accessing Structure Members by Structure pointer operator

### Slide 21
- Union
- Like Structures, union is a user defined data type.
- In union, all members share the same memory location.
- 21

### Slide 22
- For example, In
- the following C program, both x and y share the same location. If we change x, we can see the changes being reflected in y.
- #include <
- stdio.h
- >
- // Declaration of union is same as structures
- union test {
- int x, y;
- };
- int main()
- {
- // A union variable t
- union test t;
- t.x
- = 2; //
- t.y
- also gets value 2
- printf
- ("After making x = 2:\n x = %d, y = %d\n\n",
- t.x
- ,
- t.y
- );
- t.y
- = 10; //
- t.x
- is also updated to 10
- printf
- ("After making y = 10:\n x = %d, y = %d\n\n",
- t.x
- ,
- t.y
- );
- return 0;
- }
- 22

### Slide 23
- Output:
- After making x = 2:
- x = 2, y = 2
- After making y = 10:
- x = 10, y = 10
- To access any member of a union, we use the
- member access operator (.)
- .
- The member access operator is coded as a period between the union variable name and the union member that we wish to access.
- 23

### Slide 24
- Structure Vs Union
- 24

### Slide 25
- Uses of C Structure
- C Structures can be used to store huge data. Structures act as a database.
- C Structures can be used to send data to the printer.
- C Structures can interact with keyboard and mouse to store the data.
- C Structures can be used in drawing and floppy formatting.
- C Structures can be used to clear output screen contents.
- C Structures can be used to check computer’s memory size etc.
- 25

### Slide 26
- 26
- Summary

### Slide 27
- Next Lecture
- • Introduction to Nested Structures
- • Defining a Structure within Another Structure
- • Accessing Members of Nested Structures
- • Initialization of Nested Structures
- • Real-World Applications of Nested Structures
- • Programs Using Nested Structures

### Slide 28
- Frequently Asked question
- Q1
- What will be the output of the C program?
- #include<stdio.h>
- int main()
- {
- struct leader
- {
- char *lead;
- int born;
- };
- struct leader l1 = {"
- AbdulKalam
- ", 1931};
- struct leader l2 = l1;
- printf
- ("%s %d", l2.lead, l1.born);
- Ans:
- AbdulKalam
- 1931
- 28

### Slide 29
- Q2. What will be the output of the C program?
- void main()
- {
- struct bitfields {
- int bits_1: 2;
- int bits_2: 9;
- int bits_3: 6;
- int bits_4: 1;
- }bit;
- printf
- ("%d",
- sizeof
- (bit));
- }
- Ans:
- 3
- Q3.
- What are the similarities between structure and union?
- Ans:
- Both are user-defined data types used to store data of different types as a single unit. Their members can be objects of any type, including other structures and unions or arrays. A member can also consist of a bit field. Both structures and unions support only assignment = and
- sizeof
- operators. The two structures or unions in the assignment must have the same members and member types.
- A structure or a union can be passed by value to functions and returned by value by functions. The argument must have the same type as the function parameter. A structure or union is passed by value just like a scalar variable as a corresponding parameter.
- ‘.’ operator is used for accessing members.
- 29

### Slide 30
- Q4.
- Write a program to Store Information in Structure and Display it?
- 30
- #include <
- stdio.h
- >
- struct student {
- char
- firstName
- [50];
- int roll;
- float marks;
- } s[10];
- int main() {
- int
- i
- ;
- printf
- ("Enter information of students:\n");
- // storing information
- for (
- i
- = 0;
- i
- < 5; ++
- i
- ) {
- s[
- i
- ].roll =
- i
- + 1;
- printf
- ("\
- nFor
- roll
- number%d
- ,\n", s[
- i
- ].roll);
- printf
- ("Enter first name: ");
- scanf
- ("%s", s[
- i
- ].
- firstName
- );
- printf
- ("Enter marks: ");
- scanf
- ("%f", &s[
- i
- ].marks);
- }
- printf
- ("Displaying Information:\n\n");
- // displaying information
- for (
- i
- = 0;
- i
- < 5; ++
- i
- ) {
- printf
- ("\
- nRoll
- number: %d\n",
- i
- + 1);
- printf
- ("First name: ");
- puts(s[
- i
- ].
- firstName
- );
- printf
- ("Marks: %.1f", s[
- i
- ].marks);
- printf
- ("\n");
- }
- return 0;
- }

### Slide 31
- 31
- Output:

### Slide 32
- Assessment Questions
- :
- 32
- 1.
- What is the output?
- #include <
- stdio.h
- >
- int main()
- {
- struct
- xyz
- {
- int a;
- };
- struct
- xyz
- obj1={1};
- struct
- xyz
- obj2 = obj1;
- printf
- ("%d", obj2.a);
- obj2.a = 100;
- printf
- ("%d", obj1.a);
- return 0;
- }

### Slide 33
- 33
- 2.
- What will be the output of the C program?
- #include<stdio.h>
- int main()
- {
- struct
- simp
- {
- int
- i
- = 6;
- char city[] = "
- chennai
- ";
- };
- struct
- simp
- s1;
- printf
- ("%d",s1.city);
- printf
- ("%d", s1.i);
- return 0;
- 3.
- Which of the following is a properly defined struct?
- A. struct {int a;}
- B. struct
- a_struct
- {int a;}
- C. struct
- a_struct
- int a;
- D. struct
- a_struct
- {int a;};

### Slide 34
- 4. What will be the output of the program?
- #include <
- stdio.h
- >
- struct
- cppbuzz
- {
- };
- int main()
- {
- printf
- ("%d",
- sizeof
- (struct
- cppbuzz
- ));
- return 0;
- }
- 34

### Slide 35
- Discussion forum
- .
- Watch this video to know more about how structures are stored in memory and what is meant by structure padding.
- 35
- https://www.youtube.com/watch?v=aROgtACPjjg

### Slide 36
- REFERENCES
- Reference Books
- Programming in C by Reema
- Thareja
- .
- Programming in ANSI C by E.
- Balaguruswamy
- , Tata McGraw Hill.
- Programming with C (
- Schaum's
- Outline Series) by Byron Gottfried  Jitender Chhabra, Tata McGraw Hill.
- The C Programming Language by Brian W. Kernighan, Dennis Ritchie, Pearson education.
- Websites:
- https://www.studytonight.com/c/structures-in-c.php
- https://www.tutorialspoint.com/cprogramming/c_structures.htm
- https://www.geeksforgeeks.org/union-c/
- YouTube Links:
- https://www.youtube.com/watch?v=Ranc3VvjI88
- https://www.youtube.com/watch?v
- =zdUhS4YSWHg
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


## Chapter 8 Structure Part 2
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor
- of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:25CSH-107
- Academic Session 2025-26
- ODD Semester Jul-Dec 2025
- Unit No.   3                         Chapter No.   2                                        Lecture No.5
- Topic : Hands on session on Flowcharts
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
- Recap of Previous Lecture
- • Structures are user-defined data types in C.
- • Used to group related data of different data types.
- • Structure members are accessed using the dot (.) operator.
- • Structures can be initialized during declaration.
- • Arrays and nested structures can be created using structures.
- • Structures help represent real-world entities efficiently.

### Slide 5
- Space for visual (size 24)
- Nested Structure
- 5
- Syllabus/Topics To be Covered

### Slide 6
- 6
- C provides us the feature of nesting one structure within another structure by using which, complex data types are created.
- For example, we may need to store the address of an entity employee in a structure.
- The attribute address may also have the subparts as street number, city, state, and pin code.
- Hence, to store the address of the employee, we need to store the address of the employee into a separate structure and nest the structure address into the structure employee.
- Example:
- #include<stdio.h>
- struct address
- {
- char city[20];
- int pin;
- char phone[14];
- };
- Nested Structure

### Slide 7
- struct employee
- {
- char name[20];
- struct address add;
- };
- void main ()
- {
- struct employee emp;
- printf
- ("Enter employee information?\n");
- scanf
- ("%s %s %d %s",
- emp.name,emp.add.city
- , &
- emp.add.pin
- ,
- emp.add.phone
- );
- printf
- ("Printing the employee information....\n");
- printf
- ("name: %s\
- nCity
- : %s\
- nPincode
- : %d\
- nPhone
- :%s“,
- emp.name,emp.add.city
- ,
- emp.add.pin
- ,
- emp.add.phone
- );
- }
- 7

### Slide 8
- Output:
- Enter employee information?
- Arun
- Delhi
- 110001
- 1234567890
- Printing the employee information....
- name: Arun
- City: Delhi
- Pincode
- : 110001
- Phone: 1234567890
- 8

### Slide 9
- Ways of Nesting a Structure
- The structure can be nested in the following ways:
- By separate structure
- By Embedded structure
- 9

### Slide 10
- Nesting a Structure by Separate Structure
- Here, we create two structures, but the dependent structure should be used inside the main structure as a member. Consider the following example.
- struct Date
- {
- int dd;
- int mm;
- int
- yyyy
- ;
- };
- struct Employee
- {
- int id;
- char name[20];
- struct Date
- doj
- ;
- }emp1;
- As you can see,
- doj
- (date of joining) is the variable of type Date. Here
- doj
- is used as a member in Employee structure. In this way, we can use Date structure in many structures.
- 10

### Slide 11
- Nesting a Structure by Embedded structure
- The embedded structure enables us to declare the structure inside the structure. Hence, it requires less line of codes but it can not be used in multiple data structures. Consider the following example.
- struct Employee
- {
- int id;
- char name[20];
- struct Date
- {
- int dd;
- int mm;
- int
- yyyy
- ;
- }
- doj
- ;
- }emp1;
- 11

### Slide 12
- Accessing Nested Structure
- We can access the member of the nested structure by
- Outer_Structure.Nested_Structure.member
- as given below:
- e1.doj.dd
- e1.doj.mm
- e1.doj.yyyy
- 12

### Slide 13
- Nesting Structure Example
- #include <
- stdio.h
- >
- #include <
- string.h
- >
- struct
- Employee
- {
- int
- id;
- char
- name[20];
- struct
- Date
- {
- int
- dd;
- int
- mm;
- int
- yyyy
- ;
- }
- doj
- ;
- }e1;
- int
- main( )
- {
- //storing employee information
- e1.id=101;
- strcpy
- (e1.name, "
- Sonoo
- Jaiswal
- e1.doj.dd=10;
- e1.doj.mm=11;
- e1.doj.yyyy=2014;
- //printing first employee information
- printf
- ( "employee id : %d\n", e1.id);
- printf
- ( "employee name : %s\n", e1.name);
- printf
- ( "employee date of joining (dd/mm/
- yyyy
- ) : %d/%d/%d\n", e1.doj.dd,e1.doj.mm,e1.doj.yyyy);
- return
- 0;
- }
- 13

### Slide 14
- Output:
- employee id : 101
- employee name :
- Sonoo
- Jaiswal
- employee date of joining (dd/mm/
- yyyy
- ) : 10/11/2014
- 14

### Slide 15
- Array of Structures
- Declaring an array of structure is same as declaring an array of fundamental types.
- Since an array is a collection of elements of the same type.
- In an array of structures, each element of an array is of the structure type.
- Let's take an example:
- struct car
- {
- char make[20];
- char model[30];
- int year;
- };
- 15

### Slide 16
- Declaratio
- n of
- Array of Structures
- Example: struct car
- arr_car
- [10];
- Here
- arr_car
- is an array of 10 elements where each element is of type struct car.
- We can use
- arr_car
- to store 10 structure variables of type struct car.
- To access individual elements we will use subscript notation ([]) and to access the members of each element we will use dot (.) operator as usual.
- 16

### Slide 17
- arr_stu
- [0] : points to the 0th element of the array.
- arr_stu
- [1] : points to the 1st element of the array.
- arr_stu
- [0].name : refers to the name member of the 0th element of the array.
- arr_stu
- [0].
- roll_no
- : refers to the
- roll_no
- member of the 0th element of the array.
- arr_stu
- [0].marks : refers to the marks member of the 0th element of the array.
- Note:
- the precedence of [] array subscript and dot(.) operator is same and they evaluates from left to right. Therefore in the above expression first array subscript([]) is applied followed by dot (.) operator. The array subscript ([]) and dot(.) operator is same and they evaluates from left to right. Therefore in the above expression first [] array subscript is applied followed by dot (.) operator.
- 17

### Slide 18
- Example:
- #include<stdio.h>
- struct Point
- {
- int x, y;
- };
- int main()
- {
- // Create an array of structures
- struct Point
- arr
- [10];
- // Access array members
- arr
- [0].x = 10;
- arr
- [0].y = 20;
- printf
- ("%d %d",
- arr
- [0].x,
- arr
- [0].y);
- return 0;
- }
- Output:
- 10 20
- 18

### Slide 19
- Structure Vs Union
- Sr. No.
- Key
- Structure
- Union
- 1
- Definition
- Structure is the container defined in C to store data variables of different type and also supports for the user defined variables storage.
- On other hand Union is also similar kind of container in C which can also holds the different type of variables along with the user defined variables.
- 2
- Internal implementation
- Structure in C is internally implemented as that there is separate memory location is allotted to each input member
- While in case Union memory is allocated only to one member having largest size among all other input variables and the same location is being get shared among all of these.
- 3
- Syntax
- Syntax of declare a Structure in C is as follow :
- struct
- struct_name
- {
- type element1
- ;
- type element2
- ;
- .
- .
- }
- variable1
- ,
- variable2
- ,
- ...;
- On other syntax of declare a Union in C is as follow:
- union
- u_name
- {
- type element1
- ;
- type element2
- ;
- .
- .
- }
- variable1
- ,
- variable2
- ,
- ...;
- 4
- Size
- As mentioned in definition Structure do not have shared location for its members so size of Structure is equal or greater than the sum of size of all the data members.
- On other hand Union does not have separate location for each of its member so its size or equal to the size of largest member among all data members.
- 5
- Value storage
- As mentioned above in case of Structure there is specific memory location for each input data member and hence it can store multiple values of the different members.
- While in case of Union there is only one shared memory allocation for all input data members so it stores a single value at a time for all members.
- 6
- Initialization
- In Structure multiple members can be can be initializing at same time.
- On other hand in case of Union only the first member can get initialize at a time.
- 19

### Slide 20
- 20
- Summary

### Slide 21
- Next Lecture
- • Passing Structures to Functions
- • Returning Structures from Functions
- • Pointers to Structures
- • Accessing Structure Members Using Arrow (->) Operator
- • Passing Structure Pointers to Functions
- • Practical Programs and Applications

### Slide 22
- Frequently Asked Questions
- Q1
- W
- hat is the meaning of nested structure?
- Ans
- :
- Nested structures as its name suggest in C is kind of defining one structure inside another structure. Any member variables can be defined inside a structure and in turn, that structure can further be moved into another structure. The variables inside a structure can be anything like normal or pointer or anything and can be placed anywhere within the structure
- Q2
- The correct syntax to access the member of the
- ith
- structure in the array of structures is?
- struct temp
- {
- int b;
- }s[50];
- a)
- s.b.
- [
- i
- ];
- b) s.[
- i
- ].b;
- c)
- s.b
- [
- i
- ];
- d) s[
- i
- ].b;
- Ans: d
- 22

### Slide 23
- Q3: What will be the output of the C program?
- void main()
- {
- struct bitfields {
- int bits_1: 2;
- int bits_2: 9;
- int bits_3: 6;
- int bits_4: 1;
- }bit;
- printf
- ("%d",
- sizeof
- (bit));
- }
- A. 2
- B. 3
- C. 4
- D. 0
- Ans:
- Option: B
- Explanation:
- 1 byte = 8 bits
- In the above program we assign 2, 9, 6, 1 for the variables. Sum of the bits assigned is, 2 + 9 + 6 + 1 = 18, It is greater than 2 bytes, so it automatically takes 3 bytes.
- 23

### Slide 24
- Assessment Questions
- :
- 24
- 1. C Program to Calculate Size of Structure using
- Sizeof
- Operator
- 2.  Write a C program to  Sort Two Structures on the basis of any structure element and Display Information
- Program Statement – Define a structure called cricket that will describe the following information
- Player name
- Team name
- Batting average
- Using cricket, declare an array player with 10 elements and write a program to read the information about all the 10 players and print a team wise list containing names of players with their batting average.

### Slide 25
- Discussion forum
- PROBLEM: C Program to sort array of Structure in C Programming
- Write a C program to accept records of the different states using array of structures. The structure should contain char state, population, literacy rate, and income. Display the state whose literacy rate is highest and whose income is highest.
- 25

### Slide 26
- REFERENCES
- Reference Books
- Programming in C by Reema
- Thareja
- .
- Programming in ANSI C by E.
- Balaguruswamy
- , Tata McGraw Hill.
- Programming with C (
- Schaum's
- Outline Series) by Byron Gottfried  Jitender Chhabra, Tata McGraw Hill.
- The C Programming Language by Brian W. Kernighan, Dennis Ritchie, Pearson education.
- Websites:
- https://www.studytonight.com/c/structures-in-c.php
- https://www.tutorialspoint.com/cprogramming/c_structures.htm
- https://www.geeksforgeeks.org/union-c/
- YouTube Links:
- https://www.youtube.com/watch?v=Ranc3VvjI88
- https://www.youtube.com/watch?v
- =zdUhS4YSWHg
- 26

### Slide 27
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 28
- Class-wise
- feedback
- 28

### Slide 29
- THANK YOU


## Chapter 8 Structure Part 3
### Slide 1
- INSTITUTE - UIE
- Department of Engineering  Foundations
- Bachelor of Engineering (Computer Science & Engineering)
- Subject Name: Logical Thinking & Problem Solving
- Code:26CSH-101
- Academic Session 2026-27
- ODD Semester Jul-Dec 2026
- Unit No.   3                         Chapter No.   2                                        Lecture No.6
- Topic : Hands on session on Flowcharts
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
- Recap of Previous Lecture
- • Structures are user-defined data types in C.
- • Used to group related data of different data types.
- • Structure members are accessed using the dot (.) operator.
- • Structures can be initialized during declaration.
- • Arrays and nested structures can be created using structures.
- • Structures help represent real-world entities efficiently.

### Slide 5
- Space for visual (size 24)
- Structure and Union
- PASSING ENTIRE STRUCTURE TO FUNCTION
- 5
- Syllabus/Topics To be Covered

### Slide 6
- 6
- A structure can be passed to any function from main function or from any sub function.
- Structure definition will be available within the function only.
- It won’t be available to other functions unless it is passed to those functions by value or by address(reference).
- Else, we have to declare structure variable as global variable. That means, structure variable should be declared outside the main function. So, this structure will be visible to all the functions in a C program.
- Structures and Functions

### Slide 7
- 7
- It can be done in below 3 ways.
- Passing structure to a function by value
- Passing structure to a function by address(reference)
- No need to pass a structure – Declare structure variable as global
- PASSING ENTIRE STRUCTURE TO FUNCTION IN C

### Slide 8
- 8
- It means the whole structure is passed to another function with all members and their values.
- So, this structure can be accessed from called function.
- This concept is very useful while writing very big programs in C.
- Example:
- #include <
- stdio.h
- >
- #include <
- string.h
- >
- struct student
- {
- int id;
- char name[20];
- float percentage;
- };
- void
- func
- (struct student record);
- Passing Structure to Function by Value

### Slide 9
- int main()
- {
- struct student record;
- record.id=1;
- strcpy
- (record.name, "Raju");
- record.percentage
- = 86.5;
- func
- (record);
- return 0;
- }
- void
- func
- (struct student record)
- {
- printf
- (" Id is: %d \n", record.id);
- printf
- (" Name is: %s \n", record.name);
- printf
- (" Percentage is: %f \n",
- record.percentage
- );
- }
- 9
- Output:
- Id is: 1
- Name is: Raju
- Percentage is: 86.500000

### Slide 10
- 10
- It means only the address of the structure is passed to another function.
- The whole structure is not passed to another function with all members and their values.
- So, this structure can be accessed from called function by its address.
- Example:
- #include <
- stdio.h
- >
- #include <
- string.h
- >
- struct student
- {
- int id;
- char name[20];
- float percentage;
- };
- Passing Structure to Function by Address
- (reference)

### Slide 11
- void
- func
- (struct student *record);
- int main()
- {
- struct student record;
- record.id=1;
- strcpy
- (record.name, "Raju");
- record.percentage
- = 86.5;
- func
- (&record);
- return 0;
- }
- void
- func
- (struct student *record)
- {
- printf
- (" Id is: %d \n", record->id);
- printf
- (" Name is: %s \n", record->name);
- printf
- (" Percentage is: %f \n", record->percentage);
- }
- 11
- Output:
- Id is: 1
- Name is: Raju
- Percentage is: 86.500000

### Slide 12
- 12
- Structure variables also can be declared as global variables as we declare other variables in C.
- So, When a structure variable is declared as global, then it is visible to all the functions in a program.
- In this scenario, we don’t need to pass the structure to any function separately.
- Example:
- #include <
- stdio.h
- >
- #include <
- string.h
- >
- struct student
- {
- int id;
- char name[20];
- float percentage;
- };
- Declare structure variable as global

### Slide 13
- struct student record; // Global declaration of structure
- void
- structure_demo
- ();
- int main()
- {
- record.id=1;
- strcpy
- (record.name, "Raju");
- record.percentage
- = 86.5;
- structure_demo
- ();
- return 0;
- }
- void
- structure_demo
- ()
- {
- printf
- (" Id is: %d \n", record.id);
- printf
- (" Name is: %s \n", record.name);
- printf
- (" Percentage is: %f \n",
- record.percentage
- );
- }
- 13
- Output:
- Id is: 1
- Name is: Raju
- Percentage is: 86.500000

### Slide 14
- Passing individual structure members
- We can pass individual members to a function just like ordinary variables.
- The following program demonstrates how to pass structure members as arguments to the function.
- Example:
- #include<stdio.h>
- /*
- structure is defined above all functions so it is global.
- */
- struct student
- {
- char name[20];
- int
- roll_no
- ;
- int marks;
- };
- void
- print_struct
- (char name[], int
- roll_no
- , int marks);
- 14

### Slide 15
- 15
- Output:
- Name: Tim
- Roll no: 1
- Marks: 78
- int main()
- {
- struct student
- stu
- = {"Tim", 1, 78};
- print_struct
- (stu.name,
- stu.roll_no
- ,
- stu.marks
- );
- return 0;
- }
- void
- print_struct
- (char name[], int
- roll_no
- , int marks)
- {
- printf
- ("Name: %s\n", name);
- printf
- ("Roll no: %d\n",
- roll_no
- );
- printf
- ("Marks: %d\n", marks);
- printf
- ("\n");
- }

### Slide 16
- Returning Structure Variable from a Function
- To return a structure from a function the return type should be a structure only.
- Example:
- // C++ program to return a structure from a function using Call By Value Method
- #include <iostream>
- #include <
- stdlib.h
- >
- using namespace std;
- // required structure
- struct Employee {
- int Id;
- string Name;
- };
- 16

### Slide 17
- // return type of the function is structure
- Employee data(Employee E)
- {
- // Assigning the values to elements
- E.Id
- = 45;
- E.Name
- = "
- aman
- ";
- Output:
- Employee Id: 45
- Employee Name:
- aman
- // returning structure
- return (E);
- }
- // Driver code
- int main()
- {
- // creating object of Employee
- Employee Emp;
- // calling function data to assign value
- Emp = data(Emp);
- // display the output
- cout
- << "Employee Id: " <<
- Emp.Id
- ;
- cout
- << "\
- nEmployee
- Name: " <<
- Emp.Name
- ;
- return 0;
- }
- 17
- Output:
- Employee Id: 45
- Employee Name:
- aman

### Slide 18
- Structure and Pointers
- Pointer to structure: Pointer which stores address of structure is called as “Pointer to Structure “.
- Explanation :
- sptr
- is pointer to structure address.
- -> and (*).  both represents the same.
- These operators are used to access data member of structure by using structure’s pointer.
- 18

### Slide 19
- Example:
- #include<stdio.h>
- struct team {
- char *name;
- int members;
- char captain[20];
- }
- t1 = {"India",11,"Dhoni"} , *
- sptr
- = &t1;
- int main()
- {
- printf
- ("\
- nTeam
- : %s",(*
- sptr
- ).name);
- printf
- ("\
- nMemebers
- : %d",
- sptr
- ->members);
- printf
- ("\
- nCaptain
- : %s",(*
- sptr
- ).captain);
- return 0;
- }
- 19
- Output
- :

### Slide 20
- 20
- Summary

### Slide 21
- Next Lecture
- • Introduction to Dynamic Memory Allocation
- • Need for Dynamic Memory Allocation
- • Memory Allocation Functions:
- - malloc()
- -
- calloc
- ()
- -
- realloc
- ()
- - free()
- • Dynamic Allocation of Arrays
- • Memory Deallocation and Best Practices
- • Program Examples and Applications

### Slide 22
- Frequently Asked Questions
- Q1
- Write a Program to enter the employee Information & display the data passing Structures By Using Pointers
- Expected Output:
- Enter the name of the Employee : John
- Enter the Employee Id : 16
- Enter Experience of the Employee : 3
- ---------Details List---------
- Employee Name : ram
- Employee Id : 16
- Employee Experience : 3
- Solution:
- 22

### Slide 23
- 23

### Slide 24
- Assessment Questions
- :
- 24
- 1. Write a Program to demonstrate How to return multiple values from a function in C?
- 2. Program to add two distances in inch-feet system(Passing structure).

### Slide 25
- Discussion forum
- PROBLEM:
- Write a Program to add two complex numbers Using (Passing struct by reference)
- .
- 25

### Slide 26
- REFERENCES
- Reference Books
- Programming in C by Reema
- Thareja
- .
- Programming in ANSI C by E.
- Balaguruswamy
- , Tata McGraw Hill.
- Programming with C (
- Schaum's
- Outline Series) by Byron Gottfried  Jitender Chhabra, Tata McGraw Hill.
- The C Programming Language by Brian W. Kernighan, Dennis Ritchie, Pearson education.
- Websites:
- https://www.studytonight.com/c/structures-in-c.php
- https://www.tutorialspoint.com/cprogramming/c_structures.htm
- https://www.geeksforgeeks.org/union-c/
- YouTube Links:
- https://www.youtube.com/watch?v=Ranc3VvjI88
- https://www.youtube.com/watch?v
- =zdUhS4YSWHg
- 26

### Slide 27
- NPTEL/ Coursera Courses
- 1. Problem Solving Through Programming in C
- https://onlinecourses.nptel.ac.in/e-learning/preview/noc24_cs42
- 2. Programming for Everybody (Getting Started with C)
- – Beginner Friendly
- https://www.coursera.org/learn/c-for-everyone
- 3. Duke University – Introductory C Programming Specialization
- https://www.coursera.org/specializations/c-programming

### Slide 28
- Class-wise
- feedback
- 28

### Slide 29
- THANK YOU
