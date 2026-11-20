# Chapter 3.1 - All Lecture Slides Text


## Chapter 7 Pointers Part 1
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
- Recap of Previous Lecture
- • User Defined Functions are created by programmers to perform specific tasks.
- • Help in code reusability and modular programming.
- • Consist of function declaration, definition, and function call.
- • Can accept arguments and return values.
- • Improve program readability and maintenance.

### Slide 4
- Space for visual (size 24)
- Introduction to Pointers
- Types of Pointers
- 4
- Syllabus/Topics To be Covered

### Slide 5
- 5
- POINTER is a variable that stores address of another variable.
- A pointer can also be used to refer to another pointer function.
- A pointer can be incremented/decremented, i.e., to point to the next/ previous memory location.
- The purpose of pointer is to save memory space and achieve faster execution time.
- Introduction
- Source:
- https://www.geeksforgeeks.org/double-pointer-pointer-pointer-c/

### Slide 6
- Features of Pointers
- Pointers save memory space.
- Execution time with pointers is faster because data are manipulated with the address, that is, direct
- access to memory
- location.
- Memory is accessed efficiently with the pointers. The pointer assigns and releases the memory as well. Hence it can be said the Memory of pointers is dynamically allocated.
- Pointers are used with data structures. They are useful for representing two-dimensional and multi-dimensional
- arrays.
- An array, of any type can be accessed with the help of pointers, without considering its subscript range.
- Pointers are used for file handling.
- Pointers are used to allocate memory dynamically.
- In C++, a pointer declared to a base class could access the object of a derived class. However, a pointer to a derived class cannot access the object of a base class.
- 6

### Slide 7
- Declaring a pointer
- Like variables, pointers have to be declared before they can be used in your program.
- Pointers can be named anything you want as long as they obey C's naming rules.
- A pointer declaration has the following form.
- data_type
- *
- pointer_variable_name
- ;
- Here,
- data_type
- is the pointer's base type of C's variable types and indicates the type of the variable that the pointer points to.
- The asterisk (*: the same asterisk used for multiplication) which is indirection operator, declares a pointer.
- 7

### Slide 8
- Initialize a pointer
- After declaring a pointer, we initialize it like standard variables with a variable address.
- If pointers are not uninitialized and used in the program, the results are unpredictable and potentially disastrous.
- To get the address of a variable, we use the ampersand (&)operator, placed before the name of a variable whose address we need.
- Pointer initialization is done with the following
- syntax
- :
- pointer = &variable;
- 8

### Slide 9
- Example:
- #include <
- stdio.h
- >
- int main()
- {
- int a=10;    //variable declaration
- int *p;      //pointer variable declaration
- p=&a;        //store address of variable a in pointer p
- printf
- ("Address stored in a variable p is:%x\
- n",p
- );  //accessing the address
- printf
- ("Value stored in a variable p is:%d\n",*p);   //accessing the value
- return 0;
- }
- Output:
- Address stored in a variable p is:60ff08
- Value stored in a variable p is:10
- 9

### Slide 10
- Operators used with Pointers
- 10
- Operator
- Meaning
- *
- Serves 2 purpose Declaration of a pointer
- Returns the value of the referenced variable
- &
- Serves only 1 purpose
- Returns the address of a variable

### Slide 11
- Types of a pointer
- Null pointer
- We can create a null pointer by assigning null value during the pointer declaration. This method is useful when you do not have any address assigned to the pointer. A null pointer always contains value 0.
- Following program illustrates the use of a null pointer:
- #include <
- stdio.h
- >
- int main()
- {
- int *p = NULL; 	//null pointer
- printf
- (“The value inside variable p is:\
- n%x
- ”,p);
- return 0;
- }
- Output:
- The value inside variable p is:
- 0
- 11

### Slide 12
- 2. Void Pointer
- In C programming, a void pointer is also called as a generic pointer. It does not have any standard data type. A void pointer is created by using the keyword void. It can be used to store an address of any variable.
- Following program illustrates the use of a void pointer:
- #include <
- stdio.h
- >
- int main()
- {
- void *p = NULL; 	//void pointer
- printf
- ("The size of pointer is:%d\n",
- sizeof
- (p));
- return 0;
- }
- Output:
- The size of pointer is:4
- 12

### Slide 13
- 3. Wild pointer
- A pointer is said to be a wild pointer if it is not being initialized to anything. These types of pointers are not efficient because they may point to some unknown memory location which may cause problems in our program and it may lead to crashing of the program. One should always be careful while working with wild pointers.
- Following program illustrates the use of wild pointer:
- #include <
- stdio.h
- >
- int main()
- {
- int *p; 	//wild pointer
- printf
- ("\
- n%d
- ",*p);
- return 0;
- }
- Output:
- timeout: the monitored command dumped core
- sh
- : line 1: 95298 Segmentation fault      timeout 10s main
- 13

### Slide 14
- Uses of pointers
- To pass arguments by reference
- For accessing array elements
- To return multiple values
- Dynamic memory allocation
- To implement data structures
- To do system level programming where memory addresses are useful
- 14

### Slide 15
- Disadvantages of pointer
- Uninitialized pointers might cause segmentation fault.
- Dynamically allocated block needs to be freed explicitly.
- If pointers are updated with incorrect values, it might lead to memory corruption.
- 15

### Slide 16
- 16
- Summary

### Slide 17
- Next Lecture
- • Introduction to Pointer Arithmetic
- • Incrementing and Decrementing Pointers
- • Adding and Subtracting Integers from Pointers
- • Difference Between Two Pointers
- • Pointer Arithmetic with Arrays
- • Applications and Program Examples

### Slide 18
- Frequently Asked question
- Q1:2)	What will be the output of the C program?
- #include<stdio.h>
- int main(){
- int
- i
- = 3;
- int *j;
- j = &
- i
- ;
- j++
- ;
- printf
- ("%d ",*j);
- return 0;
- }
- Output:
- 18

### Slide 19
- 2) What will be the output of the C program?
- #include<stdio.h>
- int main(){
- int a = 130;
- char *
- ptr
- ;
- ptr
- = (char *)&a;
- printf
- ("%d ",*
- ptr
- );
- return 0;
- }
- Ans : -126
- 19

### Slide 20
- Output:
- 20

### Slide 21
- Q3)    What is “&” and “*” operators in C?
- Ans:
- 1.	“*” Operator is used as pointer to a variable. Example: * a where * is pointer to the variable a.
- & operator is used to get the address of the variable. Example: &a will give address of a.
- Q4) WHAT IS VOID POINTER IN C?
- Ans:
- Void pointer is a generic pointer that can be used to point another variable of any data   type.
- Void pointer can store the address of variable belonging to any of the data type. So, void pointer is also called as general  purpose pointer.
- 21

### Slide 22
- Assessment Questions
- :
- 22
- 1.	C Program to calculate Area of Circle using Pointer
- 2.	Write a C Program to Swap Two Numbers / Variables using Pointer?
- 3.	What will be the output of the C program?
- #include<stdio.h>
- #include<string.h>
- int main(){
- char *
- ptr
- = "hello";
- char a[22];
- strcpy
- (a, "world");
- printf
- ("\
- n%s
- %s",
- ptr
- , a);
- return 0;
- }

### Slide 23
- Discussion forum
- .
- Other types of pointers in 'c' are as follows:
- Dangling pointer
- Complex pointer
- Near pointer
- Far pointer
- Huge pointer
- Write a program to count the number of words, lines and characters in a text using pointer
- 23

### Slide 24
- REFERENCES
- Reference Books
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
- Websites:
- https://www.geeksforgeeks.org/features-and-use-of-pointers-in-c-c/
- https://www.guru99.com/c-pointers.html
- YouTube Links:
- https://www.youtube.com/watch?v=sY-s7O0FiYE&t=3s
- https://www.youtube.com/watch?v=qcWQ1AmmNWI&t=193s
- 24

### Slide 25
- Class-wise
- feedback
- 25

### Slide 26
- THANK YOU


## Chapter 7 Pointers Part 2
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
- Pointers Arithmetic
- 3
- Syllabus/Topics To be Covered

### Slide 4
- Recap of Previous Lecture
- • Pointers are variables that store memory addresses.
- • Declared using the (*) operator.
- • The address-of operator (&) obtains the address of a variable.
- • The dereference operator (*) accesses the value stored at an address.
- • Pointers enable efficient memory access and manipulation.
- • Widely used with arrays, functions, and dynamic memory allocation.

### Slide 5
- 5
- We already know that a pointer points to a location in memory and thus used to store the address of variables.
- So, when we define a pointer to pointer.
- The first pointer is used to store the address of the variable.
- And the second pointer is used to store the address of the first pointer.
- That is why they are also known as double pointers.
- Syntax:
- int **
- ptr
- ;    // declaring double pointers
- Introduction
- Source:
- https://www.geeksforgeeks.org/double-pointer-pointer-pointer-c/

### Slide 6
- Below diagram explains the concept of Double Pointers:
- Source:
- https://www.geeksforgeeks.org/double-pointer-pointer-pointer-c/
- The above diagram shows the memory representation of a pointer to pointer. The first pointer ptr1 stores the address of the variable and the second pointer ptr2 stores the address of the first pointer.
- 6

### Slide 7
- Example:
- #include <
- stdio.h
- >
- // C program to demonstrate pointer to pointer
- int main()
- {
- int var = 789;
- // pointer for var
- int *ptr2;
- // double pointer for ptr2
- int **ptr1;
- // storing address of var in ptr2
- ptr2 = &var;
- // Storing address of ptr2 in ptr1
- ptr1 = &ptr2;
- // Displaying value of var using both single and double pointers
- printf
- ("Value of var = %d\n", var );
- printf
- ("Value of var using single pointer = %d\n", *ptr2 );
- printf
- ("Value of var using double pointer = %d\n", **ptr1);
- return 0;
- }
- 7
- Output:
- Value of var = 789
- Value of var using single pointer = 789
- Value of var using double pointer = 789

### Slide 8
- Pointer Arithmetic
- We can perform arithmetic operations on the pointers like addition, subtraction, etc.
- However, as we know that pointer contains the address, the result of an arithmetic operation performed on the pointer will also be a pointer if the other operand is of type integer.
- In pointer-from-pointer subtraction, the result will be an integer value.
- Following arithmetic operations are possible on the pointer in C language:
- Increment
- Decrement
- Addition
- Subtraction
- Comparison
- 8

### Slide 9
- Incrementing Pointer in C
- If we increment a pointer by 1, the pointer will start pointing to the immediate next location.
- This is somewhat different from the general arithmetic since the value of the pointer will get increased by the size of the data type to which the pointer is pointing.
- We can traverse an array by using the increment operation on a pointer which will keep pointing to every element of the array, perform some operation on that, and update itself in a loop.
- The Rule to increment the pointer is given below:
- new_address
- =
- current_address
- +
- i
- *
- size_of
- (data type)
- where
- i
- is the number by which the pointer get increased.
- 9

### Slide 10
- Example: Traversing an array by using pointer
- #include<stdio.h>
- void main ()
- {
- int
- arr
- [5] = {1, 2, 3, 4, 5};
- int *p =
- arr
- ;
- int
- i
- ;
- printf
- ("printing array elements...\n");
- for(
- i
- = 0;
- i
- < 5;
- i
- ++)
- {
- printf
- ("%d  ",*(
- p+i
- ));
- }
- }
- Output:
- printing array elements...
- 1  2  3  4  5
- 10
- Note:
- 32-bit
- For 32-bit int variable, it will be incremented by 2 bytes.
- 64-bit
- For 64-bit int variable, it will be incremented by 4 bytes.

### Slide 11
- Decrementing Pointer in C
- Like increment, we can decrement a pointer variable.
- If we decrement a pointer, it will start pointing to the previous location.
- The formula of decrementing the pointer is given below:
- new_address
- =
- current_address
- -
- i
- *
- size_of
- (data type)
- Note:
- 32-bit:
- For 32-bit int variable, it will be decremented by 2 bytes.
- 64-bit:
- For 64-bit int variable, it will be decremented by 4 bytes.
- 11

### Slide 12
- Example: Decrementing pointer variable on 64-bit OS.
- #include <
- stdio.h
- >
- void main(){
- int number=50;
- int *p;//pointer to int
- p=&number;//stores the address of number variable
- printf
- ("Address of p variable is %u \
- n",p
- );
- p=p-1;
- printf
- ("After decrement: Address of p variable is %u \
- n",p
- ); // P will now point to the immediate previous location.
- }
- Output:
- Address of p variable is 3214864300
- After decrement: Address of p variable is 3214864296
- 12

### Slide 13
- C Pointer Addition
- We can add a value to the pointer variable.
- The formula of adding value to pointer is given below:
- new_address
- =
- current_address
- + (number *
- size_of
- (data type))
- Note:
- 32-bit:
- For 32-bit int variable, it will add 2 * number.
- 64-bit:
- For 64-bit int variable, it will add 4 * number.
- 13

### Slide 14
- Example:Adding
- value to pointer variable on 64-bit architecture.
- #include<stdio.h>
- int main(){
- int number=50;
- int *p;//pointer to int
- p=&number;//stores the address of number variable
- printf
- ("Address of p variable is %u \
- n",p
- );
- p=p+3;   //adding 3 to pointer variable
- printf
- ("After adding 3: Address of p variable is %u \
- n",p
- );
- return 0;
- }
- Output:
- Address of p variable is 3214864300
- After adding 3: Address of p variable is 3214864312
- As you can see, the address of p is 3214864300. But after adding 3 with p variable, it is 3214864312, i.e., 4*3=12 increment. Since we are using 64-bit architecture, it increments 12. But if we were using 32-bit architecture, it was incrementing to 6 only, i.e., 2*3=6. As integer value occupies 2-byte memory in 32-bit OS.
- 14

### Slide 15
- C Pointer Subtraction
- Like pointer addition, we can subtract a value from the pointer variable. Subtracting any number from a pointer will give an address.
- The formula of subtracting value from the pointer variable is given below:
- new_address
- =
- current_address
- - (number *
- size_of
- (data type))
- Note:
- 32-bit:For 32-bit int variable, it will subtract 2 * number.
- 64-bit:For 64-bit int variable, it will subtract 4 * number.
- 15

### Slide 16
- Example: Subtracting value from the pointer variable on 64-bit architecture.
- #include<stdio.h>
- int main(){
- int number=50;
- int *p;//pointer to int
- p=&number;//stores the address of number variable
- printf
- ("Address of p variable is %u \
- n",p
- );
- p=p-3; //subtracting 3 from pointer variable
- printf
- ("After subtracting 3: Address of p variable is %u \
- n",p
- );
- return 0;
- }
- Output:
- Address of p variable is 3214864300
- After subtracting 3: Address of p variable is 3214864288
- You can see after subtracting 3 from the pointer variable, it is 12 (4*3) less than the previous address value.
- However, instead of subtracting a number, we can also subtract an address from another address (pointer).
- This will result in a number.
- It will not be a simple arithmetic operation, but it will follow the following rule.
- 16

### Slide 17
- If two pointers are of the same type,
- Address2 - Address1 = (Subtraction of two addresses)/size of data type which pointer points
- Consider the following example to subtract one pointer from an another.
- #include<stdio.h>
- void main ()
- {
- int
- i
- = 100;
- int *p = &
- i
- ;
- int *temp;
- temp = p;
- p = p + 3;
- printf
- ("Pointer Subtraction: %d - %d = %
- d",p
- , temp, p-temp);
- }
- Output:
- Pointer Subtraction: 1030585080 - 1030585068 = 3
- 17

### Slide 18
- Illegal arithmetic with pointers
- There are various operations which can not be performed on pointers.
- Since, pointer stores address hence we must ignore the operations which may lead to an illegal address, for example, addition, and multiplication.
- A list of such operations is given below.
- Address + Address = illegal
- Address * Address = illegal
- Address % Address = illegal
- Address / Address = illegal
- Address & Address = illegal
- Address ^ Address = illegal
- Address | Address = illegal
- ~Address = illegal
- 18

### Slide 19
- Pointers and  Arrays
- When an array is declared, compiler allocates sufficient amount of memory to contain all the elements of the array.
- Base address
- i.e
- address of the first element of the array is also allocated by the compiler.
- Suppose we declare an array
- arr
- ,
- int
- arr
- [5] = { 1, 2, 3, 4, 5 };
- Assuming that the base address of
- arr
- is 1000 and each integer requires two bytes, the five elements will be stored as follows:
- Here variable
- arr
- will give the base address, which is a constant pointer pointing to the first element of the array,
- arr
- [0]. Hence
- arr
- contains the address of
- arr
- [0]
- i.e
- 1000. In short,
- arr
- has two purpose - it is the name of the array and it acts as a pointer pointing towards the first element in the array.
- arr
- is equal to &
- arr
- [0] by default
- 19

### Slide 20
- We can also declare a pointer of type int to point to the array arr.
- int *p;
- p =
- arr
- ;
- // or,
- p = &
- arr
- [0];    //both the statements are equivalent.
- Now we can access every element of the array
- arr
- using p++ to move from one element to another.
- NOTE: You cannot decrement a pointer once incremented. p-- won't work.
- 20

### Slide 21
- Pointer to Array
- As studied above, we can use a pointer to point to an array, and then we can use that pointer to access the array elements.
- Lets have an example
- ,
- #include <
- stdio.h
- >
- int main()
- {
- int
- i
- ;
- int a[5] = {1, 2, 3, 4, 5};
- int *p = a;     // same as int*p = &a[0]
- for (
- i
- = 0;
- i
- < 5;
- i
- ++)
- {
- printf
- ("%d", *p);
- p++;
- }
- return 0;
- }
- In the above program, the pointer *p will print all the values stored in the array one by one. We can also use the Base address (a in above case) to act as a pointer and print all the values.
- 21

### Slide 22
- The generalized form for using pointer with an array
- *(
- a+i
- )
- is same as
- a[
- i
- ].
- Source:
- https://www.studytonight.com/c/pointers-with-array.php
- 22

### Slide 23
- Pointer to Multidimensional Array
- A multidimensional array is of form, a[
- i
- ][j].
- Lets see how we can make a pointer point to such an array.
- As we know now, name of the array gives its base address.
- In a[
- i
- ][j], a will give the base address of this array, even a + 0 + 0 will also give the base address, that is the address of a[0][0] element.
- Here is the generalized form for using pointer with multidimensional arrays.
- *(*(a +
- i
- ) + j)
- which is same as,
- a[
- i
- ][j]
- 23

### Slide 24
- Array of Pointers
- We can also have array of pointers.
- Pointers are very helpful in handling character array with rows of varying length.
- Example:
- char *name[3] = {
- "Adam",
- "
- chris
- ",
- "
- Deniel
- "
- };
- //Now lets see same array without using pointer
- char name[3][20] = {
- "Adam",
- "
- chris
- ",
- "
- Deniel
- "
- };
- 24
- Source:
- https://www.studytonight.com/c/pointers-with-array.php

### Slide 25
- In the second approach memory wastage is more, hence it is
- prefered
- to use pointer in such cases.
- Note:
- When we say memory wastage, it doesn't means that the strings will start occupying less space, no, characters will take the same space, but when we define array of characters, a contiguous memory space is located equal to the maximum size of the array, which is a wastage, which can be avoided if we use pointers instead.
- 25

### Slide 26
- Example: Array of Pointers
- #include <
- stdio.h
- >
- const
- int MAX = 3;
- int main ()
- {
- int  var[] = {10, 100, 200};
- int
- i
- ;
- for (
- i
- = 0;
- i
- < MAX;
- i
- ++)
- {
- printf
- ("Value of var[%d] = %d\n",
- i
- , var[
- i
- ] );
- }
- return 0;
- }
- Output:
- Value of var[0] = 10
- Value of var[1] = 100
- Value of var[2] = 200
- 26

### Slide 27
- 27
- Summary

### Slide 28
- Next Lecture
- • Passing Pointers as Function Arguments
- • Returning Pointers from Functions
- • Call by Reference Using Pointers
- • Swapping Values Using Pointers
- • Functions with Arrays and Pointers
- • Program Examples and Applications

### Slide 29
- Next Lecture
- • Introduction to Storage Classes
- • Automatic (auto) Storage Class
- • Register Storage Class
- • Static Storage Class
- • External (extern) Storage Class
- • Scope, Lifetime, and Visibility of Variables
- • Program Examples and Applications

### Slide 30
- Frequently Asked question
- Q1:Write a C program to Biggest value in the array using pointers in C
- Solution:
- 30
- #include <
- stdio.h
- >
- int main()
- {
- long array[100], *maximum, size, c, location = 1;
- printf
- ("Enter the number of elements in array\n");
- scanf
- ("%
- ld
- ", &size);
- printf
- ("Enter %
- ld
- integers\n", size);
- for ( c = 0 ; c < size ;
- c++
- )
- scanf
- ("%
- ld
- ", &array[c]);
- maximum  = array;
- *maximum = *array;
- for (c = 1; c < size;
- c++
- )
- {
- if (*(
- array+c
- ) > *maximum)
- {
- *maximum = *(
- array+c
- );
- location = c+1;
- }
- }
- printf
- ("Maximum element is present at location number %
- ld
- and it's value is %ld.\n", location, *maximum);
- return 0;
- }

### Slide 31
- 2) Write C Program to Add Two Numbers Using Pointer
- Solution:
- #include<stdio.h>
- int main() {
- int *ptr1, *ptr2;
- int
- num
- ;
- printf
- ("\
- nEnter
- two numbers : ");
- scanf
- ("%d %d", ptr1, ptr2);
- num
- = *ptr1 + *ptr2;
- printf
- ("Sum = %d",
- num
- );
- return (0);
- }
- 31
- Output:

### Slide 32
- Output:
- 32

### Slide 33
- Q3)    What is “&” and “*” operators in C?
- Ans:
- 1.	“*” Operator is used as pointer to a variable. Example: * a where * is pointer to the variable a.
- & operator is used to get the address of the variable. Example: &a will give address of a.
- Q4) WHAT IS VOID POINTER IN C?
- Ans:
- Void pointer is a generic pointer that can be used to point another variable of any data   type.
- Void pointer can store the address of variable belonging to any of the data type. So, void pointer is also called as general  purpose pointer.
- 33

### Slide 34
- Assessment Questions
- :
- 34
- C Program to compute sum of the array elements using pointers ?
- Write a C program to Find transpose of a matrix.
- Write a C program to find the length of string using pointers.
- What will be the output of the C program?
- #include<stdio.h>
- #include<string.h>
- int main(){
- char *
- ptr
- = "hello";
- char a[22];
- *
- ptr
- = "world";
- printf
- ("\
- n%s
- %s",
- ptr
- , a);
- return 0;
- }
- What will be the output of the C program?
- #include<stdio.h>
- int main(){
- int
- i
- = 3;
- int *j;
- int **k;
- j = &
- i
- ;
- k = &j;
- k++;
- printf
- ("%d ",**k);
- return 0;
- }

### Slide 35
- Discussion forum
- .
- C Program to read integers into an array and reversing them using pointers
- 35

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
- https://www.geeksforgeeks.org/double-pointer-pointer-pointer-c/
- https://www.studytonight.com/c/pointers-with-array.php
- YouTube Links:
- https://www.youtube.com/watch?v=ahKfY1EsWd8&t=1s
- https://www.youtube.com/watch?v=jYuqC9UD4GI
- https://www.youtube.com/watch?v=kKKvGYAX_Zs
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


## Chapter 7 Pointers Part 3 and Storage classes
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
- Recap of Previous Lecture
- • Pointer arithmetic allows manipulation of memory addresses.
- • Pointers can be incremented (++) and decremented (--).
- • Integers can be added to or subtracted from pointers.
- • The difference between two pointers gives the number of elements between them.
- • Commonly used for traversing arrays efficiently.
- • Pointer arithmetic depends on the size of the data type.

### Slide 4
- Space for visual (size 24)
- Call by value and Call by reference
- Passing Pointer to function
- Function Returning pointer
- Storage classes
- 4
- Syllabus/Topics To be Covered

### Slide 5
- Call by Value Vs Call by Address
- Call by Value
- Call by Reference
- The actual arguments can be variable or constant.
- The actual arguments can only be variable.
- The values of actual argument are sent to formal argument which are normal variables.
- The reference of actual argument are sent to formal argument which are pointer variables.
- Any changes made by formal arguments will not reflect to actual arguments.
- Any changes made by formal arguments will reflect to actual arguments.
- 5

### Slide 6
- Example: Passing Pointers to Functions
- #include <
- stdio.h
- >
- void
- addOne
- (int*
- ptr
- ) {
- (*
- ptr
- )++; // adding 1 to *
- ptr
- }
- int main()
- {
- int* p,
- i
- = 10;
- p = &
- i
- ;
- addOne
- (p);
- printf
- ("%d", *p); // 11
- return 0;
- }
- 6
- Output:

### Slide 7
- Explanation of the Program:
- Here, the value stored at p, *p, is 10 initially.
- We then passed the pointer p to the
- addOne
- () function. The
- ptr
- pointer gets this address in the
- addOne
- () function.
- Inside the function, we increased the value stored at
- ptr
- by 1 using (*
- ptr
- )++;. Since
- ptr
- and p pointers both have the same address, *p inside main() is also 11.
- 7

### Slide 8
- Function Returning a Pointer
- Like normal variable, a function can also return reference or address. When function returns reference or address, the return type of function must be pointer type.
- Syntax for function returning pointer:
- return-type *function-name(argument list)
- {
- - - - - - - - - - -
- body of function
- - - - - - - - - - -
- }
- 8

### Slide 9
- Example:  Write a C program for function returning pointer
- #include <
- stdio.h
- >
- int *reference(int *n);  // Function declaration
- int main() {
- int A = 10;
- int *
- ptr
- ;
- printf
- ("Address of A in main() is %u\n", &A);
- ptr
- = reference(&A);
- printf
- ("Address of A in reference() is %u\n",
- ptr
- );
- printf
- ("Value pointed by
- ptr
- is %d\n", *
- ptr
- );
- return 0;
- }
- int *reference(int *n) {
- // Function now receives and returns a valid address
- return n;
- }
- 9
- Output:

### Slide 10
- A function can also return a pointer to the calling function.
- In this case you must be careful, because local variables of function doesn't live outside the function.
- They have scope only inside the function.
- Hence if you return a pointer connected to a local variable, that pointer will be pointing to nothing when the function ends.
- 10

### Slide 11
- Storage Classes
- Storage Classes defines the scope and life time of variable declare in a function.
- Types of Storage Classes
- Auto ( Automatic ) storage class
- Static storage class
- Extern ( External ) storage class
- Register storage class
- 11

### Slide 12
- Auto (Automatic) storage class - Auto variables
- Auto variables have local scope. All the variables declared in function are auto, by default. We can declare same variables in different functions as well.
- The auto keyword is optional, there is no need to write it.
- All the formal arguments have auto scope.
- If not initialized auto variables have garbage value.
- The value is lost after the execution of function.
- Syntax of auto storage class:
- auto Data-type Variable-name;
- OR
- Data-type Variable-name;
- 12

### Slide 13
- Example of auto storage class
- #include<stdio.h>
- void display();
- int main()
- {
- auto int a=10;       //OR int a=10;
- printf
- ("\
- nA
- : %
- d",a
- );
- display();
- printf
- ("\
- nA
- : %
- d",a
- );
- }
- void display()
- {
- int a=20;               //OR auto int a=20;
- printf
- ("\
- nA
- : %
- d",a
- );
- }
- 13
- Output:

### Slide 14
- Static storage class - Static variables
- Static variable also have local scope as automatic variables. During multiple calling static variables retains their previous value.
- We must declare variable as static.
- Static variables can't be accessed outside the function.
- If not initialized static variables have zero as initial value.
- Syntax of static storage class:
- static Data-type Variable-name;
- 14

### Slide 15
- Example of static storage class:
- #include<stdio.h>
- void display();
- int main()
- {
- display();
- display();
- display();
- }
- void display()
- {
- static int a=1;
- printf
- ("\
- nA
- : %
- d",a
- );
- a++;
- }
- 15
- Output:

### Slide 16
- Extern (External) storage class - External variables
- External variables have global scope. They are declared outside all the functions.
- The extern keyword is optional, there is no need to write it.
- The scope of external variable is the entire program.
- If not initialized external variable is assigned a zero value.
- The value is not lost after the execution of function.
- One function can assign value and another can display the value.
- Syntax of external storage class or global variable
- extern Data-type Variable-name;
- OR
- Data-type Variable-name;
- 16

### Slide 17
- Example of external storage class or global variable
- #include<stdio.h>
- void display();
- int a=10;                     //global variable
- int main()
- {
- printf
- ("\
- nA
- : %
- d",a
- );
- increment();
- display();
- printf
- ("\
- nA
- : %
- d",a
- );
- }
- 17
- Output:
- A : 10
- A : 20
- A : 20
- void increment()
- {
- a = 20;
- }
- void display()
- {
- printf
- ("\
- nA
- : %
- d",a
- );
- }
- a++;
- }

### Slide 18
- Register storage class - Register variables
- Register variables have local scope as automatic variables. They are declared within motherboard's register memory. All the arithmetic and logical operations are carried out within these registers.
- These variables are stored in registers. If registers are not available values are stored in main memory.
- Register variables works faster then other kind of variables because register memory is
- fatser
- then main memory.
- Address operator '&' can't be used with these variables.
- Pointer to register variables are not allowed.
- These variables are used for loops to increase efficiency.
- Syntax of register storage class:
- register Data-type Variable-name;
- 18

### Slide 19
- Example of register storage class
- include<
- stdio.h
- >
- int main()
- {
- register int a=10;
- printf
- ("\
- nA
- : %
- d",a
- );
- }
- Output:
- 19

### Slide 20
- The table summarizes the principal features of each storage class which are commonly used in C programming:
- 20
- Storage Class
- Declaration
- Storage
- Default Initial Value
- Scope
- Lifetime
- auto
- Inside a function/block
- Memory
- Unpredictable
- Within the function/block
- Within the function/block
- register
- Inside a function/block
- CPU Registers
- Garbage
- Within the function/block
- Within the function/block
- extern
- Outside all functions
- Memory
- Zero
- Entire the file and other files where the variable is declared as extern
- program runtime
- Static (local)
- Inside a function/block
- Memory
- Zero
- Within the function/block
- program runtime
- Static (global)
- Outside all functions
- Memory
- Zero
- Global
- program runtime

### Slide 21
- 21
- Summary

### Slide 22
- Next Lecture
- • Introduction to Structures
- • Defining and Declaring Structures
- • Accessing Structure Members
- • Initialization of Structures
- • Arrays of Structures
- • Nested Structures
- • Practical Programs Using Structures

### Slide 23
- Frequently Asked question
- Q1:What will the Output of the Program?
- #include<stdio.h>
- int main()
- {
- printf
- ("%d",
- sizeof
- (void *));
- return 0;
- }
- Output:
- 23

### Slide 24
- 2) What will be the Output?
- #include<stdio.h>
- void function(char**);
- int main()
- {
- char *
- arr
- [] = { "ant", "bat", "cat", "dog", "egg", "fly" };
- function(
- arr
- );
- return 0;
- }
- void function(char **
- ptr
- )
- {
- char *ptr1;
- ptr1 = (
- ptr
- +=
- sizeof
- (int))[-2];
- printf
- ("%s\n", ptr1);
- }
- return (0);}
- 24
- Output:

### Slide 25
- Q3)    What is “&” and “*” operators in C?
- Ans:
- 1.	“*” Operator is used as pointer to a variable. Example: * a where * is pointer to the variable a.
- & operator is used to get the address of the variable. Example: &a will give address of a.
- Q4) WHAT IS VOID POINTER IN C?
- Ans:
- Void pointer is a generic pointer that can be used to point another variable of any data   type.
- Void pointer can store the address of variable belonging to any of the data type. So, void pointer is also called as general  purpose pointer.
- 25

### Slide 26
- Assessment Questions
- :
- 26
- What will be the output of the C program?
- #include<stdio.h>
- int main(){
- int a = 25, b;
- int *
- ptr
- , *ptr1;
- ptr
- = &a;
- ptr1 = &b;
- b = 36;
- printf
- ("%d %d",*
- ptr
- , *ptr1);
- return 0;
- }
- 2.	What will be the output of the C program?
- #include<stdio.h>
- int main(){
- int *
- ptr
- ;
- printf
- ("%d",
- sizeof
- (
- ptr
- ));
- return 0;
- }

### Slide 27
- 3.     What will be the output of the C program?
- #include<stdio.h>
- int main()
- {
- char *str = "His";
- int
- i
- ;
- for(
- i
- = 0;
- i
- <
- strlen
- (str);
- i
- ++)
- printf
- ("%s", str++);
- return 0;
- }
- 27

### Slide 28
- Discussion forum
- .
- Write a program in C to add numbers using call by reference.
- 28

### Slide 29
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
- https://www.programiz.com/c-programming/c-pointer-functions
- https://www.studytonight.com/c/pointer-with-function-in-c.php
- YouTube Links:
- 1.
- https://www.youtube.com/watch?v=BRsv3ZXoHto
- 29

### Slide 30
- Class-wise
- feedback
- 30

### Slide 31
- THANK YOU
