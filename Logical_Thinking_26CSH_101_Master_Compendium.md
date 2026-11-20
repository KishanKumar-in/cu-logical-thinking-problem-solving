# LOGICAL THINKING AND PROBLEM SOLVING (CONT_26CSH-101 / 26CSH-101)
## Master Examination Definition, Algorithm, Concept & Code Compendium — Units 1, 2 and 3

**Course:** Logical Thinking and Problem Solving (`CONT_26CSH-101` / `26CSH-101`)  
**University:** Chandigarh University  
**Academic Session:** 2026–27  
**Source Repository:** [`KishanKumar-in/cu-logical-thinking-problem-solving`](https://github.com/KishanKumar-in/cu-logical-thinking-problem-solving)  
**Primary Source:** `_COMPLETE_CONT_26CSH-101 — Semester Master Notes`

---

### EXAMINER'S COVERAGE & METHODOLOGY NOTE

- **[DIRECTLY IN NOTES]**: Core syllabus concepts explicitly covered in CU course materials, lecture notes, and presentation slides.
- **[RESTORED STANDARD EQUATION / CODE]**: Standard C formulations, memory address formulas, and complete working code included for completeness.
- **[EXAM SUPPORT]**: Step-by-step algorithms, dry-run tracing tables, time/space complexity analysis, and solved numericals.
- **⚠ Examiner’s flag**: Critical warnings highlighting common student traps, compilation errors, undefined behavior, memory leaks, and examination pitfalls.

---


# UNIT 1: PROBLEM SOLVING, ALGORITHMS, FLOWCHARTS & C FUNDAMENTALS

UNIT 1: PROBLEM SOLVING, ALGORITHMS, FLOWCHARTS & C FUNDAMENTALS

## Chapter 1.1: Problem Solving and Algorithms


### 1.1.1 Introduction to Problem Solving

[DIRECTLY IN NOTES]
Definition:
Problem solving is a systematic process of identifying a problem, analysing its requirements, developing a logical solution, implementing the solution and verifying that the result is correct.
In computer programming, problem solving involves converting a real-world problem into a sequence of instructions that a computer can execute.
Objectives of problem solving:
Understand the problem clearly.
Identify the required input.
Determine the expected output.
Develop a logical solution.
Implement the solution using a programming language.
Test and debug the implementation.
Improve efficiency and reliability.

### 1.1.2 Phases of Problem Solving

[DIRECTLY IN NOTES]
Problem solving consists of five major phases.
1. Problem Analysis
The problem is studied to identify its requirements.
Activities:
Understand the problem statement.
Identify available inputs.
Determine required outputs.
Identify constraints.
Identify special cases.
2. Solution Design
A logical solution is developed before writing the program.
Common techniques:
Algorithms.
Flowcharts.
Pseudocode.
Modular decomposition.
3. Coding
The designed solution is translated into a programming language such as C.
4. Testing
The program is executed using different test cases to verify its correctness.
Types of testing:
Normal test cases.
Boundary test cases.
Invalid input test cases.
Special test cases.
5. Debugging
Debugging is the process of locating, analysing and correcting errors in a program.
Types of programming errors:
Error
Description
Example
Syntax error
Violation of language grammar
Missing semicolon
Logical error
Incorrect algorithm or logic
Wrong formula
Runtime error
Error occurring during execution
Division by zero
Compilation error
Compiler cannot translate the source
Undeclared identifier
```text
Problem-solving lifecycle:
START
  |
  v
Problem Analysis
  |
  v
Solution Design
  |
  v
Coding
  |
  v
Testing ----[Is it correct?]----
  |             |             |
 (No)          (Yes)          |
  |             |             |
  v             v             |
Debugging   Final Program     |
  |                           |
  +---------------------------+
```
[EXAM SUPPORT]
Example: Find the sum of two numbers.
Problem analysis:
Input: Two integers a and b.
Processing: Add the two integers.
Output: Sum.
Algorithm:
Start.
Read a and b.
Calculate sum = a + b.
Display sum.
Stop.
C implementation:
#include <stdio.h> int main(void) { int a, b, sum; // Read two integers printf("Enter two numbers: "); scanf("%d %d", &a, &b); // Calculate their sum sum = a + b; // Display the result printf("Sum = %d\n", sum); return 0; }
Dry run:
Step
a
b
Operation
sum
Input
10
20
Read values
-
Processing
10
20
10 + 20
30
Output
10
20
Display
30
Complexity:
Time complexity: \(O(1)\)
Auxiliary space complexity: \(O(1)\)

### 1.1.3 Algorithm

[DIRECTLY IN NOTES]
Definition:
An algorithm is a finite, ordered sequence of well-defined instructions designed to solve a particular computational problem.
An algorithm accepts input, processes it according to specified rules and produces the required output.
Characteristics of an algorithm
There are five fundamental characteristics.
1. Input
An algorithm may accept zero or more inputs.
Example: Two integers a and b.
2. Output
An algorithm must produce at least one meaningful output.
Example: Sum of two integers.
3. Definiteness
Every instruction must be clear, precise and unambiguous.
4. Finiteness
An algorithm must terminate after a finite number of steps.
5. Effectiveness
Every operation must be sufficiently basic and executable within a finite amount of time.
Characteristic
Meaning
Input
Zero or more input values
Output
At least one output
Definiteness
Instructions must be unambiguous
Finiteness
Must terminate
Effectiveness
Operations must be executable

### 1.1.4 Algorithm Representation

Algorithms can be represented using:
Natural language.
Pseudocode.
Flowcharts.
Programming languages.
Example: Algorithm to find the largest of two numbers
ALGORITHM LargestOfTwo 1. START 2. INPUT A, B 3. IF A > B THEN PRINT A ELSE PRINT B 4. STOP
Dry run:
A
B
Condition A > B
Output
20
10
True
20
5
15
False
15
10
10
False
10

### 1.1.5 Time Complexity

[RESTORED STANDARD EQUATION / CODE]
Definition:
Time complexity represents how the number of computational operations performed by an algorithm grows as the input size increases.
It is expressed using asymptotic notation.
Big-O notation
Big-O represents an asymptotic upper bound on the growth rate.
Common complexities:
Complexity
Name
Example
\(O(1)\)
Constant
Accessing an array element
\(O(\log n)\)
Logarithmic
Binary search
\(O(n)\)
Linear
Linear search
\(O(n\log n)\)
Linearithmic
Merge sort
\(O(n^2)\)
Quadratic
Bubble sort
\(O(2^n)\)
Exponential
Naive Fibonacci
\(O(n!)\)
Factorial
Generating all permutations
Example 1: Constant complexity
int getFirst(int arr[]) { return arr[0]; }
Only one array element is accessed.
\[ T(n)=O(1) \]
Example 2: Linear complexity
void display(int arr[], int n) { for (int i = 0; i < n; i++) { printf("%d ", arr[i]); } }
The loop executes \(n\) times.
\[ T(n)=O(n) \]
Example 3: Quadratic complexity
void printPairs(int n) { for (int i = 0; i < n; i++) { for (int j = 0; j < n; j++) { printf("%d %d\n", i, j); } } }
The outer loop executes \(n\) times, and the inner loop executes \(n\) times for every outer iteration.
\[ T(n)=n\times n \]
\[ T(n)=O(n^2) \]

### 1.1.6 Space Complexity

Definition:
Space complexity represents the total memory required by an algorithm as a function of input size.
It includes:
Input storage.
Variables.
Auxiliary data structures.
Function call stack.
Recursion overhead.
Example:
int sum(int a, int b) { int result = a + b; return result; }
The function uses a fixed amount of auxiliary storage.
\[ S(n)=O(1) \]
Difference between time and space complexity
Time Complexity
Space Complexity
Measures execution growth
Measures memory growth
Counts computational work
Measures storage requirements
Expressed using \(O\), \(\Theta\), \(\Omega\)
Expressed using the same notations

### 1.1.7 Best, Average and Worst Cases

[EXAM SUPPORT]
Consider linear search.
int linearSearch(int arr[], int n, int key) { for (int i = 0; i < n; i++) { if (arr[i] == key) return i; } return -1; }
Case
Situation
Complexity
Best
Element at first position
\(O(1)\)
Average
Element around middle
\(O(n)\)
Worst
Element at last position or absent
\(O(n)\)

### 1.1.8 Flowcharts

[DIRECTLY IN NOTES]
Definition:
A flowchart is a graphical representation of an algorithm using standardised symbols connected by directional arrows.
Flowcharts illustrate the sequence of operations and decision-making processes in a program.
Standard flowchart symbols
Symbol
Shape
Purpose
Terminal
Oval
Start or Stop
Input/Output
Parallelogram
Read or display data
Process
Rectangle
Calculation or assignment
Decision
Diamond
Conditional checking
Connector
Circle
Connect different flowchart sections
Flow line
Arrow
Direction of execution
Flowchart example: Addition of two numbers
( START ) | v / Input A, B / | v +-------------+ | SUM = A + B | +-------------+ | v / Display SUM / | v ( STOP )
Flowchart example: Check even or odd
( START ) | v / Input N / | v < N % 2 == 0? > / \ YES NO | | v v / Print Even / / Print Odd / | | +----+-----+ | v ( STOP )
Advantages of flowcharts
Easy to understand.
Improves logical thinking.
Helps identify errors.
Simplifies communication.
Helps in program documentation.
Makes complex processes easier to visualise.
Limitations of flowcharts
Large flowcharts become difficult to manage.
Modifications may require redrawing.
Time-consuming for complicated problems.
Not ideal for representing extensive program logic.

### 1.1.9 Pseudocode

[DIRECTLY IN NOTES]
Definition:
Pseudocode is an informal, language-independent representation of an algorithm using structured English-like statements.
It describes program logic without following the strict syntax of a particular programming language.
Common pseudocode conventions
Keyword
Purpose
START
Begin algorithm
STOP
End algorithm
INPUT
Accept data
OUTPUT
Display data
SET
Assign value
IF
Conditional statement
ELSE
Alternative branch
WHILE
Repetition
FOR
Count-controlled repetition
RETURN
Return a result
Example:
START INPUT N IF N > 0 THEN OUTPUT "Positive" ELSE IF N < 0 THEN OUTPUT "Negative" ELSE OUTPUT "Zero" END IF STOP
Algorithm vs Flowchart vs Pseudocode
Algorithm
Flowchart
Pseudocode
Step-by-step instructions
Graphical representation
Structured textual representation
Uses natural language
Uses standard symbols
Uses programming-like statements
Easy to write
Easy to visualise
Easy to convert into code
⚠ Examiner's flag
An algorithm must terminate.
An algorithm must have at least one output.
A flowchart decision symbol must have clearly labelled branches.
Flowchart arrows must show the execution direction.
Pseudocode is not executable C code.
Time complexity describes growth, not exact execution time.

## Chapter 1.2: Structure of a C Program and Memory Layout


### 1.2.1 Introduction to C

[DIRECTLY IN NOTES]
C is a general-purpose, procedural and structured programming language developed by Dennis Ritchie at Bell Laboratories around 1972.
It is widely used in:
Operating systems.
Embedded systems.
Compilers.
Device drivers.
System utilities.
Database systems.
Important characteristics of C
Structured programming.
Portability.
Efficient execution.
Rich operators.
Pointer support.
Dynamic memory allocation.
Recursion.
Modular programming.

### 1.2.2 Structure of a C Program

[DIRECTLY IN NOTES]
A C program generally contains the following sections:
Documentation section.
Preprocessor directives.
Definition section.
Global declaration section.
Main function.
Local declarations.
Executable statements.
User-defined functions.
General syntax
/* Documentation section */ #include <stdio.h> #define MAX 100 int globalVariable = 10; /* Function declaration */ void display(void); int main(void) { /* Local declaration */ int number = 20; /* Executable statement */ printf("Number = %d\n", number); display(); return 0; } /* Function definition */ void display(void) { printf("Hello from function\n"); }
Explanation
Component
Purpose
#include
Includes header files
#define
Defines macros
Global declaration
Declares globally accessible identifiers
main()
Program entry point
Local declaration
Declares local variables
Statements
Perform operations
return 0
Indicates successful termination

### 1.2.3 Preprocessor Directives

[DIRECTLY IN NOTES]
Preprocessor directives are instructions processed before the actual compilation stage.
They begin with the # symbol.
Examples:
#include <stdio.h> #include <stdlib.h> #define PI 3.14159 #define MAX 100
Common directives:
Directive
Purpose
#include
Header inclusion
#define
Macro definition
#undef
Undefine a macro
#ifdef
Conditional compilation
#ifndef
Compile if macro is not defined
#if
Conditional compilation
#else
Alternative preprocessing branch
#endif
End conditional block

### 1.2.4 Compilation and Execution Process

[DIRECTLY IN NOTES]
A C program passes through several stages before execution.
```text
Compilation Pipeline:
Source Code (main.c)
        |
        v
   Preprocessor
        |
        v
Expanded Source (main.i)
        |
        v
     Compiler
        |
        v
Assembly Code (main.s)
        |
        v
    Assembler
        |
        v
 Object Code (main.o)
        |
        v
      Linker
        |
        v
 Executable (main.exe / a.out)
        |
        v
      Loader
        |
        v
    Execution
```
1. Preprocessor
Processes directives such as #include and #define.
2. Compiler
Translates the preprocessed C source into assembly language or an intermediate representation.
3. Assembler
Converts assembly language into object code.
4. Linker
Combines object files and required library code to produce an executable.
5. Loader
Loads the executable into memory so the operating system can execute it.
Example GCC commands:
gcc -E program.c -o program.i gcc -S program.i -o program.s gcc -c program.s -o program.o gcc program.o -o program ./program
⚠ Examiner's flag
Compilation and linking are separate stages. A source file can compile successfully but fail during linking because of an undefined function or missing definition.

### 1.2.5 Memory Layout of a C Program

[RESTORED STANDARD EQUATION / CODE]
Definition:
Memory layout describes how a running process organises its memory into different logical regions.
A conventional process memory layout contains:
Text segment.
Initialized data segment.
Uninitialized data segment.
Heap.
Stack.
Memory layout diagram
HIGH MEMORY ADDRESSES +----------------------+ | | | STACK | | Local variables | | Function parameters | | Return information | | | | | v | | | | ^ | | | | | HEAP | | Dynamic allocations | | malloc / calloc | | | +----------------------+ | | | .bss | | Uninitialized static | | and global variables | +----------------------+ | | | .data | | Initialized global | | and static variables | +----------------------+ | | | TEXT SEGMENT | | Executable code | +----------------------+ LOW MEMORY ADDRESSES
This is a conceptual layout. Actual process layouts depend on the operating system, executable format, architecture and address-space randomisation.
1. Text Segment
Stores executable machine instructions.
Characteristics:
Contains compiled program code.
Commonly read-only.
Shared code pages may be possible between processes.
2. Initialized Data Segment (.data)
Stores initialized global and static variables.
Example:
int globalValue = 100; int main(void) { static int count = 10; return 0; }
3. Uninitialized Data Segment (.bss)
Stores uninitialized or zero-initialized static-storage-duration variables.
Example:
int globalValue; static int counter; int main(void) { return 0; }
These variables are initialized to zero before program execution begins.
4. Heap Segment
Used for dynamic memory allocation.
Common functions:
malloc()
calloc()
realloc()
free()
5. Stack Segment
Typically stores automatic local variables, function parameters and function-call information.
Example:
void calculate(void) { int a = 10; int b = 20; } int main(void) { calculate(); return 0; }
The local variables normally have automatic storage duration.
Comparison table
Segment
Stores
Typical allocation
Text
Instructions
Program loading
.data
Initialized static/global variables
Static storage
.bss
Zero-initialized static/global variables
Static storage
Heap
Dynamic objects
Runtime
Stack
Automatic local objects and call information
Function calls
⚠ Examiner's flag
Global variables are not automatically stored on the stack.
Local variables are not necessarily stored on the stack in every implementation.
malloc() allocates memory from the dynamic allocation area, conventionally called the heap.
Heap and stack growth directions are implementation-dependent.
The C language standard specifies storage duration and allocation behaviour, not a mandatory physical memory layout.

## Chapter 1.3: Data Types, Variables, Input/Output and Operators


### 1.3.1 Data Types in C

[DIRECTLY IN NOTES]
Definition:
A data type specifies the type of value a variable can store and the operations that can be performed on it.
C provides several fundamental data types.
Data type
Purpose
Example
int
Integer values
int age = 18;
char
Character values
char grade = 'A';
float
Single-precision floating point
float x = 3.14f;
double
Double-precision floating point
double pi = 3.14159;
void
No value or generic function return
void display(void);
Typical sizes
The following are common values, not universal guarantees.
Data type
Common size
char
1 byte
int
4 bytes
float
4 bytes
double
8 bytes
long long
8 bytes
Use sizeof to determine actual sizes on a particular system.
#include <stdio.h> int main(void) { printf("char = %zu bytes\n", sizeof(char)); printf("int = %zu bytes\n", sizeof(int)); printf("float = %zu bytes\n", sizeof(float)); printf("double = %zu bytes\n", sizeof(double)); return 0; }

### 1.3.2 Type Modifiers

[DIRECTLY IN NOTES]
Type modifiers modify the range or properties of fundamental integer types.
Common modifiers:
signed
unsigned
short
long
Examples:
short int a = 100; unsigned int b = 200; long int c = 50000L; long long int d = 9000000000LL; signed char e = -10;
Typical integer ranges
Type
Typical range
signed char
-128 to 127
unsigned char
0 to 255
short
-32768 to 32767
unsigned short
0 to 65535
int
Commonly -2147483648 to 2147483647
unsigned int
Commonly 0 to 4294967295
Actual ranges depend on the implementation.

### 1.3.3 Variables

[DIRECTLY IN NOTES]
Definition:
A variable is a named object associated with a memory location that stores a value during program execution.
Syntax:
data_type variable_name;
Examples:
int age; float salary; char grade; double distance;
Variable initialization:
int age = 18; float marks = 95.5f; char grade = 'A';
Multiple declarations:
int a, b, c;
Rules for naming variables
Must begin with a letter or underscore.
Cannot begin with a digit.
Cannot contain spaces.
Cannot be a C keyword.
Identifiers are case-sensitive.
Valid:
int age; int student_marks; int _count; int number1;
Invalid:
int 1number; int student marks; int float;

### 1.3.4 Constants

Definition:
A constant is a value that does not change during the relevant execution or compilation context.
Types of constants
1. Integer constants
int a = 100;
2. Floating-point constants
float pi = 3.14f;
3. Character constants
char grade = 'A';
4. String literals
char name[] = "Chandigarh";
5. Const-qualified variables
const int MAX = 100;
6. Macro constants
#define PI 3.14159
Difference:
const
#define
C language declaration
Preprocessor directive
Has a declared type
Textual substitution
Follows scope rules
Macro replacement follows preprocessing rules
Can be inspected by debugger
Usually no independent runtime object

### 1.3.5 Input and Output Functions

[DIRECTLY IN NOTES]
C provides standard input/output functions through the header file:
#include <stdio.h>
printf()
Used to display formatted output.
Syntax:
printf("format string", arguments);
Example:
int age = 18; printf("Age = %d\n", age);
scanf()
Used to read formatted input.
Syntax:
scanf("format string", &variable);
Example:
int age; scanf("%d", &age);
Format specifiers
Specifier
Meaning
%d
Signed decimal integer
%i
Signed integer input, also accepts other bases
%u
Unsigned decimal integer
%f
Floating-point output and float input
%lf
double input with scanf
%c
Character
%s
String
%p
Pointer address
%ld
Long integer
%lld
Long long integer
%x
Hexadecimal
%o
Octal
%zu
size_t
Important distinction
For printf():
float a = 10.5f; double b = 20.5; printf("%f\n", a); printf("%f\n", b);
For scanf():
float a; double b; scanf("%f", &a); scanf("%lf", &b);
Escape sequences
Escape sequence
Meaning
\n
New line
\t
Horizontal tab
\b
Backspace
\r
Carriage return
\\
Backslash
\'
Single quotation mark
\"
Double quotation mark
\0
Null character
\a
Alert character
getchar()
Reads one character from standard input.
char ch; ch = getchar();
putchar()
Displays one character.
putchar('A');
puts()
Displays a string followed by a newline.
puts("Hello World");
gets()
Historically used to read a line of text.
char name[30]; /* Do not use gets() in modern C. */
gets() was removed from the C standard because it cannot limit the number of characters read and can cause buffer overflows.
Use fgets() instead.
#include <stdio.h> int main(void) { char name[30]; printf("Enter your name: "); if (fgets(name, sizeof(name), stdin) != NULL) { printf("Name: %s", name); } return 0; }
⚠ Examiner's flag
Use & with ordinary scalar variables in scanf().
Do not use & with a character array when reading a string using %s.
%lf is required for reading a double using scanf().
gets() is unsafe and removed from modern C.
%s stops reading at whitespace.
Always ensure the destination buffer is large enough.

## Chapter 1.4: Operators and Expressions


### 1.4.1 Operators

[DIRECTLY IN NOTES]
Definition:
An operator is a symbol that specifies an operation to be performed on one or more operands.
Example:
int result = a + b;
Here:
+ is the operator.
a and b are operands.

### 1.4.2 Arithmetic Operators

Operator
Meaning
Example
+
Addition
a + b
-
Subtraction
a - b
*
Multiplication
a * b
/
Division
a / b
%
Modulus
a % b
Example:
#include <stdio.h> int main(void) { int a = 17; int b = 5; printf("Addition = %d\n", a + b); printf("Subtraction = %d\n", a - b); printf("Multiplication = %d\n", a * b); printf("Division = %d\n", a / b); printf("Remainder = %d\n", a % b); return 0; }
Output:
Addition = 22 Subtraction = 12 Multiplication = 85 Division = 3 Remainder = 2

### 1.4.3 Relational Operators

Used to compare two operands.
Operator
Meaning
==
Equal to
!=
Not equal to
>
Greater than
<
Less than
>=
Greater than or equal
<=
Less than or equal
Example:
int a = 10; int b = 20; printf("%d", a < b);
Output:
1
In C, a comparison expression produces an integer result of either zero or one.

### 1.4.4 Logical Operators

| Operator | Meaning |
|---|---|
| && | Logical AND |
| || | Logical OR |
| ! | Logical NOT |
Truth table:
A
B
A && B
A || B
0
0
0
0
0
1
0
1
1
0
0
1
1
1
1
1
NOT:
A
!A
0
1
1
0
Example:
int age = 20; int hasID = 1; if (age >= 18 && hasID == 1) { printf("Eligible\n"); }
Short-circuit evaluation
For logical AND, if the first operand evaluates to false, the second operand is not evaluated.
For logical OR, if the first operand evaluates to true, the second operand is not evaluated.

### 1.4.5 Assignment Operators

Operator
Equivalent expression
=
a = b
+=
a = a + b
-=
a = a - b
*=
a = a * b
/=
a = a / b
%=
a = a % b
Example:
int a = 10; a += 5; a *= 2; printf("%d", a);
Output:
30

### 1.4.6 Increment and Decrement Operators

[DIRECTLY IN NOTES]
Increment increases a variable by one.
Decrement decreases a variable by one.
Pre-increment
++x;
The increment operation is performed before the new value is used.
Post-increment
x++;
The expression produces the old value; the increment is performed as part of evaluating the expression.
Example:
#include <stdio.h> int main(void) { int x = 5; int a, b; a = ++x; printf("After pre-increment:\n"); printf("x = %d, a = %d\n", x, a); x = 5; b = x++; printf("After post-increment:\n"); printf("x = %d, b = %d\n", x, b); return 0; }
Output:
After pre-increment: x = 6, a = 6 After post-increment: x = 6, b = 5
Dry-run table:
Expression
Initial x
Assigned value
Final x
a = ++x
5
6
6
b = x++
5
5
6
⚠ Examiner's flag
Avoid expressions that modify the same scalar object multiple times without a defined sequencing relationship.
For example:
int i = 5; /* Undefined behavior */ printf("%d %d", i++, i++);
Do not assume a left-to-right evaluation order for function arguments.

### 1.4.7 Bitwise Operators

[DIRECTLY IN NOTES]
Bitwise operators perform operations on the individual bits of integer operands.
Operator
Meaning
&
Bitwise AND
\|
Bitwise OR
^
Bitwise XOR
~
Bitwise complement
<<
Left shift
>>
Right shift
Example:
Let:
\[ A=5=0101_2 \]
\[ B=3=0011_2 \]
Bitwise AND
\[ 0101 \mathbin{\&} 0011=0001 \]
Result:
\[ 1 \]
Bitwise OR
\[ 0101 \mathbin{|} 0011=0111 \]
Result:
\[ 7 \]
Bitwise XOR
\[ 0101 \oplus 0011=0110 \]
Result:
\[ 6 \]
Left shift
\[ 5 \ll 1=10 \]
Right shift
\[ 5 \gg 1=2 \]
Example program:
#include <stdio.h> int main(void) { unsigned int a = 5; unsigned int b = 3; printf("AND = %u\n", a & b); printf("OR = %u\n", a | b); printf("XOR = %u\n", a ^ b); printf("Left shift = %u\n", a << 1); printf("Right shift = %u\n", a >> 1); return 0; }
Output:
AND = 1 OR = 7 XOR = 6 Left shift = 10 Right shift = 2

### 1.4.8 Conditional or Ternary Operator

[DIRECTLY IN NOTES]
The conditional operator is a shorthand alternative to a simple if-else statement.
Syntax:
condition ? expression1 : expression2;
If the condition is true, expression1 is evaluated. Otherwise, expression2 is evaluated.
Example:
#include <stdio.h> int main(void) { int a = 10; int b = 20; int maximum = (a > b) ? a : b; printf("Maximum = %d\n", maximum); return 0; }
Output:
Maximum = 20

### 1.4.9 sizeof Operator

The sizeof operator determines the size in bytes of a type or object.
Syntax:
sizeof(expression) sizeof(type)
Example:
#include <stdio.h> int main(void) { int a; printf("Size of int = %zu\n", sizeof(int)); printf("Size of a = %zu\n", sizeof(a)); return 0; }

### 1.4.10 Comma Operator

The comma operator evaluates its left operand first, discards its value and then evaluates its right operand.
Example:
#include <stdio.h> int main(void) { int a, b, c; c = (a = 5, b = 10, a + b); printf("%d", c); return 0; }
Output:
15

### 1.4.11 Type Conversion and Typecasting

[DIRECTLY IN NOTES]
Type conversion changes a value from one data type to another.
Two major categories:
1. Implicit Type Conversion
Performed automatically by the compiler.
Example:
int a = 10; float b = 2.5f; float result = a + b;
The integer value is converted to floating point during the usual arithmetic conversions.
2. Explicit Type Conversion
Performed by the programmer using a cast operator.
Syntax:
(type) expression
Example:
#include <stdio.h> int main(void) { int a = 5; int b = 2; float result = (float)a / b; printf("%.2f\n", result); return 0; }
Output:
2.50
Without the cast, integer division would produce 2.

### 1.4.12 Operator Precedence and Associativity

[RESTORED STANDARD EQUATION / CODE]
Operator precedence determines which operators bind more tightly.
Associativity determines grouping when operators of the same precedence occur together.
Priority
Operators
Associativity
1
(), [], ., ->, postfix ++, postfix --
Left to right
2
Prefix ++, prefix --, !, ~, unary +, unary -, *, &, sizeof, casts
Right to left
3
*, /, %
Left to right
4
+, -
Left to right
5
<<, >>
Left to right
6
<, <=, >, >=
Left to right
7
==, !=
Left to right
8
&
Left to right
9
^
Left to right
10
\|
Left to right
11
&&
Left to right
12
\|\|
Left to right
13
?:
Right to left
14
Assignment operators
Right to left
15
,
Left to right
Example 1
int result = 10 + 5 * 2;
Multiplication has higher precedence.
\[ result=10+10=20 \]
Example 2
int result = (10 + 5) * 2;
Parentheses are evaluated first.
\[ result=15\times2=30 \]
Example 3
int a = 10, b = 20, c = 30; a = b = c;
Assignment is right-associative.
\[ a=(b=c) \]
Final values:
\[ a=30,\quad b=30,\quad c=30 \]
⚠ Examiner's flag
= is assignment, while == is comparison.
% is defined for integer operands, not floating-point operands.
Integer division discards the fractional part.
Bitwise operators and logical operators are different.
Parentheses should be used to clarify complicated expressions.
Precedence does not determine the evaluation order of every operand.

## Chapter 1.5: Decision Control Structures


### 1.5.1 Decision Making

[DIRECTLY IN NOTES]
Definition:
Decision control structures allow a program to select a particular execution path depending on whether a condition evaluates to true or false.
C provides:
Simple if.
if-else.
Nested if-else.
else-if ladder.
switch.
goto.

### 1.5.2 Simple if Statement

Syntax:
if (condition) { statements; }
Working:
Condition is evaluated.
If nonzero, the body executes.
If zero, the body is skipped.
Example:
#include <stdio.h> int main(void) { int age = 20; if (age >= 18) { printf("Eligible to vote\n"); } return 0; }

### 1.5.3 if-else Statement

Syntax:
if (condition) { statements1; } else { statements2; }
Example:
#include <stdio.h> int main(void) { int number; printf("Enter a number: "); scanf("%d", &number); if (number % 2 == 0) { printf("Even\n"); } else { printf("Odd\n"); } return 0; }
Dry run:
Number
Remainder
Condition
Output
8
0
True
Even
7
1
False
Odd

### 1.5.4 Nested if-else

An if statement inside another if statement is called nested decision making.
Example:
#include <stdio.h> int main(void) { int number; printf("Enter number: "); scanf("%d", &number); if (number >= 0) { if (number == 0) { printf("Zero\n"); } else { printf("Positive\n"); } } else { printf("Negative\n"); } return 0; }

### 1.5.5 else-if Ladder

Used when multiple conditions must be checked sequentially.
Syntax:
if (condition1) { statements1; } else if (condition2) { statements2; } else if (condition3) { statements3; } else { default_statements; }
Example: Grade calculation.
#include <stdio.h> int main(void) { int marks; printf("Enter marks: "); scanf("%d", &marks); if (marks >= 90) { printf("Grade A\n"); } else if (marks >= 80) { printf("Grade B\n"); } else if (marks >= 70) { printf("Grade C\n"); } else if (marks >= 60) { printf("Grade D\n"); } else { printf("Grade F\n"); } return 0; }
Dry run:
Marks
First satisfied condition
Output
95
marks >= 90
A
85
marks >= 80
B
75
marks >= 70
C
65
marks >= 60
D
45
Else
F

### 1.5.6 switch Statement

[DIRECTLY IN NOTES]
Definition:
The switch statement is a multi-way decision-making construct that selects one execution path according to the value of an integer-compatible controlling expression.
Syntax:
switch (expression) { case constant1: statements; break; case constant2: statements; break; default: statements; }
Working rules
The controlling expression is evaluated.
Its value is compared with case labels.
Matching case statements execute.
break terminates the switch.
Without break, execution falls through into subsequent case bodies.
default executes if no case matches and control reaches it.
Example:
#include <stdio.h> int main(void) { int choice; printf("1. Add\n"); printf("2. Subtract\n"); printf("3. Multiply\n"); printf("Enter choice: "); scanf("%d", &choice); switch (choice) { case 1: printf("Addition selected\n"); break; case 2: printf("Subtraction selected\n"); break; case 3: printf("Multiplication selected\n"); break; default: printf("Invalid choice\n"); } return 0; }
Fall-through mechanism
Example:
#include <stdio.h> int main(void) { int number = 2; switch (number) { case 1: printf("One\n"); case 2: printf("Two\n"); case 3: printf("Three\n"); break; default: printf("Other\n"); } return 0; }
Output:
Two Three
Explanation:
Execution begins at case 2. Since there is no break after case 2, execution continues into case 3.
Important switch rules
Case labels must be integer constant expressions.
Duplicate case values are not permitted.
Floating-point values cannot be used as case labels.
A break exits the nearest enclosing switch or loop.
The default label is optional.
A switch statement can contain multiple case labels for the same statement.

### 1.5.7 goto Statement

[DIRECTLY IN NOTES]
Definition:
The goto statement transfers program control directly to a labelled statement within the same function.
Syntax:
goto label; /* Other statements */ label: statement;
Example:
#include <stdio.h> int main(void) { int number = 1; start: printf("%d\n", number); number++; if (number <= 5) { goto start; } return 0; }
Output:
1 2 3 4 5
Advantages
Can simplify certain error-handling paths.
Can be used to exit deeply nested constructs.
Disadvantages
Makes program flow difficult to understand.
Can create difficult-to-maintain code.
Can introduce accidental infinite loops.
Structured alternatives such as loops, functions and break are generally preferred.

### 1.5.8 Comparison of Decision Structures

Structure
Purpose
Number of branches
if
Execute if true
One
if-else
Select between two alternatives
Two
Nested if
Decision within decision
Multiple
else-if ladder
Check multiple conditions
Multiple
switch
Select based on matching constant value
Multiple
goto
Transfer to labelled statement
Unconditional transfer
⚠ Examiner's flag
Do not put a semicolon immediately after an if condition unless an empty statement is intended.
Use braces to avoid dangling-else confusion.
Remember that switch supports fall-through.
Do not forget break when fall-through is not intended.
Do not use floating-point case labels.
goto labels must be in the same function.
A condition evaluating to zero is false; a nonzero value is true.
UNIT 1: EXAMINATION CHECKPOINT
Important theory questions
Define problem solving and explain its five phases.
Define an algorithm and explain its five characteristics.
Differentiate between algorithm, pseudocode and flowchart.
Draw and explain standard flowchart symbols.
Explain time and space complexity.
Differentiate between best, average and worst-case complexity.
Explain the structure of a C program with an example.
Explain the stages of compilation and execution.
Draw and explain the memory layout of a C program.
Explain fundamental C data types and modifiers.
Differentiate between const and #define.
Explain formatted input and output functions.
Explain arithmetic, relational and logical operators.
Differentiate between pre-increment and post-increment.
Explain bitwise operators with examples.
Explain implicit and explicit type conversion.
Explain operator precedence and associativity.
Differentiate between if-else and switch.
Explain fall-through in a switch statement.
Explain the goto statement and its limitations.
Important programming questions
No.
Program
Main concept
1
Sum of two numbers
Input/output
2
Area of a circle
Arithmetic
3
Even or odd
Decision making
4
Largest of two numbers
if-else
5
Largest of three numbers
Nested if
6
Grade calculator
else-if ladder
7
Simple calculator
switch
8
Leap year checker
Logical operators
9
Positive, negative or zero
Nested decisions
10
Demonstrate pre/post increment
Increment operators

This part covers all five chapters of Unit 2, with formal definitions, syntax, working principles, memory diagrams, algorithms, C implementations, dry-run tables, complexity analysis and examination traps.

**Source coverage labels**

- **[DIRECTLY IN NOTES]** Explicitly covered in the CU course material.
- **[RESTORED STANDARD EQUATION / CODE]** Standard C formulations and equations included to complete or clarify the material.
- **[EXAM SUPPORT]** Additional solved examples, tracing and examination-oriented explanations.



# UNIT 2: LOOPING, ARRAYS, STRINGS, FUNCTIONS & RECURSION

## CHAPTER 2.1: LOOPING CONTROL STRUCTURES



### 2.1.1 Introduction to Looping


[DIRECTLY IN NOTES]

**Definition:**

Looping is a control structure that repeatedly executes a block of statements as long as a specified condition is satisfied.

A loop reduces code repetition and makes programs shorter, more efficient and easier to maintain.

**Applications of looping:**

1. Printing a sequence of numbers.
2. Calculating factorials.
3. Finding the sum of digits.
4. Reversing a number.
5. Searching and sorting arrays.
6. Processing matrices.
7. Generating multiplication tables.

There are three fundamental looping statements in C:

1. `while` loop.
2. `for` loop.
3. `do-while` loop.


### 2.1.2 Components of a Loop


Every conventional loop involves three major components.

**1. Initialization**

Establishes the starting value of the loop-control variable.

Example:

```
int i = 1;
```

**2. Condition**

Determines whether the loop should execute.

Example:

```
i <= 10
```

**3. Update**

Changes the loop-control variable to eventually terminate the loop.

Example:

```
i++;
```

**General looping flow**

```
          START
            |
            v
      Initialization
            |
            v
       Condition?
        /      \
      YES       NO
       |         |
       v         |
    Statements   |
       |         |
       v         |
     Update      |
       |         |
       +---------+
                 |
                 v
               STOP
```


### 2.1.3 Entry-Controlled and Exit-Controlled Loops


[DIRECTLY IN NOTES]

Loops are classified according to when their conditions are evaluated.

### Entry-Controlled Loops

The condition is checked before executing the loop body.

Examples:

- `for`
- `while`

If the condition is false initially, the loop body does not execute.

### Exit-Controlled Loop

The condition is checked after executing the loop body.

Example:

\- `do-while`

The loop body executes at least once, regardless of the initial condition.

**Comparison**

| Feature                   | while            | for              | do-while        |
| ------------------------- | ---------------- | ---------------- | --------------- |
| Control                   | Entry-controlled | Entry-controlled | Exit-controlled |
| Condition checking        | Before body      | Before body      | After body      |
| Minimum executions        | 0                | 0                | 1               |
| Initialization            | Usually outside  | In loop header   | Usually outside |
| Update                    | Usually inside   | In loop header   | Usually inside  |
| Semicolon after condition | No               | No               | Yes             |


### 2.1.4 while Loop


[DIRECTLY IN NOTES]

**Definition:**

A `while` loop repeatedly executes a block of statements while the specified condition evaluates to true.

**Syntax:**

```
initialization;

while (condition)
{
    statements;

    update;
}
```

**Working rules**

1. Initialization is performed.
2. The condition is evaluated.
3. If true, the loop body executes.
4. The update statement executes.
5. Control returns to the condition.
6. If false, the loop terminates.

**Flowchart**

```
         START
           |
           v
      i = 1
           |
           v
       i <= 5?
       /     \
     YES      NO
      |        |
      v        |
  Print i      |
      |        |
      v        |
    i = i + 1  |
      |        |
      +--------+
               |
               v
              STOP
```

### Example 1: Print numbers from 1 to 5

[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    int i = 1;

    // Repeat while i is less than or equal to 5
    while (i <= 5)
    {
        printf("%d\n", i);

        // Increase the loop variable
        i++;
    }

    return 0;
}
```

Output:

```
1
2
3
4
5
```

**Dry-run table**

| Iteration | i before condition | Condition | Output | i after update |
| --------- | ------------------ | --------- | ------ | -------------- |
| 1         | 1                  | True      | 1      | 2              |
| 2         | 2                  | True      | 2      | 3              |
| 3         | 3                  | True      | 3      | 4              |
| 4         | 4                  | True      | 4      | 5              |
| 5         | 5                  | True      | 5      | 6              |
| 6         | 6                  | False     | None   | 6              |

**Complexity**

For \\(n\\) iterations:

\\[ T(n)=O(n) \\]

\\[ S(n)=O(1) \\]

### Example 2: Sum of first N natural numbers

```
#include <stdio.h>

int main(void)
{
    int n, i = 1;
    long long sum = 0;

    printf("Enter N: ");
    scanf("%d", &n);

    while (i <= n)
    {
        sum += i;
        i++;
    }

    printf("Sum = %lld\n", sum);

    return 0;
}
```

For \\(n=5\\):

\\[ S=1+2+3+4+5=15 \\]

Dry run:

| Iteration | i | sum before | sum after |
| --------- | - | ---------- | --------- |
| 1         | 1 | 0          | 1         |
| 2         | 2 | 1          | 3         |
| 3         | 3 | 3          | 6         |
| 4         | 4 | 6          | 10        |
| 5         | 5 | 10         | 15        |

Complexity:

\\[ T(n)=O(n) \\]

\\[ S(n)=O(1) \\]


### 2.1.5 for Loop


[DIRECTLY IN NOTES]

**Definition:**

A `for` loop is an entry-controlled looping statement in which initialization, condition checking and updating are generally written in one loop header.

**Syntax:**

```
for (initialization; condition; update)
{
    statements;
}
```

**Working rules**

1. Initialization executes once.
2. Condition is checked.
3. If true, the loop body executes.
4. Update executes.
5. Condition is checked again.
6. The process continues until the condition becomes false.

### Example 1: Print numbers from 1 to 10

```
#include <stdio.h>

int main(void)
{
    int i;

    for (i = 1; i <= 10; i++)
    {
        printf("%d\n", i);
    }

    return 0;
}
```

Output:

```
1
2
3
4
5
6
7
8
9
10
```

### Example 2: Multiplication table

[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    int number;

    printf("Enter a number: ");
    scanf("%d", &number);

    for (int i = 1; i <= 10; i++)
    {
        printf("%d x %d = %d\n",
               number, i, number * i);
    }

    return 0;
}
```

For input \\(5\\):

```
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
```

Dry-run table:

| Iteration | i  | Calculation | Result |
| --------- | -- | ----------- | ------ |
| 1         | 1  | 5 × 1       | 5      |
| 2         | 2  | 5 × 2       | 10     |
| 3         | 3  | 5 × 3       | 15     |
| 4         | 4  | 5 × 4       | 20     |
| 5         | 5  | 5 × 5       | 25     |
| 6         | 6  | 5 × 6       | 30     |
| 7         | 7  | 5 × 7       | 35     |
| 8         | 8  | 5 × 8       | 40     |
| 9         | 9  | 5 × 9       | 45     |
| 10        | 10 | 5 × 10      | 50     |

Complexity:

\\[ T(n)=O(n) \\]

\\[ S(n)=O(1) \\]

### Example 3: Factorial using a for loop

```
#include <stdio.h>

int main(void)
{
    int n;
    unsigned long long factorial = 1;

    printf("Enter a non-negative integer: ");
    scanf("%d", &n);

    if (n < 0)
    {
        printf("Factorial is not defined for negative integers.\n");
        return 1;
    }

    for (int i = 1; i <= n; i++)
    {
        factorial *= i;
    }

    printf("Factorial = %llu\n", factorial);

    return 0;
}
```

Mathematical definition:

\\[ n!=n\times(n-1)\times(n-2)\times\cdots\times1 \\]

Special case:

\\[ 0!=1 \\]

For \\(n=5\\):

\\[ 5!=5\times4\times3\times2\times1=120 \\]

Dry run:

| i | Previous factorial | Operation | New factorial |
| - | ------------------ | --------- | ------------- |
| 1 | 1                  | 1 × 1     | 1             |
| 2 | 1                  | 1 × 2     | 2             |
| 3 | 2                  | 2 × 3     | 6             |
| 4 | 6                  | 6 × 4     | 24            |
| 5 | 24                 | 24 × 5    | 120           |

Complexity:

\\[ T(n)=O(n) \\]

\\[ S(n)=O(1) \\]


### 2.1.6 do-while Loop


[DIRECTLY IN NOTES]

**Definition:**

A `do-while` loop is an exit-controlled loop that executes the loop body first and checks the condition afterward.

**Syntax:**

```
do
{
    statements;
}
while (condition);
```

**Important:** The semicolon after the `while` condition is mandatory.

**Working rules**

1. Execute the body.
2. Evaluate the condition.
3. If true, repeat.
4. If false, terminate.

### Example 1: Print numbers from 1 to 5

```
#include <stdio.h>

int main(void)
{
    int i = 1;

    do
    {
        printf("%d\n", i);
        i++;
    }
    while (i <= 5);

    return 0;
}
```

### Example 2: Demonstrate minimum one execution

```
#include <stdio.h>

int main(void)
{
    int i = 10;

    do
    {
        printf("Executed once\n");
        i++;
    }
    while (i < 5);

    return 0;
}
```

Output:

```
Executed once
```

Even though the condition is initially false, the loop body executes once.

**Dry run**

| Step    | i  | Condition   | Result        |
| ------- | -- | ----------- | ------------- |
| Initial | 10 | Not checked | Enter body    |
| Body    | 10 | Not checked | Print message |
| Update  | 11 | Not checked | Increment     |
| Check   | 11 | False       | Terminate     |

### Example 3: Menu-driven program

[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    int choice;

    do
    {
        printf("\n--- MENU ---\n");
        printf("1. Hello\n");
        printf("2. Display message\n");
        printf("3. Exit\n");

        printf("Enter choice: ");
        scanf("%d", &choice);

        switch (choice)
        {
            case 1:
                printf("Hello!\n");
                break;

            case 2:
                printf("Welcome to C programming.\n");
                break;

            case 3:
                printf("Exiting...\n");
                break;

            default:
                printf("Invalid choice.\n");
        }

    }
    while (choice != 3);

    return 0;
}
```


### 2.1.7 Nested Loops


[DIRECTLY IN NOTES]

**Definition:**

A nested loop is a loop placed inside another loop.

The inner loop executes completely for every iteration of the outer loop, unless control is transferred out of it.

**General syntax**

```
for (initialization1; condition1; update1)
{
    for (initialization2; condition2; update2)
    {
        statements;
    }
}
```

### Example 1: Print a rectangle pattern

```
#include <stdio.h>

int main(void)
{
    int rows = 3;
    int columns = 4;

    for (int i = 1; i <= rows; i++)
    {
        for (int j = 1; j <= columns; j++)
        {
            printf("* ");
        }

        printf("\n");
    }

    return 0;
}
```

Output:

```
* * * *
* * * *
* * * *
```

Dry-run table:

| Outer i | Inner j values | Number of inner executions |
| ------- | -------------- | -------------------------- |
| 1       | 1, 2, 3, 4     | 4                          |
| 2       | 1, 2, 3, 4     | 4                          |
| 3       | 1, 2, 3, 4     | 4                          |

Total executions:

\\[ 3\times4=12 \\]

For \\(R\\) rows and \\(C\\) columns:

\\[ T(R,C)=O(RC) \\]

Auxiliary space:

\\[ S(R,C)=O(1) \\]

### Example 2: Right-angled triangle

```
#include <stdio.h>

int main(void)
{
    int n = 5;

    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= i; j++)
        {
            printf("* ");
        }

        printf("\n");
    }

    return 0;
}
```

Output:

```
*
* *
* * *
* * * *
* * * * *
```

Number of executions of the inner statement:

\\[ 1+2+3+\cdots+n \\]

Using the arithmetic-series formula:

\\[ T(n)=\frac{n(n+1)}{2} \\]

Therefore:

\\[ T(n)=O(n^2) \\]

### Example 3: Number pyramid

```
#include <stdio.h>

int main(void)
{
    int n = 5;

    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= i; j++)
        {
            printf("%d ", j);
        }

        printf("\n");
    }

    return 0;
}
```

Output:

```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```


### 2.1.8 Infinite Loops


[DIRECTLY IN NOTES]

**Definition:**

An infinite loop is a loop that continues executing without reaching its termination condition.

Example:

```
while (1)
{
    printf("Running forever\n");
}
```

Another example:

```
for (;;)
{
    printf("Infinite loop\n");
}
```

**Accidental infinite loop**

```
int i = 1;

while (i <= 5)
{
    printf("%d\n", i);

    // Missing i++ causes an infinite loop.
}
```

**Correction**

```
int i = 1;

while (i <= 5)
{
    printf("%d\n", i);
    i++;
}
```

**⚠ Examiner's flag**

- Always check whether the loop-control variable changes.
- Check whether the condition can eventually become false.
- Ensure the update moves the variable toward termination.
- Be careful with unsigned variables because decrementing zero wraps to a large unsigned value.


### 2.1.9 Jump Statements


[DIRECTLY IN NOTES]

Jump statements alter the normal sequential flow of program execution.

Important statements:

1. `break`
2. `continue`
3. `return`
4. `exit()`

### 1. break Statement

Terminates the nearest enclosing loop or switch statement immediately.

Example:

```
#include <stdio.h>

int main(void)
{
    for (int i = 1; i <= 10; i++)
    {
        if (i == 5)
        {
            break;
        }

        printf("%d ", i);
    }

    return 0;
}
```

Output:

```
1 2 3 4
```

Dry run:

| i | Condition i == 5 | Action    |
| - | ---------------- | --------- |
| 1 | False            | Print 1   |
| 2 | False            | Print 2   |
| 3 | False            | Print 3   |
| 4 | False            | Print 4   |
| 5 | True             | Exit loop |

### 2. continue Statement

Skips the remaining statements in the current loop iteration and proceeds to the next iteration.

Example:

```
#include <stdio.h>

int main(void)
{
    for (int i = 1; i <= 5; i++)
    {
        if (i == 3)
        {
            continue;
        }

        printf("%d ", i);
    }

    return 0;
}
```

Output:

```
1 2 4 5
```

Dry run:

| i | Condition i == 3 | Action     |
| - | ---------------- | ---------- |
| 1 | False            | Print 1    |
| 2 | False            | Print 2    |
| 3 | True             | Skip print |
| 4 | False            | Print 4    |
| 5 | False            | Print 5    |

### 3. return Statement

Terminates the current function and optionally returns a value to its caller.

Example:

```
int square(int n)
{
    return n * n;
}
```

For a function returning `void`:

```
void display(void)
{
    printf("Hello\n");
    return;
}
```

### 4. exit() Function

Terminates the entire program.

It is declared in:

```
#include <stdlib.h>
```

Example:

```
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    printf("Before exit\n");

    exit(EXIT_SUCCESS);

    printf("This will not execute\n");
}
```

**Comparison**

| Statement  | Effect                        |
| ---------- | ----------------------------- |
| `break`    | Exits nearest loop or switch  |
| `continue` | Skips current loop iteration  |
| `return`   | Terminates current function   |
| `exit()`   | Terminates the entire program |

**Important difference between break and continue in nested loops**

`break` and `continue` affect only the nearest enclosing loop.

Example:

```
#include <stdio.h>

int main(void)
{
    for (int i = 1; i <= 3; i++)
    {
        for (int j = 1; j <= 3; j++)
        {
            if (j == 2)
            {
                break;
            }

            printf("%d %d\n", i, j);
        }
    }

    return 0;
}
```

Output:

```
1 1
2 1
3 1
```

The inner loop terminates each time, but the outer loop continues.


## CHAPTER 2.2: ONE-DIMENSIONAL AND TWO-DIMENSIONAL ARRAYS



### 2.2.1 Introduction to Arrays


[DIRECTLY IN NOTES]

**Definition:**

An array is a collection of elements of the same data type stored in contiguous memory locations and accessed using a common name and an index.

Arrays allow programmers to store multiple related values under one identifier.

Example:

```
int marks[5] = {80, 75, 90, 85, 95};
```

Instead of declaring five individual variables, one array stores all five values.

**Characteristics of arrays**

1. Store elements of the same type.
2. Elements are stored contiguously.
3. Use zero-based indexing in C.
4. Support direct indexed access.
5. Have a fixed size when declared as ordinary fixed-size arrays.
6. Can be one-dimensional or multidimensional.


### 2.2.2 One-Dimensional Arrays


[DIRECTLY IN NOTES]

**Definition:**

A one-dimensional array is a linear collection of elements arranged sequentially in memory.

**Declaration syntax**

```
data_type array_name[size];
```

Example:

```
int marks[5];
```

This declares an integer array containing five elements.

**Memory representation**

Assume:

```
int arr[5] = {10, 20, 30, 40, 50};
```

Conceptual memory layout, assuming four-byte integers and base address 1000:

```
Array: arr

Index       Value       Address
--------------------------------
arr[0]       10          1000
arr[1]       20          1004
arr[2]       30          1008
arr[3]       40          1012
arr[4]       50          1016
```

The array elements occupy consecutive memory locations.

### Address Calculation Formula

[RESTORED STANDARD EQUATION / CODE]

Let:

- \\(B\\) = Base address.
- \\(i\\) = Array index.
- \\(S\\) = Size of each element in bytes.

For a zero-based one-dimensional array:

\\[ \text{Address}(A[i])=B+i\times S \\]

Example:

Given:

\\[ B=1000 \\]

\\[ i=3 \\]

\\[ S=4 \\]

Then:

\\[ \text{Address}(A[3])=1000+3\times4 \\]

\\[ =1012 \\]

**⚠ Examiner's flag**

C does not automatically check array bounds. Accessing an element outside the valid range results in undefined behavior.

For an array of size \\(n\\), valid indices are:

\\[ 0\leq i\<n \\]


### 2.2.3 Array Initialization


[DIRECTLY IN NOTES]

Arrays can be initialized at declaration time or populated during program execution.

### 1. Complete Initialization

```
int arr[5] = {10, 20, 30, 40, 50};
```

### 2. Partial Initialization

```
int arr[5] = {10, 20};
```

Remaining elements are initialized to zero.

Memory representation:

```
Index       Value
-----------------
0            10
1            20
2             0
3             0
4             0
```

### 3. Size Inference

```
int arr[] = {10, 20, 30, 40};
```

The compiler determines the array size from the initializer.

### 4. Zero Initialization

```
int arr[5] = {0};
```

All elements are initialized to zero.

### 5. Run-Time Initialization

```
#include <stdio.h>

int main(void)
{
    int arr[5];

    for (int i = 0; i < 5; i++)
    {
        printf("Enter element %d: ", i);
        scanf("%d", &arr[i]);
    }

    return 0;
}
```

**Compile-time vs run-time initialization**

| Compile-time initialization    | Run-time initialization            |
| ------------------------------ | ---------------------------------- |
| Values supplied in declaration | Values supplied during execution   |
| Usually uses initializer list  | Usually uses input or calculations |
| Example: `{1, 2, 3}`           | Example: `scanf()` in loop         |


### 2.2.4 Traversal of an Array


[DIRECTLY IN NOTES]

**Definition:**

Array traversal is the process of visiting each element of an array to read, process or display its value.

Example:

```
#include <stdio.h>

int main(void)
{
    int arr[5] = {10, 20, 30, 40, 50};

    for (int i = 0; i < 5; i++)
    {
        printf("arr[%d] = %d\n", i, arr[i]);
    }

    return 0;
}
```

Output:

```
arr[0] = 10
arr[1] = 20
arr[2] = 30
arr[3] = 40
arr[4] = 50
```

Dry run:

| i | arr[i] | Output      |
| - | ------ | ----------- |
| 0 | 10     | arr[0] = 10 |
| 1 | 20     | arr[1] = 20 |
| 2 | 30     | arr[2] = 30 |
| 3 | 40     | arr[3] = 40 |
| 4 | 50     | arr[4] = 50 |

Complexity:

\\[ T(n)=O(n) \\]

\\[ S(n)=O(1) \\]


### 2.2.5 Sum and Average of Array Elements


[EXAM SUPPORT]

Algorithm:

1. Read the number of elements.
2. Read all array elements.
3. Initialize sum to zero.
4. Traverse the array.
5. Add each element to sum.
6. Calculate average.
7. Display results.

C program:

```
#include <stdio.h>

int main(void)
{
    int n;
    long long sum = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    if (n <= 0 || n > 100)
    {
        printf("Invalid array size.\n");
        return 1;
    }

    int arr[100];

    for (int i = 0; i < n; i++)
    {
        printf("Enter element %d: ", i + 1);
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++)
    {
        sum += arr[i];
    }

    double average = (double)sum / n;

    printf("Sum = %lld\n", sum);
    printf("Average = %.2f\n", average);

    return 0;
}
```

Example input:

```
5
10 20 30 40 50
```

Output:

```
Sum = 150
Average = 30.00
```

Dry-run table:

| Index | Element | Previous sum | New sum |
| ----- | ------- | ------------ | ------- |
| 0     | 10      | 0            | 10      |
| 1     | 20      | 10           | 30      |
| 2     | 30      | 30           | 60      |
| 3     | 40      | 60           | 100     |
| 4     | 50      | 100          | 150     |

\\[ \text{Average}=\frac{\text{Sum}}{n} \\]

\\[ =\frac{150}{5}=30 \\]

Complexity:

\\[ T(n)=O(n) \\]

\\[ S(n)=O(n) \\]

The array requires \\(O(n)\\) storage. The additional auxiliary storage is \\(O(1)\\).


### 2.2.6 Linear Search


[DIRECTLY IN NOTES]

**Definition:**

Linear search is a searching technique that checks array elements sequentially until the required element is found or all elements have been examined.

**Algorithm**

```
START

INPUT array A and size n
INPUT key

FOR i = 0 TO n-1

    IF A[i] == key
        OUTPUT position
        STOP

END FOR

OUTPUT "Not Found"

STOP
```

**C implementation**

```
#include <stdio.h>

int main(void)
{
    int arr[100];
    int n, key;
    int position = -1;

    printf("Enter array size: ");
    scanf("%d", &n);

    if (n <= 0 || n > 100)
    {
        printf("Invalid size.\n");
        return 1;
    }

    printf("Enter array elements:\n");

    for (int i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }

    printf("Enter search element: ");
    scanf("%d", &key);

    for (int i = 0; i < n; i++)
    {
        if (arr[i] == key)
        {
            position = i;
            break;
        }
    }

    if (position != -1)
    {
        printf("Element found at index %d\n", position);
    }
    else
    {
        printf("Element not found.\n");
    }

    return 0;
}
```

Example:

Array:

\\[ A=[10,20,30,40,50] \\]

Search key:

\\[ K=30 \\]

Dry-run table:

| Iteration | Index | A[i] | Comparison | Result |
| --------- | ----- | ---- | ---------- | ------ |
| 1         | 0     | 10   | 10 == 30   | False  |
| 2         | 1     | 20   | 20 == 30   | False  |
| 3         | 2     | 30   | 30 == 30   | True   |

Output:

```
Element found at index 2
```

**Complexity analysis**

Best case:

\\[ T(n)=O(1) \\]

Average case:

\\[ T(n)=O(n) \\]

Worst case:

\\[ T(n)=O(n) \\]

Auxiliary space:

\\[ S(n)=O(1) \\]


### 2.2.7 Binary Search


[DIRECTLY IN NOTES]

**Definition:**

Binary search is an efficient searching algorithm that repeatedly divides a sorted search interval into two halves until the required element is found or the interval becomes empty.

**Important prerequisite:** The array must be sorted.

**Algorithm**

1. Initialize `low = 0`.
2. Initialize `high = n - 1`.
3. Calculate the middle index.
4. Compare the middle element with the key.
5. If equal, return the position.
6. If the key is smaller, search the left half.
7. If the key is larger, search the right half.
8. Repeat until the element is found or the interval is empty.

**Formula**

\\[ mid=low+\frac{high-low}{2} \\]

This formulation avoids the potential overflow risk of calculating `(low + high) / 2` with large integer indices.

### C implementation

```
#include <stdio.h>

int main(void)
{
    int arr[100];
    int n, key;

    int low, high, mid;
    int position = -1;

    printf("Enter array size: ");
    scanf("%d", &n);

    if (n <= 0 || n > 100)
    {
        printf("Invalid size.\n");
        return 1;
    }

    printf("Enter sorted array elements:\n");

    for (int i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }

    printf("Enter search key: ");
    scanf("%d", &key);

    low = 0;
    high = n - 1;

    while (low <= high)
    {
        mid = low + (high - low) / 2;

        if (arr[mid] == key)
        {
            position = mid;
            break;
        }
        else if (arr[mid] < key)
        {
            low = mid + 1;
        }
        else
        {
            high = mid - 1;
        }
    }

    if (position != -1)
    {
        printf("Found at index %d\n", position);
    }
    else
    {
        printf("Not found.\n");
    }

    return 0;
}
```

Example:

\\[ A=[10,20,30,40,50,60,70] \\]

Search key:

\\[ K=60 \\]

Dry-run table:

| Iteration | low | high | mid | A[mid] | Decision     |
| --------- | --- | ---- | --- | ------ | ------------ |
| 1         | 0   | 6    | 3   | 40     | Search right |
| 2         | 4   | 6    | 5   | 60     | Found        |

Output:

```
Found at index 5
```

**Complexity**

Best case:

\\[ T(n)=O(1) \\]

Average case:

\\[ T(n)=O(\log n) \\]

Worst case:

\\[ T(n)=O(\log n) \\]

Iterative auxiliary space:

\\[ S(n)=O(1) \\]

**Linear Search vs Binary Search**

| Linear Search                | Binary Search                 |
| ---------------------------- | ----------------------------- |
| Works on unsorted data       | Requires sorted data          |
| Checks elements sequentially | Divides search interval       |
| Worst case \\(O(n)\\)        | Worst case \\(O(\log n)\\)    |
| Simple implementation        | More restrictive prerequisite |

**⚠ Examiner's flag**

Binary search on an unsorted array does not guarantee a correct result.


### 2.2.8 Bubble Sort


[DIRECTLY IN NOTES]

**Definition:**

Bubble sort is a comparison-based sorting algorithm that repeatedly compares adjacent elements and swaps them when they are in the wrong order.

After each complete pass, the largest remaining element reaches its correct position at the end of the unsorted section.

**Algorithm**

```
START

INPUT array A and size n

FOR i = 0 TO n-2

    FOR j = 0 TO n-i-2

        IF A[j] > A[j+1]

            SWAP A[j], A[j+1]

        END IF

    END FOR

END FOR

DISPLAY sorted array

STOP
```

### C implementation

```
#include <stdio.h>

int main(void)
{
    int arr[100];
    int n;

    printf("Enter array size: ");
    scanf("%d", &n);

    if (n <= 0 || n > 100)
    {
        printf("Invalid size.\n");
        return 1;
    }

    printf("Enter elements:\n");

    for (int i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n - 1; i++)
    {
        for (int j = 0; j < n - i - 1; j++)
        {
            if (arr[j] > arr[j + 1])
            {
                int temp = arr[j];

                arr[j] = arr[j + 1];

                arr[j + 1] = temp;
            }
        }
    }

    printf("Sorted array:\n");

    for (int i = 0; i < n; i++)
    {
        printf("%d ", arr[i]);
    }

    printf("\n");

    return 0;
}
```

Example:

Initial array:

\\[ [5,1,4,2,8] \\]

**Pass 1**

| Comparison | Before      | After       |
| ---------- | ----------- | ----------- |
| 5 and 1    | [5,1,4,2,8] | [1,5,4,2,8] |
| 5 and 4    | [1,5,4,2,8] | [1,4,5,2,8] |
| 5 and 2    | [1,4,5,2,8] | [1,4,2,5,8] |
| 5 and 8    | [1,4,2,5,8] | No swap     |

Array after pass 1:

\\[ [1,4,2,5,8] \\]

**Pass 2**

| Comparison | Before      | After       |
| ---------- | ----------- | ----------- |
| 1 and 4    | [1,4,2,5,8] | No swap     |
| 4 and 2    | [1,4,2,5,8] | [1,2,4,5,8] |
| 4 and 5    | [1,2,4,5,8] | No swap     |

Array after pass 2:

\\[ [1,2,4,5,8] \\]

**Pass 3 and Pass 4**

No further changes are required.

Final output:

```
1 2 4 5 8
```

**Complexity**

Standard bubble sort:

Best case without optimization:

\\[ T(n)=O(n^2) \\]

Average case:

\\[ T(n)=O(n^2) \\]

Worst case:

\\[ T(n)=O(n^2) \\]

Auxiliary space:

\\[ S(n)=O(1) \\]

**Optimized Bubble Sort**

[EXAM SUPPORT]

An optimized version stops early when a complete pass performs no swaps.

```
#include <stdio.h>

int main(void)
{
    int arr[] = {1, 2, 3, 4, 5};

    int n = sizeof(arr) / sizeof(arr[0]);

    for (int i = 0; i < n - 1; i++)
    {
        int swapped = 0;

        for (int j = 0; j < n - i - 1; j++)
        {
            if (arr[j] > arr[j + 1])
            {
                int temp = arr[j];

                arr[j] = arr[j + 1];
                arr[j + 1] = temp;

                swapped = 1;
            }
        }

        if (!swapped)
        {
            break;
        }
    }

    for (int i = 0; i < n; i++)
    {
        printf("%d ", arr[i]);
    }

    return 0;
}
```

Optimized best case:

\\[ T(n)=O(n) \\]

Average and worst cases:

\\[ T(n)=O(n^2) \\]


### 2.2.9 Two-Dimensional Arrays


[DIRECTLY IN NOTES]

**Definition:**

A two-dimensional array is a collection of elements organised in rows and columns.

It is commonly used to represent matrices and tabular data.

**Declaration syntax**

```
data_type array_name[rows][columns];
```

Example:

```
int matrix[3][3];
```

This declares a matrix with three rows and three columns.

### Initialization

```
int matrix[2][3] =
{
    {10, 20, 30},
    {40, 50, 60}
};
```

Memory representation:

```
             Column
          0    1    2
        +----+----+----+
Row 0   | 10 | 20 | 30 |
        +----+----+----+
Row 1   | 40 | 50 | 60 |
        +----+----+----+
```

Element access:

```
matrix[0][0] = 10;
matrix[0][1] = 20;
matrix[1][2] = 60;
```


### 2.2.10 Memory Representation of 2D Arrays


[RESTORED STANDARD EQUATION / CODE]

In C, multidimensional arrays are stored in row-major order.

This means elements of the first row are stored consecutively, followed by elements of the second row.

Example:

```
int A[2][3] =
{
    {10, 20, 30},
    {40, 50, 60}
};
```

Conceptual linear memory layout:

```
A[0][0]  A[0][1]  A[0][2]  A[1][0]  A[1][1]  A[1][2]
   10       20       30       40       50       60
```

### Row-Major Address Calculation

Given a two-dimensional array:

\\[ A[R][C] \\]

Let:

- \\(B\\) = Base address.
- \\(i\\) = Row index.
- \\(j\\) = Column index.
- \\(C\\) = Number of columns.
- \\(S\\) = Size of each element.

The row-major address formula is:

\\[ \boxed{ \text{Address}(A[i][j]) = B+[i\times C+j]\times S } \\]

**Solved numerical example**

Given:

\\[ B=1000 \\]

\\[ C=4 \\]

\\[ i=2,\quad j=1 \\]

\\[ S=4\text{ bytes} \\]

Find the address of \\(A[2][1]\\).

Substitution:

\\[ \text{Address}(A[2][1]) = 1000+[2\times4+1]\times4 \\]

\\[ =1000+[8+1]\times4 \\]

\\[ =1000+36 \\]

\\[ \boxed{1036} \\]

### Column-Major Address Calculation

[RESTORED STANDARD EQUATION / CODE]

Column-major storage places elements of each column consecutively.

Although C uses row-major order for its built-in multidimensional arrays, the column-major formula is useful for comparative memory-address examination questions.

For an array with \\(R\\) rows:

\\[ \boxed{ \text{Address}(A[i][j]) = B+[j\times R+i]\times S } \\]

**Solved numerical example**

Given:

\\[ B=2000 \\]

\\[ R=3 \\]

\\[ i=1,\quad j=2 \\]

\\[ S=4 \\]

Then:

\\[ \text{Address}(A[1][2]) = 2000+[2\times3+1]\times4 \\]

\\[ =2000+[7]\times4 \\]

\\[ =2000+28 \\]

\\[ \boxed{2028} \\]

**Row-major vs column-major**

| Row-major                      | Column-major                                |
| ------------------------------ | ------------------------------------------- |
| Stores rows consecutively      | Stores columns consecutively                |
| Used by C                      | Used by several other languages and systems |
| Formula uses number of columns | Formula uses number of rows                 |

**⚠ Examiner's flag**

- C uses row-major storage for multidimensional arrays.
- Do not confuse the number of rows with the number of columns.
- Array indices start from zero.
- The base address represents the first element.
- The element size must be expressed in bytes.
- In C, a two-dimensional array passed to a function must have its later dimensions specified in the parameter type.


### 2.2.11 Matrix Addition


[DIRECTLY IN NOTES]

**Definition:**

Matrix addition is the operation of adding corresponding elements of two matrices having identical dimensions.

If:

\\[ A=[a\_{ij}] \\]

\\[ B=[b\_{ij}] \\]

Then:

\\[ C=A+B \\]

Each element is calculated as:

\\[ c\_{ij}=a\_{ij}+b\_{ij} \\]

**Condition**

Both matrices must have the same number of rows and columns.

### Example

\\[ A= \begin{bmatrix} 1&2\\\ 3&4 \end{bmatrix} \\]

\\[ B= \begin{bmatrix} 5&6\\\ 7&8 \end{bmatrix} \\]

Then:

\\[ C= \begin{bmatrix} 1+5&2+6\\\ 3+7&4+8 \end{bmatrix} \\]

\\[ \boxed{ C= \begin{bmatrix} 6&8\\\ 10&12 \end{bmatrix} } \\]

### C implementation

```
#include <stdio.h>

int main(void)
{
    int A[10][10], B[10][10], C[10][10];
    int rows, cols;

    printf("Enter rows and columns: ");
    scanf("%d %d", &rows, &cols);

    if (rows <= 0 || cols <= 0 ||
        rows > 10 || cols > 10)
    {
        printf("Invalid matrix dimensions.\n");
        return 1;
    }

    printf("Enter first matrix:\n");

    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            scanf("%d", &A[i][j]);
        }
    }

    printf("Enter second matrix:\n");

    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            scanf("%d", &B[i][j]);
        }
    }

    // Add corresponding elements
    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            C[i][j] = A[i][j] + B[i][j];
        }
    }

    printf("Resultant matrix:\n");

    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            printf("%d ", C[i][j]);
        }

        printf("\n");
    }

    return 0;
}
```

**Dry run**

| i | j | A[i][j] | B[i][j] | C[i][j] |
| - | - | ------- | ------- | ------- |
| 0 | 0 | 1       | 5       | 6       |
| 0 | 1 | 2       | 6       | 8       |
| 1 | 0 | 3       | 7       | 10      |
| 1 | 1 | 4       | 8       | 12      |

Complexity:

For an \\(R\times C\\) matrix:

\\[ T(R,C)=O(RC) \\]

Space for result matrix:

\\[ S(R,C)=O(RC) \\]


### 2.2.12 Matrix Multiplication


[DIRECTLY IN NOTES]

**Definition:**

Matrix multiplication is the operation of multiplying rows of the first matrix with columns of the second matrix and adding the resulting products.

**Compatibility condition**

If matrix \\(A\\) has dimensions:

\\[ R_1\times C_1 \\]

and matrix \\(B\\) has dimensions:

\\[ R_2\times C_2 \\]

Multiplication is possible only when:

\\[ \boxed{C_1=R_2} \\]

The resulting matrix has dimensions:

\\[ \boxed{R_1\times C_2} \\]

**Formula**

\\[ C[i][j] = \sum\_{k=0}^{C_1-1} A[i][k]\times B[k][j] \\]

### Example

\\[ A= \begin{bmatrix} 1&2\\\ 3&4 \end{bmatrix} \\]

\\[ B= \begin{bmatrix} 5&6\\\ 7&8 \end{bmatrix} \\]

Calculate:

\\[ C\_{00}=(1\times5)+(2\times7)=19 \\]

\\[ C\_{01}=(1\times6)+(2\times8)=22 \\]

\\[ C\_{10}=(3\times5)+(4\times7)=43 \\]

\\[ C\_{11}=(3\times6)+(4\times8)=50 \\]

Result:

\\[ \boxed{ C= \begin{bmatrix} 19&22\\\ 43&50 \end{bmatrix} } \\]

### C implementation

```
#include <stdio.h>

int main(void)
{
    int A[10][10], B[10][10], C[10][10];

    int r1, c1, r2, c2;

    printf("Enter dimensions of first matrix: ");
    scanf("%d %d", &r1, &c1);

    printf("Enter dimensions of second matrix: ");
    scanf("%d %d", &r2, &c2);

    if (r1 <= 0 || c1 <= 0 ||
        r2 <= 0 || c2 <= 0 ||
        r1 > 10 || c1 > 10 ||
        r2 > 10 || c2 > 10)
    {
        printf("Invalid matrix dimensions.\n");
        return 1;
    }

    // Verify multiplication compatibility
    if (c1 != r2)
    {
        printf("Matrix multiplication is not possible.\n");
        return 1;
    }

    printf("Enter first matrix:\n");

    for (int i = 0; i < r1; i++)
    {
        for (int j = 0; j < c1; j++)
        {
            scanf("%d", &A[i][j]);
        }
    }

    printf("Enter second matrix:\n");

    for (int i = 0; i < r2; i++)
    {
        for (int j = 0; j < c2; j++)
        {
            scanf("%d", &B[i][j]);
        }
    }

    // Initialize and calculate the product
    for (int i = 0; i < r1; i++)
    {
        for (int j = 0; j < c2; j++)
        {
            C[i][j] = 0;

            for (int k = 0; k < c1; k++)
            {
                C[i][j] += A[i][k] * B[k][j];
            }
        }
    }

    printf("Product matrix:\n");

    for (int i = 0; i < r1; i++)
    {
        for (int j = 0; j < c2; j++)
        {
            printf("%d ", C[i][j]);
        }

        printf("\n");
    }

    return 0;
}
```

**Dry-run table for C[0][0]**

| k | A[0][k] | B[k][0] | Product | Running sum |
| - | ------- | ------- | ------- | ----------- |
| 0 | 1       | 5       | 5       | 5           |
| 1 | 2       | 7       | 14      | 19          |

Final:

\\[ C[0][0]=19 \\]

**Complexity**

For dimensions:

\\[ A:R_1\times C_1 \\]

\\[ B:C_1\times C_2 \\]

The conventional algorithm takes:

\\[ T=O(R_1C_1C_2) \\]

For two square matrices of order \\(n\\):

\\[ T(n)=O(n^3) \\]

Result storage:

\\[ S(R_1,C_2)=O(R_1C_2) \\]


### 2.2.13 Matrix Transpose


[DIRECTLY IN NOTES]

**Definition:**

The transpose of a matrix is obtained by interchanging its rows and columns.

If matrix \\(A\\) has dimensions \\(R\times C\\), its transpose has dimensions \\(C\times R\\).

**Formula**

\\[ A^T[j][i]=A[i][j] \\]

### Example

Original matrix:

\\[ A= \begin{bmatrix} 1&2&3\\\ 4&5&6 \end{bmatrix} \\]

Transpose:

\\[ A^T= \begin{bmatrix} 1&4\\\ 2&5\\\ 3&6 \end{bmatrix} \\]

### C implementation

```
#include <stdio.h>

int main(void)
{
    int A[10][10], T[10][10];
    int rows, cols;

    printf("Enter rows and columns: ");
    scanf("%d %d", &rows, &cols);

    if (rows <= 0 || cols <= 0 ||
        rows > 10 || cols > 10)
    {
        printf("Invalid dimensions.\n");
        return 1;
    }

    printf("Enter matrix elements:\n");

    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            scanf("%d", &A[i][j]);
        }
    }

    // Interchange row and column indices
    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            T[j][i] = A[i][j];
        }
    }

    printf("Transpose:\n");

    for (int i = 0; i < cols; i++)
    {
        for (int j = 0; j < rows; j++)
        {
            printf("%d ", T[i][j]);
        }

        printf("\n");
    }

    return 0;
}
```

Dry run:

| Original index | Original value | Transposed index |
| -------------- | -------------- | ---------------- |
| A[0][0]        | 1              | T[0][0]          |
| A[0][1]        | 2              | T[1][0]          |
| A[0][2]        | 3              | T[2][0]          |
| A[1][0]        | 4              | T[0][1]          |
| A[1][1]        | 5              | T[1][1]          |
| A[1][2]        | 6              | T[2][1]          |

Complexity:

\\[ T(R,C)=O(RC) \\]

\\[ S(R,C)=O(RC) \\]


## Chapter 2.3: Strings (Character Arrays)



### 2.3.1 Introduction to Strings


[DIRECTLY IN NOTES]

**Definition:**

A string in C is a sequence of characters stored in a character array and terminated by a special null character `'\0'`.

Unlike some other programming languages, C does not provide a separate built-in string data type.

Example:

```
char name[] = "Vishan";
```

Memory representation:

| Index | Character | ASCII value |
| ----- | --------- | ----------- |
| 0     | V         | 86          |
| 1     | i         | 105         |
| 2     | s         | 115         |
| 3     | h         | 104         |
| 4     | a         | 97          |
| 5     | n         | 110         |
| 6     | `\0`      | 0           |

Conceptual memory layout:

```
Index:    0    1    2    3    4    5     6
        +----+----+----+----+----+----+------+
        | V  | i  | s  | h  | a  | n  | \0   |
        +----+----+----+----+----+----+------+
```

**Important property:**

The null character marks the end of a C string.

\\[ \text{String length}=\text{Number of characters before }\backslash 0 \\]


### 2.3.2 String Declaration


[DIRECTLY IN NOTES]

Syntax:

```
char string_name[size];
```

Examples:

```
char name[20];
char city[30];
char university[] = "Chandigarh University";
```

**Different ways to initialise strings**

Method 1:

```
char str[] = "Hello";
```

Method 2:

```
char str[6] = "Hello";
```

Method 3:

```
char str[] = {'H', 'e', 'l', 'l', 'o', '\0'};
```

Method 4:

```
char str[20] = "Hello";
```

**Memory requirement:**

For a string containing \\(n\\) characters:

\\[ \text{Minimum array size}=n+1 \\]

The additional position is required for `'\0'`.


### 2.3.3 String Input and Output


[DIRECTLY IN NOTES]

**1. Using scanf()**

```
#include <stdio.h>

int main(void)
{
    char name[30];

    printf("Enter name: ");
    scanf("%29s", name);

    printf("Name: %s\n", name);

    return 0;
}
```

The field width prevents reading more than 29 characters, leaving one position for the null terminator.

However, `%s` stops at whitespace.

**2. Using fgets()**

```
#include <stdio.h>

int main(void)
{
    char sentence[100];

    printf("Enter a sentence: ");

    if (fgets(sentence, sizeof(sentence), stdin) != NULL)
    {
        printf("You entered: %s", sentence);
    }

    return 0;
}
```

`fgets()` reads at most one less than the buffer capacity and null-terminates the resulting string when successful.

It may retain the newline character if there is room.

**3. Using puts()**

```
#include <stdio.h>

int main(void)
{
    char message[] = "Welcome to C programming";

    puts(message);

    return 0;
}
```

`puts()` automatically appends a newline.

**4. Using getchar()**

```
#include <stdio.h>

int main(void)
{
    char ch;

    printf("Enter a character: ");
    ch = getchar();

    printf("Character: ");
    putchar(ch);

    putchar('\n');

    return 0;
}
```

**Comparison**

| Function           | Purpose               | Whitespace handling        |
| ------------------ | --------------------- | -------------------------- |
| `scanf("%s", ...)` | Read a word           | Stops at whitespace        |
| `fgets()`          | Read a line           | Can include spaces         |
| `puts()`           | Display a string      | Adds newline               |
| `getchar()`        | Read one character    | Reads next input character |
| `putchar()`        | Display one character | Character output           |

**⚠ Examiner's flag**

Never use `gets()` in modern C. It was removed from the C standard because it cannot prevent buffer overflow.


### 2.3.4 Standard String Library


[DIRECTLY IN NOTES]

The standard string-handling functions are declared in:

```
#include <string.h>
```

Important functions:

| Function   | Purpose                                              |
| ---------- | ---------------------------------------------------- |
| `strlen()` | Finds string length                                  |
| `strcpy()` | Copies a string                                      |
| `strcat()` | Concatenates strings                                 |
| `strcmp()` | Compares strings                                     |
| `strrev()` | Reverses a string in some non-standard libraries     |
| `strupr()` | Converts to uppercase in some non-standard libraries |
| `strlwr()` | Converts to lowercase in some non-standard libraries |

Important distinction: `strrev()`, `strupr()` and `strlwr()` are not part of the ISO C standard library. Their availability depends on the compiler or library.


### 2.3.5 strlen() Function


**Definition:**

`strlen()` returns the number of characters in a string before the terminating null character.

Syntax:

```
strlen(string);
```

Example:

```
#include <stdio.h>
#include <string.h>

int main(void)
{
    char str[] = "Chandigarh";

    printf("Length = %zu\n", strlen(str));

    return 0;
}
```

Output:

```
Length = 10
```

Mathematically:

\\[ \text{strlen}(s)=\text{Number of characters before }\backslash 0 \\]

Complexity:

\\[ T(n)=O(n) \\]


### 2.3.6 strcpy() Function


**Definition:**

`strcpy()` copies a null-terminated source string, including its terminating null character, into the destination array.

Syntax:

```
strcpy(destination, source);
```

Example:

```
#include <stdio.h>
#include <string.h>

int main(void)
{
    char source[] = "Programming";
    char destination[30];

    strcpy(destination, source);

    printf("Copied string: %s\n", destination);

    return 0;
}
```

Output:

```
Copied string: Programming
```

**Memory illustration:**

Before copying:

```
source:
+---+---+---+---+---+---+
| P | r | o | g | ... | \0 |
+---+---+---+---+---+---+

destination:
+---+---+---+---+---+
| ? | ? | ? | ? | ? |
+---+---+---+---+---+
```

After copying:

```
destination:
+---+---+---+---+---+------+
| P | r | o | g | ... | \0 |
+---+---+---+---+---+------+
```

The destination must have enough capacity.

\\[ \text{Destination capacity}\geq\text{Source length}+1 \\]


### 2.3.7 strcat() Function


**Definition:**

`strcat()` appends a source string to the end of a destination string.

Syntax:

```
strcat(destination, source);
```

Example:

```
#include <stdio.h>
#include <string.h>

int main(void)
{
    char first[50] = "Hello ";
    char second[] = "World";

    strcat(first, second);

    printf("%s\n", first);

    return 0;
}
```

Output:

```
Hello World
```

Memory representation:

Before concatenation:

```
first:  H e l l o _ \0
second: W o r l d \0
```

After concatenation:

```
first:  H e l l o _ W o r l d \0
```

Required capacity:

\\[ \text{Capacity}\geq L_1+L_2+1 \\]


### 2.3.8 strcmp() Function


**Definition:**

`strcmp()` compares two strings lexicographically.

Syntax:

```
strcmp(string1, string2);
```

Return value:

| Return value      | Meaning                      |
| ----------------- | ---------------------------- |
| Less than zero    | First string precedes second |
| Zero              | Strings are equal            |
| Greater than zero | First string follows second  |

Example:

```
#include <stdio.h>
#include <string.h>

int main(void)
{
    char a[] = "Apple";
    char b[] = "Apple";
    char c[] = "Banana";

    printf("%d\n", strcmp(a, b));
    printf("%d\n", strcmp(a, c));

    return 0;
}
```

The first comparison returns zero. The exact nonzero value of the second comparison is implementation-dependent.


### 2.3.9 strrev(), strupr() and strlwr()


[RESTORED STANDARD EQUATION / CODE]

These functions are commonly included in older teaching material, but they are not ISO C standard functions.

**strrev()**

Reverses a string.

**strupr()**

Converts alphabetic characters to uppercase.

**strlwr()**

Converts alphabetic characters to lowercase.

For portable C, implement these operations manually.


### 2.3.10 Manual String Length Without strlen()


[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    char str[100];
    int length = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    while (str[length] != '\0' &&
           str[length] != '\n')
    {
        length++;
    }

    printf("Length = %d\n", length);

    return 0;
}
```

Dry run for `"HELLO"`:

| Index | Character | Condition | Length |
| ----- | --------- | --------- | ------ |
| 0     | H         | True      | 1      |
| 1     | E         | True      | 2      |
| 2     | L         | True      | 3      |
| 3     | L         | True      | 4      |
| 4     | O         | True      | 5      |
| 5     | `\0`      | False     | 5      |

\\[ T(n)=O(n) \\]

\\[ S(n)=O(1) \\]


### 2.3.11 Manual String Copy Without strcpy()


[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    char source[100];
    char destination[100];
    int i = 0;

    printf("Enter a string: ");

    if (fgets(source, sizeof(source), stdin) == NULL)
    {
        return 1;
    }

    // Copy until null terminator
    while (source[i] != '\0')
    {
        destination[i] = source[i];
        i++;
    }

    // Add null terminator
    destination[i] = '\0';

    printf("Copied string: %s", destination);

    return 0;
}
```

**Dry run:**

Input: `CAT`

| Iteration | source[i] | destination[i] |
| --------- | --------- | -------------- |
| 0         | C         | C              |
| 1         | A         | A              |
| 2         | T         | T              |
| 3         | `\0`      | Stop           |


### 2.3.12 Manual String Concatenation Without strcat()


[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    char first[100] = "Hello ";
    char second[] = "World";

    int i = 0;
    int j = 0;

    // Find end of first string
    while (first[i] != '\0')
    {
        i++;
    }

    // Append second string
    while (second[j] != '\0')
    {
        first[i] = second[j];

        i++;
        j++;
    }

    // Terminate the result
    first[i] = '\0';

    printf("%s\n", first);

    return 0;
}
```

Output:

```
Hello World
```

**Complexity:**

\\[ T(n,m)=O(n+m) \\]


### 2.3.13 Manual String Comparison Without strcmp()


[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    char first[100];
    char second[100];

    int i = 0;

    printf("Enter first string: ");
    scanf("%99s", first);

    printf("Enter second string: ");
    scanf("%99s", second);

    // Compare corresponding characters
    while (first[i] == second[i] &&
           first[i] != '\0')
    {
        i++;
    }

    if (first[i] == second[i])
    {
        printf("Strings are equal.\n");
    }
    else if ((unsigned char)first[i] <
             (unsigned char)second[i])
    {
        printf("First string is smaller.\n");
    }
    else
    {
        printf("First string is greater.\n");
    }

    return 0;
}
```


### 2.3.14 Manual String Reversal


[EXAM SUPPORT]

```
#include <stdio.h>
#include <string.h>

int main(void)
{
    char str[100];
    int left = 0;
    int right;
    char temp;

    printf("Enter a string: ");

    if (fgets(str, sizeof(str), stdin) == NULL)
    {
        return 1;
    }

    // Remove newline if present
    size_t length = strlen(str);

    if (length > 0 && str[length - 1] == '\n')
    {
        str[length - 1] = '\0';
        length--;
    }

    right = (int)length - 1;

    // Reverse using two pointers
    while (left < right)
    {
        temp = str[left];
        str[left] = str[right];
        str[right] = temp;

        left++;
        right--;
    }

    printf("Reversed string: %s\n", str);

    return 0;
}
```

Example:

Input:

```
CHANDIGARH
```

Output:

```
HRAGIDNAHC
```

**Dry run:**

| Step | Left | Right | Swap    | Result      |
| ---- | ---- | ----- | ------- | ----------- |
| 1    | 0    | 9     | C and H | H...C       |
| 2    | 1    | 8     | H and A | HA...HC     |
| 3    | 2    | 7     | A and R | HAR...RHC   |
| 4    | 3    | 6     | N and G | HARG...NRHC |
| 5    | 4    | 5     | D and I | HRAGIDNAHC  |

Complexity:

\\[ T(n)=O(n) \\]

\\[ S(n)=O(1) \\]


### 2.3.15 Manual Uppercase Conversion


[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    char str[100];
    int i = 0;

    printf("Enter a string: ");

    if (fgets(str, sizeof(str), stdin) == NULL)
    {
        return 1;
    }

    while (str[i] != '\0')
    {
        if (str[i] >= 'a' && str[i] <= 'z')
        {
            str[i] = str[i] - ('a' - 'A');
        }

        i++;
    }

    printf("Uppercase: %s", str);

    return 0;
}
```


### 2.3.16 Manual Lowercase Conversion


[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    char str[100];
    int i = 0;

    printf("Enter a string: ");

    if (fgets(str, sizeof(str), stdin) == NULL)
    {
        return 1;
    }

    while (str[i] != '\0')
    {
        if (str[i] >= 'A' && str[i] <= 'Z')
        {
            str[i] = str[i] + ('a' - 'A');
        }

        i++;
    }

    printf("Lowercase: %s", str);

    return 0;
}
```

**⚠ Examiner's flag**

- A C string must terminate with `'\0'`.
- Character arrays do not automatically check their boundaries.
- `strlen()` does not count the null terminator.
- `strcpy()` requires enough destination memory.
- `strcat()` requires enough destination memory.
- `strcmp()` does not return only `-1`, `0` or `1`; only the sign is guaranteed.
- String comparison must use `strcmp()`, not `==`.
- `strrev()`, `strupr()` and `strlwr()` are non-standard.
- Never write beyond an array's allocated capacity.


## Chapter 2.4: Functions and Modular Programming



### 2.4.1 Introduction to Functions


[DIRECTLY IN NOTES]

**Definition:**

A function is a named, reusable block of statements designed to perform a specific task.

Functions divide a large program into smaller, manageable modules.

**Advantages of functions**

1. Code reusability.
2. Modularity.
3. Easier debugging.
4. Improved readability.
5. Reduced code duplication.
6. Easier maintenance.
7. Better program organisation.


### 2.4.2 Types of Functions


Functions in C are broadly classified into:

**1. Library Functions**

Predefined functions provided by standard libraries.

Examples:

- `printf()`
- `scanf()`
- `strlen()`
- `sqrt()`
- `malloc()`

**2. User-Defined Functions**

Functions created by programmers.

Example:

```
int add(int a, int b)
{
    return a + b;
}
```


### 2.4.3 Function Declaration or Prototype


[DIRECTLY IN NOTES]

**Definition:**

A function prototype declares a function's name, return type and parameter types before its actual definition or use.

Syntax:

```
return_type function_name(parameter_list);
```

Example:

```
int add(int, int);
```


### 2.4.4 Function Definition


A function definition contains the actual statements that perform the required operation.

Syntax:

```
return_type function_name(parameters)
{
    statements;

    return value;
}
```

Example:

```
int add(int a, int b)
{
    int sum = a + b;

    return sum;
}
```


### 2.4.5 Function Call


A function call transfers control to the specified function.

Example:

```
int result = add(10, 20);
```


### 2.4.6 Complete Function Program


[EXAM SUPPORT]

```
#include <stdio.h>

// Function declaration
int add(int a, int b);

int main(void)
{
    int x = 10;
    int y = 20;
    int result;

    // Function call
    result = add(x, y);

    printf("Sum = %d\n", result);

    return 0;
}

// Function definition
int add(int a, int b)
{
    int sum = a + b;

    return sum;
}
```

Output:

```
Sum = 30
```

**Function execution flow:**

```
        main()
           |
           v
      add(x, y)
           |
           v
    Calculate a + b
           |
           v
      return sum
           |
           v
     Back to main()
           |
           v
     Display result
```


### 2.4.7 Actual Arguments and Formal Parameters


[DIRECTLY IN NOTES]

**Actual arguments:**

The values or expressions supplied when calling a function.

**Formal parameters:**

The variables declared in the function definition to receive the supplied arguments.

Example:

```
#include <stdio.h>

int multiply(int a, int b)
{
    return a * b;
}

int main(void)
{
    int result;

    result = multiply(5, 4);

    printf("%d\n", result);

    return 0;
}
```

Here:

- `5` and `4` are actual arguments.
- `a` and `b` are formal parameters.

| Actual arguments         | Formal parameters              |
| ------------------------ | ------------------------------ |
| Present in function call | Present in function definition |
| Supply values            | Receive values                 |
| Can be expressions       | Declared variables             |


### 2.4.8 Types of User-Defined Functions


[DIRECTLY IN NOTES]

Four common categories are based on arguments and return values.

**Type 1: No arguments and no return value**

```
#include <stdio.h>

void display(void)
{
    printf("Hello World\n");
}

int main(void)
{
    display();

    return 0;
}
```

**Type 2: Arguments and no return value**

```
#include <stdio.h>

void add(int a, int b)
{
    printf("Sum = %d\n", a + b);
}

int main(void)
{
    add(10, 20);

    return 0;
}
```

**Type 3: No arguments but return value**

```
#include <stdio.h>

int getNumber(void)
{
    int number;

    printf("Enter a number: ");
    scanf("%d", &number);

    return number;
}

int main(void)
{
    int result = getNumber();

    printf("Number = %d\n", result);

    return 0;
}
```

**Type 4: Arguments and return value**

```
#include <stdio.h>

int add(int a, int b)
{
    return a + b;
}

int main(void)
{
    int result = add(10, 20);

    printf("Sum = %d\n", result);

    return 0;
}
```


### 2.4.9 Call by Value


[DIRECTLY IN NOTES]

**Definition:**

Call by value is a parameter-passing mechanism in which a function receives a copy of the argument's value.

Changes to the formal parameter do not directly modify the caller's original variable.

Example:

```
#include <stdio.h>

void change(int x)
{
    x = 100;
}

int main(void)
{
    int number = 10;

    change(number);

    printf("Number = %d\n", number);

    return 0;
}
```

Output:

```
Number = 10
```

**Memory representation:**

Before function call:

```
main():
+----------------+
| number = 10    |
+----------------+
```

During function call:

```
main() stack frame:

+----------------+
| number = 10    |
+----------------+

change() stack frame:

+----------------+
| x = 10         |
+----------------+
```

After changing `x`:

```
main():
+----------------+
| number = 10    |
+----------------+

change():
+----------------+
| x = 100        |
+----------------+
```

The original value remains unchanged.


### 2.4.10 Call by Reference Using Pointers


[DIRECTLY IN NOTES] [RESTORED STANDARD EQUATION / CODE]

C passes function arguments by value. Reference-like behaviour is achieved by passing a pointer to an object.

**Definition:**

The function receives the address of the caller's variable and uses dereferencing to modify the original object.

Example:

```
#include <stdio.h>

void change(int *x)
{
    *x = 100;
}

int main(void)
{
    int number = 10;

    change(&number);

    printf("Number = %d\n", number);

    return 0;
}
```

Output:

```
Number = 100
```

**Memory illustration:**

```
main():
+----------------------+
| number = 100         |
| Address = 1000       |
+----------------------+
           ^
           |
           |
change():
+----------------------+
| x = 1000             |
| *x = 100             |
+----------------------+
```

Here, `x` contains the address of `number`.

Dereferencing `x` accesses the original object.


### 2.4.11 Swapping Two Numbers Using Pointers


[EXAM SUPPORT]

```
#include <stdio.h>

void swap(int *a, int *b)
{
    int temp;

    temp = *a;
    *a = *b;
    *b = temp;
}

int main(void)
{
    int x = 10;
    int y = 20;

    printf("Before swapping:\n");
    printf("x = %d, y = %d\n", x, y);

    swap(&x, &y);

    printf("After swapping:\n");
    printf("x = %d, y = %d\n", x, y);

    return 0;
}
```

Output:

```
Before swapping:
x = 10, y = 20

After swapping:
x = 20, y = 10
```

Dry-run table:

| Step        | temp | \*a | \*b |
| ----------- | ---- | --- | --- |
| Initial     | -    | 10  | 20  |
| `temp = *a` | 10   | 10  | 20  |
| `*a = *b`   | 10   | 20  | 20  |
| `*b = temp` | 10   | 20  | 10  |


### 2.4.12 Difference Between Call by Value and Pointer-Based Reference


| Call by value                              | Pointer-based modification      |
| ------------------------------------------ | ------------------------------- |
| Receives a copy of the value               | Receives a copy of an address   |
| Original variable is not directly modified | Original object can be modified |
| Uses ordinary parameters                   | Uses pointer parameters         |
| No dereferencing needed                    | Dereferencing is required       |

**Important:** C does not have a separate language-level call-by-reference parameter mechanism. Both ordinary values and pointer values are passed by value.


### 2.4.13 Return Types


[DIRECTLY IN NOTES]

A function's return type specifies the type of value returned to its caller.

Examples:

```
int getAge(void)
{
    return 18;
}

float getPercentage(void)
{
    return 95.5f;
}

char getGrade(void)
{
    return 'A';
}

void display(void)
{
    printf("Hello\n");
}
```

**Void functions**

A function declared with `void` as its return type does not return a value.

```
void message(void)
{
    printf("Welcome\n");
}
```


### 2.4.14 Scope of Variables


[DIRECTLY IN NOTES]

**Definition:**

Scope determines the region of a program in which an identifier can be accessed by name.

Main categories:

1. Local scope.
2. File scope.
3. Function scope for labels.
4. Block scope.

**Local variable**

Declared inside a function or block.

```
void display(void)
{
    int x = 10;

    printf("%d", x);
}
```

The variable `x` cannot be accessed by name outside its block.

**Global variable**

Declared outside all functions.

```
#include <stdio.h>

int number = 100;

void display(void)
{
    printf("%d\n", number);
}

int main(void)
{
    display();

    return 0;
}
```


### 2.4.15 Lifetime of Variables


Lifetime describes the period during program execution for which an object exists.

| Variable category            | Typical lifetime                   |
| ---------------------------- | ---------------------------------- |
| Automatic local variable     | During execution of its block      |
| Global variable              | Entire program execution           |
| Local static variable        | Entire program execution           |
| Dynamically allocated object | From allocation until deallocation |


### 2.4.16 Local vs Global Variables


| Local variable                      | Global variable                                |
| ----------------------------------- | ---------------------------------------------- |
| Declared inside a function or block | Declared outside functions                     |
| Limited scope                       | File scope, subject to linkage                 |
| Automatic duration by default       | Static storage duration                        |
| Not automatically initialised       | Zero-initialised if not explicitly initialised |
| Created for block execution         | Exists for entire program execution            |

**⚠ Examiner's flag**

- A function prototype must match the function definition.
- Do not use an undeclared function.
- A non-void function should return an appropriate value along all paths where a value is required.
- A `void` function cannot return an expression.
- C passes arguments by value, including pointers.
- Local uninitialised automatic variables have indeterminate values.
- Do not return the address of an ordinary local automatic variable.


## Chapter 2.5: Recursion



### 2.5.1 Introduction to Recursion


[DIRECTLY IN NOTES]

**Definition:**

Recursion is a programming technique in which a function calls itself directly or indirectly to solve a problem by reducing it into smaller subproblems.

A recursive function must have:

1. Base condition.
2. Recursive condition.
3. Progress toward termination.

**General syntax:**

```
return_type function_name(parameters)
{
    if (base_condition)
    {
        return base_value;
    }

    return function_name(modified_parameters);
}
```


### 2.5.2 Base Condition


The base condition is the terminating condition that stops further recursive calls.

Without a reachable base condition, recursion may continue until available stack resources are exhausted.


### 2.5.3 Recursive Case


The recursive case reduces the problem and calls the same function again.

Example:

```
int countDown(int n)
{
    if (n == 0)
    {
        return 0;
    }

    printf("%d\n", n);

    return countDown(n - 1);
}
```


### 2.5.4 Direct and Indirect Recursion


[DIRECTLY IN NOTES]

**Direct recursion**

A function directly calls itself.

```
void functionA(void)
{
    functionA();
}
```

This example has no base condition and is not a safe terminating implementation.

**Indirect recursion**

One function calls another, which eventually calls the first function again.

```
#include <stdio.h>

void functionB(int n);

void functionA(int n)
{
    if (n <= 0)
        return;

    printf("A: %d\n", n);

    functionB(n - 1);
}

void functionB(int n)
{
    if (n <= 0)
        return;

    printf("B: %d\n", n);

    functionA(n - 1);
}

int main(void)
{
    functionA(4);

    return 0;
}
```

Output:

```
A: 4
B: 3
A: 2
B: 1
```


### 2.5.5 Memory Execution of Recursive Functions


[DIRECTLY IN NOTES] [EXAM SUPPORT]

Every active function invocation requires its own execution state.

This is commonly represented using an activation record or stack frame.

An activation record may contain:

- Parameters.
- Local variables.
- Return address.
- Saved registers.
- Other implementation-specific information.

Example:

```
#include <stdio.h>

void display(int n)
{
    if (n == 0)
        return;

    printf("%d\n", n);

    display(n - 1);
}

int main(void)
{
    display(3);

    return 0;
}
```

**Call sequence:**

```
main()
  |
  v
display(3)
  |
  v
display(2)
  |
  v
display(1)
  |
  v
display(0)
  |
  v
Return
```

**Conceptual stack during deepest call:**

```
       TOP OF STACK
      +-------------+
      | display(0)  |
      +-------------+
      | display(1)  |
      +-------------+
      | display(2)  |
      +-------------+
      | display(3)  |
      +-------------+
      | main()      |
      +-------------+
       BOTTOM
```

As recursive calls return, their stack frames are removed in reverse order.


### 2.5.6 Factorial Using Recursion


[DIRECTLY IN NOTES] [EXAM SUPPORT]

**Definition:**

Factorial of a non-negative integer \\(n\\) is the product of all positive integers from 1 to \\(n\\).

Mathematical formula:

\\[ n!=n\times(n-1)\times(n-2)\times\cdots\times1 \\]

Base condition:

\\[ 0!=1 \\]

Recursive formula:

\\[ n!=n\times(n-1)! \\]

**C implementation:**

```
#include <stdio.h>

long long factorial(int n)
{
    // Base condition
    if (n == 0 || n == 1)
    {
        return 1;
    }

    // Recursive call
    return n * factorial(n - 1);
}

int main(void)
{
    int n;

    printf("Enter a non-negative integer: ");
    scanf("%d", &n);

    if (n < 0)
    {
        printf("Factorial is not defined for negative integers.\n");
        return 1;
    }

    // long long can hold factorial values only within its range
    if (n > 20)
    {
        printf("Input is too large for long long factorial.\n");
        return 1;
    }

    printf("Factorial = %lld\n", factorial(n));

    return 0;
}
```

Example:

\\[ 5!=5\times4\times3\times2\times1 \\]

\\[ 5!=120 \\]

**Dry-run table:**

| Function call  | Operation                  | Return value |
| -------------- | -------------------------- | ------------ |
| `factorial(5)` | \\(5\times factorial(4)\\) | 120          |
| `factorial(4)` | \\(4\times factorial(3)\\) | 24           |
| `factorial(3)` | \\(3\times factorial(2)\\) | 6            |
| `factorial(2)` | \\(2\times factorial(1)\\) | 2            |
| `factorial(1)` | Base condition             | 1            |

Call stack:

```
factorial(5)
    |
factorial(4)
    |
factorial(3)
    |
factorial(2)
    |
factorial(1)
    |
    v
    1
```

Complexity:

\\[ T(n)=O(n) \\]

Recursive stack space:

\\[ S(n)=O(n) \\]


### 2.5.7 Fibonacci Series Using Recursion


[DIRECTLY IN NOTES] [EXAM SUPPORT]

**Definition:**

The Fibonacci sequence is a sequence in which each term after the first two terms is the sum of the preceding two terms.

Sequence:

\\[ 0,1,1,2,3,5,8,13,21,\ldots \\]

Mathematical definition:

\\[ F(0)=0 \\]

\\[ F(1)=1 \\]

\\[ F(n)=F(n-1)+F(n-2) \\]

**C implementation:**

```
#include <stdio.h>

long long fibonacci(int n)
{
    // Base conditions
    if (n == 0)
        return 0;

    if (n == 1)
        return 1;

    // Recursive calculation
    return fibonacci(n - 1) +
           fibonacci(n - 2);
}

int main(void)
{
    int n, i;

    printf("Enter number of terms: ");
    scanf("%d", &n);

    if (n < 1 || n > 93)
    {
        printf("Enter a number between 1 and 93.\n");
        return 1;
    }

    printf("Fibonacci Series:\n");

    for (i = 0; i < n; i++)
    {
        printf("%lld ", fibonacci(i));
    }

    printf("\n");

    return 0;
}
```

Output for 7 terms:

```
0 1 1 2 3 5 8
```

**Dry-run table:**

| n | Calculation    | Result |
| - | -------------- | ------ |
| 0 | Base condition | 0      |
| 1 | Base condition | 1      |
| 2 | F(1) + F(0)    | 1      |
| 3 | F(2) + F(1)    | 2      |
| 4 | F(3) + F(2)    | 3      |
| 5 | F(4) + F(3)    | 5      |
| 6 | F(5) + F(4)    | 8      |

**Complexity analysis:**

Naive recursive Fibonacci has exponential time complexity.

\\[ T(n)=O(\varphi^n) \\]

where:

\\[ \varphi=\frac{1+\sqrt5}{2} \\]

It is commonly bounded by:

\\[ T(n)=O(2^n) \\]

Maximum recursion depth:

\\[ S(n)=O(n) \\]

**Exam note:** The iterative Fibonacci algorithm runs in linear time and constant auxiliary space, while naive recursion repeats many calculations.


### 2.5.8 Fibonacci Using Iteration


[EXAM SUPPORT]

```
#include <stdio.h>

int main(void)
{
    int n, i;
    long long first = 0;
    long long second = 1;
    long long next;

    printf("Enter number of terms: ");
    scanf("%d", &n);

    if (n < 1 || n > 93)
    {
        printf("Invalid number of terms.\n");
        return 1;
    }

    for (i = 0; i < n; i++)
    {
        printf("%lld ", first);

        next = first + second;
        first = second;
        second = next;
    }

    printf("\n");

    return 0;
}
```

Complexity:

\\[ T(n)=O(n) \\]

\\[ S(n)=O(1) \\]


### 2.5.9 GCD Using Euclid's Algorithm


[DIRECTLY IN NOTES] [EXAM SUPPORT]

**Definition:**

The Greatest Common Divisor (GCD) of two integers is the largest positive integer that divides both numbers without leaving a remainder.

Euclid's algorithm uses the mathematical identity:

\\[ \gcd(a,b)=\gcd(b,a\bmod b) \\]

Base condition:

\\[ \gcd(a,0)=|a| \\]

**Recursive algorithm:**

1. Start.
2. Read two integers.
3. If the second integer is zero, return the absolute value of the first.
4. Otherwise, call GCD with the second number and the remainder.
5. Continue until the second number becomes zero.
6. Display the result.

**C implementation:**

```
#include <stdio.h>

int gcd(int a, int b)
{
    // Base condition
    if (b == 0)
    {
        return a;
    }

    // Recursive Euclidean step
    return gcd(b, a % b);
}

int main(void)
{
    int a, b;

    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    // Restrict this simple implementation to non-negative inputs
    if (a < 0 || b < 0)
    {
        printf("Enter non-negative integers.\n");
        return 1;
    }

    printf("GCD = %d\n", gcd(a, b));

    return 0;
}
```

Example:

\\[ \gcd(48,18) \\]

\\[ =\gcd(18,48\bmod18) \\]

\\[ =\gcd(18,12) \\]

\\[ =\gcd(12,6) \\]

\\[ =\gcd(6,0) \\]

\\[ =6 \\]

**Dry-run table:**

| Step | a  | b  | a % b |
| ---- | -- | -- | ----- |
| 1    | 48 | 18 | 12    |
| 2    | 18 | 12 | 6     |
| 3    | 12 | 6  | 0     |
| 4    | 6  | 0  | Stop  |

Complexity:

\\[ T(n)=O(\log(\min(a,b))) \\]

Recursive stack space:

\\[ S(n)=O(\log(\min(a,b))) \\]

**⚠ Examiner's flag**

- The remainder operation requires a nonzero divisor.
- Handle negative values if the question requires arbitrary integers.
- The mathematical GCD is normally non-negative.
- A practical implementation should consider the special case of the minimum signed integer when taking its absolute value.


### 2.5.10 Tower of Hanoi


[DIRECTLY IN NOTES] [EXAM SUPPORT]

**Definition:**

Tower of Hanoi is a mathematical puzzle involving three rods and a set of disks of different sizes.

Initially, all disks are stacked on one rod in decreasing order of size.

The objective is to move all disks to another rod using an auxiliary rod while following three rules.

**Rules:**

1. Only one disk may be moved at a time.
2. Only the top disk of a rod may be moved.
3. A larger disk cannot be placed on a smaller disk.

**Three rods:**

- Source (A).
- Auxiliary (B).
- Destination (C).

**Algorithm:**

To move \\(n\\) disks from A to C using B:

1. Move \\(n-1\\) disks from A to B using C.
2. Move the largest disk from A to C.
3. Move \\(n-1\\) disks from B to C using A.

**Recursive pseudocode:**

```
TOH(n, source, auxiliary, destination)

IF n == 1
    PRINT source TO destination
    RETURN

TOH(n-1, source, destination, auxiliary)

PRINT source TO destination

TOH(n-1, auxiliary, source, destination)
```

**C implementation:**

```
#include <stdio.h>

void towerOfHanoi(int n, char source,
                  char auxiliary, char destination)
{
    // Base condition
    if (n == 1)
    {
        printf("Move disk 1 from %c to %c\n",
               source, destination);

        return;
    }

    // Move n-1 disks to auxiliary rod
    towerOfHanoi(n - 1, source,
                 destination, auxiliary);

    // Move largest disk to destination
    printf("Move disk %d from %c to %c\n",
           n, source, destination);

    // Move n-1 disks to destination
    towerOfHanoi(n - 1, auxiliary,
                 source, destination);
}

int main(void)
{
    int n;

    printf("Enter number of disks: ");
    scanf("%d", &n);

    if (n < 1 || n > 20)
    {
        printf("Enter a disk count between 1 and 20.\n");
        return 1;
    }

    towerOfHanoi(n, 'A', 'B', 'C');

    return 0;
}
```

Example for 3 disks:

```
Move disk 1 from A to C
Move disk 2 from A to B
Move disk 1 from C to B
Move disk 3 from A to C
Move disk 1 from B to A
Move disk 2 from B to C
Move disk 1 from A to C
```

**Dry-run table:**

| Move | Disk | Source | Destination |
| ---- | ---- | ------ | ----------- |
| 1    | 1    | A      | C           |
| 2    | 2    | A      | B           |
| 3    | 1    | C      | B           |
| 4    | 3    | A      | C           |
| 5    | 1    | B      | A           |
| 6    | 2    | B      | C           |
| 7    | 1    | A      | C           |


### 2.5.11 Tower of Hanoi Recurrence Relation


[DIRECTLY IN NOTES]

Let \\(T(n)\\) represent the minimum number of moves required for \\(n\\) disks.

The recurrence relation is:

\\[ T(n)=2T(n-1)+1 \\]

Base condition:

\\[ T(1)=1 \\]

Expanding:

\\[ T(n)=2[2T(n-2)+1]+1 \\]

\\[ T(n)=4T(n-2)+2+1 \\]

Continuing:

\\[ T(n)=2^nT(0)+(2^{n-1}+\cdots+2+1) \\]

Using:

\\[ T(0)=0 \\]

And the geometric series:

\\[ 1+2+4+\cdots+2^{n-1}=2^n-1 \\]

Therefore:

\\[ \boxed{T(n)=2^n-1} \\]

**Number of moves for different disk counts:**

| Disks | Minimum moves |
| ----- | ------------- |
| 1     | 1             |
| 2     | 3             |
| 3     | 7             |
| 4     | 15            |
| 5     | 31            |
| 6     | 63            |
| 7     | 127           |
| 8     | 255           |
| 10    | 1023          |

Time complexity:

\\[ T(n)=O(2^n) \\]

Auxiliary recursion stack:

\\[ S(n)=O(n) \\]

**⚠ Examiner's flag**

- Do not interchange the auxiliary and destination parameters.
- Always move \\(n-1\\) disks before moving the largest disk.
- The base condition is essential.
- The minimum number of moves is \\(2^n-1\\), not \\(2^n\\).
- Tower of Hanoi has exponential time complexity.


# UNIT 2: EXAMINATION CHECKPOINT


## Important theory questions

1. Differentiate between entry-controlled and exit-controlled loops.
2. Explain `while`, `do-while` and `for` loops with syntax and examples.
3. Explain nested loops and infinite loops.
4. Differentiate between `break`, `continue`, `return` and `exit()`.
5. Define an array and explain its memory organisation.
6. Differentiate between compile-time and run-time array initialisation.
7. Explain linear search and binary search with algorithms.
8. Explain bubble sort with a dry-run table.
9. Explain one-dimensional and two-dimensional arrays.
10. Derive the row-major and column-major address calculation formulas.
11. Explain matrix addition, multiplication and transpose.
12. Define a string and explain the importance of the null character.
13. Explain `strlen()`, `strcpy()`, `strcat()` and `strcmp()`.
14. Differentiate between `scanf()` and `fgets()` for string input.
15. Explain string manipulation without using library functions.
16. Define functions and explain function declaration, definition and calling.
17. Differentiate between actual arguments and formal parameters.
18. Explain the four categories of user-defined functions.
19. Differentiate between call by value and pointer-based modification.
20. Explain local and global variables, scope and lifetime.
21. Define recursion and explain direct and indirect recursion.
22. Explain activation records and recursive function execution.
23. Write recursive programs for factorial, Fibonacci and GCD.
24. Explain Tower of Hanoi with its recurrence relation.
25. Derive the minimum number of Tower of Hanoi moves.

## Important programming questions

| No. | Program                              | Main concept        |
| --- | ------------------------------------ | ------------------- |
| 1   | Print numbers from 1 to N            | `for` loop          |
| 2   | Sum of first N natural numbers       | Loop                |
| 3   | Factorial using iteration            | Loop                |
| 4   | Reverse a number                     | `while` loop        |
| 5   | Check palindrome number              | Loop and conditions |
| 6   | Prime number checking                | Nested loops        |
| 7   | Fibonacci series                     | Iteration           |
| 8   | Find largest array element           | Array traversal     |
| 9   | Linear search                        | Searching           |
| 10  | Binary search                        | Searching           |
| 11  | Bubble sort                          | Sorting             |
| 12  | Matrix addition                      | 2D arrays           |
| 13  | Matrix multiplication                | Nested loops        |
| 14  | Matrix transpose                     | 2D arrays           |
| 15  | String length without `strlen()`     | Strings             |
| 16  | String reversal                      | Character arrays    |
| 17  | String comparison without `strcmp()` | Strings             |
| 18  | Swap two numbers using pointers      | Functions           |
| 19  | Factorial using recursion            | Recursion           |
| 20  | GCD using Euclid's algorithm         | Recursion           |
| 21  | Tower of Hanoi                       | Recursion           |

## Essential formulas for Unit 2

**Arrays**

Row-major order:

\\[ \operatorname{Address}(A[i][j]) = B+(i\times C+j)\times S \\]

Column-major order:

\\[ \operatorname{Address}(A[i][j]) = B+(j\times R+i)\times S \\]

Where:

- \\(B\\) = Base address.
- \\(R\\) = Number of rows.
- \\(C\\) = Number of columns.
- \\(S\\) = Size of each element.

**Matrix multiplication**

\\[ C[i][j]=\sum\_{k=0}^{n-1}A[i][k]B[k][j] \\]

**String storage**

\\[ \text{Required storage}=\text{String length}+1 \\]

**Factorial**

\\[ n!=n\times(n-1)! \\]

\\[ 0!=1 \\]

**Fibonacci**

\\[ F(n)=F(n-1)+F(n-2) \\]

**Euclidean GCD**

\\[ \gcd(a,b)=\gcd(b,a\bmod b) \\]

**Tower of Hanoi**

\\[ T(n)=2T(n-1)+1 \\]

\\[ \boxed{T(n)=2^n-1} \\]


# UNIT 2: IMPORTANT COMPLEXITY TABLE


| Algorithm                 | Time complexity                  | Auxiliary space                  |
| ------------------------- | -------------------------------- | -------------------------------- |
| Array traversal           | \\(O(n)\\)                       | \\(O(1)\\)                       |
| Linear search             | \\(O(n)\\)                       | \\(O(1)\\)                       |
| Binary search             | \\(O(\log n)\\)                  | \\(O(1)\\) iterative             |
| Bubble sort               | \\(O(n^2)\\) worst case          | \\(O(1)\\)                       |
| Matrix addition           | \\(O(mn)\\)                      | \\(O(1)\\) excluding result      |
| Matrix multiplication     | \\(O(n^3)\\) for square matrices | \\(O(1)\\) excluding result      |
| Matrix transpose          | \\(O(mn)\\)                      | \\(O(1)\\) excluding result      |
| String length             | \\(O(n)\\)                       | \\(O(1)\\)                       |
| String reversal           | \\(O(n)\\)                       | \\(O(1)\\)                       |
| String concatenation      | \\(O(n+m)\\)                     | \\(O(1)\\) excluding destination |
| Recursive factorial       | \\(O(n)\\)                       | \\(O(n)\\)                       |
| Naive recursive Fibonacci | \\(O(2^n)\\) upper bound         | \\(O(n)\\)                       |
| Iterative Fibonacci       | \\(O(n)\\)                       | \\(O(1)\\)                       |
| Recursive GCD             | \\(O(\log(\min(a,b)))\\)         | \\(O(\log(\min(a,b)))\\)         |
| Tower of Hanoi            | \\(O(2^n)\\)                     | \\(O(n)\\)                       |

**



# UNIT 3: POINTERS, STORAGE CLASSES, STRUCTURES, UNIONS & DYNAMIC MEMORY ALLOCATION



This final part completes the C programming compendium with Unit 3, followed by 15 solved high-yield programs, a common-mistakes and debugging checklist, and a quick-revision cheat sheet.

**Notation used throughout:**

- `[DIRECTLY IN NOTES]` identifies core syllabus concepts.
- `[RESTORED STANDARD EQUATION / CODE]` identifies standard C concepts, equations, or implementations included to make the material complete.
- `[EXAM SUPPORT]` identifies additional explanations, examples, and likely examination points.
- `⚠ Examiner’s flag:` identifies common errors, undefined behaviour, portability issues, and examination traps.



# UNIT 3: POINTERS, STORAGE CLASSES, STRUCTURES, UNIONS & DYNAMIC MEMORY ALLOCATION




## CHAPTER 3.1: POINTERS IN C



### 3.1.1 Introduction to pointers


[DIRECTLY IN NOTES]

A **pointer** is a variable that stores the memory address of another variable.

Ordinary variables store values, whereas pointer variables store addresses.

For example:

```
int number = 25;
int *ptr = &number;
```

Here:

- `number` is an integer variable containing `25`.
- `&number` gives the memory address of `number`.
- `ptr` is a pointer variable that stores that address.
- `*ptr` accesses the value stored at the address contained in `ptr`.


### 3.1.2 Why are pointers required?


Pointers are important because they allow C programs to:

1. Access and manipulate memory directly.
2. Pass addresses to functions.
3. Modify original variables through pointer parameters.
4. Process arrays and strings efficiently.
5. Create dynamic data structures.
6. Allocate and release memory dynamically.
7. Work with structures and linked data.
8. Implement low-level system programming operations.


### 3.1.3 Address operator and indirection operator


[DIRECTLY IN NOTES]

C provides two important pointer operators.

| Operator | Name                             | Purpose                                 |
| -------- | -------------------------------- | --------------------------------------- |
| `&`      | Address-of operator              | Returns the address of a variable       |
| `*`      | Indirection/dereference operator | Accesses the value stored at an address |

Example:

```
#include <stdio.h>

int main(void)
{
    int x = 50;
    int *p = &x;

    printf("Value of x: %d\n", x);
    printf("Address of x: %p\n", (void *)&x);
    printf("Value stored in p: %p\n", (void *)p);
    printf("Value accessed through p: %d\n", *p);

    return 0;
}
```

**Conceptual memory diagram**

```
             VARIABLE x
        +-------------------+
        | Value = 50        |
        | Address = 1000    |
        +-------------------+
                 ^
                 |
                 | ptr stores 1000
                 |
        +-------------------+
        | Pointer ptr       |
        | Value = 1000      |
        | Address = 2000    |
        +-------------------+

        *ptr gives the value 50
        &x gives the address 1000
```

Illustrative addresses only. Actual addresses are assigned by the execution environment.


### 3.1.4 Pointer declaration and initialization


[DIRECTLY IN NOTES]

**General syntax:**

```
data_type *pointer_name;
```

Examples:

```
int *p;
float *fp;
char *cp;
double *dp;
```

A pointer's declared type determines the type of object it can point to and the type of value obtained when it is dereferenced.

Correct initialization:

```
int x = 10;
int *p = &x;
```

A pointer can also be initialized to `NULL` when it does not currently point to a valid object:

```
int *p = NULL;
```

⚠ **Examiner’s flag:** An uninitialized local pointer contains an indeterminate value. Dereferencing it can cause undefined behaviour.


### 3.1.5 Understanding pointer declaration syntax


Consider:

```
int *p, q;
```

Only `p` is a pointer. `q` is an ordinary integer.

For two integer pointers:

```
int *p, *q;
```

The asterisk belongs to each declarator, not automatically to every variable in the declaration.


### 3.1.6 Pointer dereferencing


[DIRECTLY IN NOTES]

Dereferencing means accessing the object pointed to by a pointer.

```
#include <stdio.h>

int main(void)
{
    int a = 100;
    int *p = &a;

    printf("%d\n", *p);

    *p = 250;

    printf("%d\n", a);

    return 0;
}
```

**Output:**

```
100
250
```

Explanation:

- Initially, `*p` reads the value of `a`.
- Assigning `250` to `*p` modifies the object `a`.
- Therefore, printing `a` gives `250`.


### 3.1.7 Pointer arithmetic


[DIRECTLY IN NOTES]

Pointer arithmetic allows a pointer to move between elements of an array.

Valid pointer arithmetic operations include:

- Incrementing a pointer.
- Decrementing a pointer.
- Adding an integer to a pointer.
- Subtracting an integer from a pointer.
- Subtracting two pointers that point into the same array, or one position beyond it.

For an array of type `T`, adding one to a pointer advances it by `sizeof(T)` bytes.

\\[ p+1 = p+\operatorname{sizeof}(T) \\]

If an integer occupies 4 bytes on a particular implementation, incrementing an `int *` advances its address by 4 bytes.

Example:

```
#include <stdio.h>

int main(void)
{
    int arr[] = {10, 20, 30, 40};
    int *p = arr;

    printf("%d\n", *p);

    p++;

    printf("%d\n", *p);

    p = p + 2;

    printf("%d\n", *p);

    return 0;
}
```

**Output:**

```
10
20
40
```

### Pointer arithmetic memory diagram

Assume each integer occupies 4 bytes.

```
Array:

Index       0       1       2       3
          +-------+-------+-------+-------+
Value     |  10   |  20   |  30   |  40   |
          +-------+-------+-------+-------+
Address    1000    1004    1008    1012
             ^
             |
             p

After p++:

Index       0       1       2       3
          +-------+-------+-------+-------+
Value     |  10   |  20   |  30   |  40   |
          +-------+-------+-------+-------+
Address    1000    1004    1008    1012
                     ^
                     |
                     p
```

### Pointer arithmetic rules

| Expression | Meaning                                        |
| ---------- | ---------------------------------------------- |
| `p++`      | Move to the next element                       |
| `p--`      | Move to the previous element                   |
| `p + 3`    | Move forward by three elements                 |
| `p - 2`    | Move backward by two elements                  |
| `p2 - p1`  | Number of elements between compatible pointers |
| `*p`       | Value pointed to by `p`                        |
| `*(p + 2)` | Value at the third element relative to `p`     |

⚠ **Examiner’s flag:** Pointer arithmetic is not ordinary byte arithmetic. `p + 1` advances by one pointed-to element, not necessarily one byte.

Pointer arithmetic must remain within the same array object or its one-past-the-end position. Dereferencing the one-past pointer is invalid.


### 3.1.8 Pointer subtraction


[RESTORED STANDARD EQUATION / CODE]

If two pointers point into the same array, subtracting them gives the number of elements between them.

```
#include <stdio.h>
#include <stddef.h>

int main(void)
{
    int a[] = {5, 10, 15, 20, 25};

    int *p1 = &a[1];
    int *p2 = &a[4];

    ptrdiff_t difference = p2 - p1;

    printf("Difference = %td\n", difference);

    return 0;
}
```

**Output:**

```
Difference = 3
```

\\[ p_2-p_1=4-1=3 \\]

The result is measured in array elements, not bytes.


### 3.1.9 Relationship between arrays and pointers


[DIRECTLY IN NOTES]

The array name usually converts to a pointer to its first element when used in an expression.

For an array:

```
int arr[5] = {10, 20, 30, 40, 50};
```

The following expressions are equivalent:

```
arr[0]
*(arr + 0)

arr[1]
*(arr + 1)

arr[2]
*(arr + 2)
```

In general:

\\[ arr[i] = \*(arr+i) \\]

Example:

```
#include <stdio.h>

int main(void)
{
    int arr[] = {10, 20, 30, 40, 50};

    for (int i = 0; i < 5; i++)
    {
        printf("%d ", *(arr + i));
    }

    return 0;
}
```

**Output:**

```
10 20 30 40 50
```

⚠ **Examiner’s flag:** An array name is not an ordinary modifiable pointer variable. You cannot write `arr++` or assign a new address to `arr`.


### 3.1.10 Pointer to pointer


[DIRECTLY IN NOTES]

A pointer to pointer stores the address of another pointer.

**Syntax:**

```
data_type **pointer_name;
```

Example:

```
#include <stdio.h>

int main(void)
{
    int x = 75;

    int *p = &x;
    int **q = &p;

    printf("Value of x: %d\n", x);
    printf("Using p: %d\n", *p);
    printf("Using q: %d\n", **q);

    return 0;
}
```

**Output:**

```
Value of x: 75
Using p: 75
Using q: 75
```

Memory relationship:

```
       x
   +--------+
   |   75   |
   +--------+
       ^
       |
       | p stores address of x
       |
   +--------+
   |   p    |
   +--------+
       ^
       |
       | q stores address of p
       |
   +--------+
   |   q    |
   +--------+

   *p  = 75
   **q = 75
```


### 3.1.11 Different types of pointers


[EXAM SUPPORT]

| Pointer type     | Description                     |
| ---------------- | ------------------------------- |
| `int *`          | Points to an integer            |
| `char *`         | Points to a character           |
| `float *`        | Points to a float               |
| `double *`       | Points to a double              |
| `void *`         | Generic object pointer          |
| `int **`         | Pointer to an integer pointer   |
| Null pointer     | Points to no object or function |
| Function pointer | Stores a function address       |

### Void pointer

A `void *` is a generic pointer type that can hold the address of an object of any type.

```
#include <stdio.h>

int main(void)
{
    int x = 25;
    void *ptr = &x;

    printf("%d\n", *(int *)ptr);

    return 0;
}
```

**Output:**

```
25
```

A `void *` must be converted to an appropriate object-pointer type before dereferencing.

⚠ **Examiner’s flag:** Standard C does not allow direct arithmetic on a `void *`. Some compilers provide this as an extension, but it is not portable C.

### Null pointer

```
int *p = NULL;
```

A null pointer is guaranteed not to compare equal to a pointer to any object or function.

⚠ **Examiner’s flag:** Never dereference a null pointer.

### Wild pointer

A wild pointer is an uninitialized pointer that has not been assigned a valid address.

```
int *p;     /* Indeterminate pointer */
```

### Dangling pointer

A dangling pointer refers to an object whose lifetime has ended.

Example:

```
int *p;

{
    int x = 10;
    p = &x;
}

/* x no longer exists here.
   p is now dangling. */
```

### Function pointer

[EXAM SUPPORT]

A function pointer stores the address of a function.

```
#include <stdio.h>

int add(int a, int b)
{
    return a + b;
}

int main(void)
{
    int (*fp)(int, int) = add;

    printf("%d\n", fp(10, 20));

    return 0;
}
```

**Output:**

```
30
```


## CHAPTER 3.2: STORAGE CLASSES IN C



### 3.2.1 Introduction


[DIRECTLY IN NOTES]

A **storage class** in C determines properties associated with an identifier, including its scope, storage duration, and linkage.

The four traditional storage-class specifiers commonly taught in introductory C are:

1. `auto`
2. `register`
3. `static`
4. `extern`

Modern C also has other storage-class specifiers, such as `_Thread_local` and `typedef` in its grammar. For this syllabus, the four traditional categories are the primary focus.


### 3.2.2 Automatic storage class


[DIRECTLY IN NOTES]

The `auto` storage class is the default for ordinary local variables declared inside a block.

**Syntax:**

```
auto int x = 10;
```

Example:

```
#include <stdio.h>

int main(void)
{
    auto int x = 10;

    printf("%d\n", x);

    return 0;
}
```

**Output:**

```
10
```

Characteristics:

- Block scope when declared inside a block.
- Automatic storage duration.
- Created when execution enters its block.
- Its lifetime ends when execution leaves its block.
- An uninitialized automatic variable has an indeterminate value.

⚠ **Examiner’s flag:** `auto` does not mean that a variable is automatically initialized to zero.


### 3.2.3 Register storage class


[DIRECTLY IN NOTES]

The `register` keyword historically requests that a variable be stored in a CPU register for faster access.

**Syntax:**

```
register int count;
```

Example:

```
#include <stdio.h>

int main(void)
{
    register int i;

    for (i = 1; i <= 5; i++)
    {
        printf("%d ", i);
    }

    return 0;
}
```

**Output:**

```
1 2 3 4 5
```

Characteristics:

- Normally used for frequently accessed local variables.
- Has automatic storage duration.
- The compiler may ignore the register request.
- In traditional C teaching, the address operator `&` is not permitted on an object declared with `register`.

⚠ **Examiner’s flag:** `register` does not guarantee that the variable will physically be stored in a CPU register. Modern compilers make their own optimization decisions.


### 3.2.4 Static storage class


[DIRECTLY IN NOTES]

A variable declared with `static` has static storage duration. Its storage exists for the entire execution of the program.

A local static variable retains its value between function calls.

Example:

```
#include <stdio.h>

void counter(void)
{
    static int count = 0;

    count++;

    printf("%d\n", count);
}

int main(void)
{
    counter();
    counter();
    counter();

    return 0;
}
```

**Output:**

```
1
2
3
```

Explanation:

- `count` is initialized only once.
- Its value is retained after `counter()` finishes.
- Each call increments the previous value.

### Automatic variable versus static local variable

```
#include <stdio.h>

void test(void)
{
    int a = 0;
    static int b = 0;

    a++;
    b++;

    printf("a = %d, b = %d\n", a, b);
}

int main(void)
{
    test();
    test();
    test();

    return 0;
}
```

**Output:**

```
a = 1, b = 1
a = 1, b = 2
a = 1, b = 3
```

Memory concept:

```
Automatic variable a:
Call 1: Created as 0 -> incremented to 1 -> destroyed
Call 2: Created as 0 -> incremented to 1 -> destroyed
Call 3: Created as 0 -> incremented to 1 -> destroyed

Static variable b:
Program starts: Initialized to 0
Call 1: 0 -> 1
Call 2: 1 -> 2
Call 3: 2 -> 3
Program ends: Storage duration ends
```

A file-scope `static` variable or function has internal linkage, meaning it is accessible by name only within the same translation unit.


### 3.2.5 External storage class


[DIRECTLY IN NOTES]

The `extern` keyword declares an identifier that is defined elsewhere or later in the program.

Example using two source files:

**File 1:&#x20;**`main.c`

```
#include <stdio.h>

extern int total;

int main(void)
{
    printf("%d\n", total);

    return 0;
}
```

**File 2:&#x20;**`data.c`

```
int total = 500;
```

When both files are compiled and linked together, the program can print:

```
500
```

An `extern` declaration usually does not allocate a new object. It declares an existing object defined elsewhere.

A complete build command for these two files is:

```
gcc main.c data.c -o program
```

⚠ **Examiner’s flag:** Writing `extern int total;` does not itself initialize or define `total`. A compatible definition must exist somewhere in the program.


### 3.2.6 Comparison of storage classes


| Feature                           | `auto`                                            | `register`                                        | `static`                                    | `extern`                    |
| --------------------------------- | ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------- | --------------------------- |
| Typical use                       | Local variables                                   | Frequently used local variables                   | Persistent variables or internal linkage    | Access external definitions |
| Storage duration                  | Automatic                                         | Automatic                                         | Static                                      | Depends on declared object  |
| Default initialization            | Indeterminate for uninitialized automatic objects | Indeterminate for uninitialized automatic objects | Zero-initialized if no explicit initializer | Depends on definition       |
| Scope                             | Usually block                                     | Usually block                                     | Depends on declaration location             | Depends on declaration      |
| Retains local value between calls | No                                                | No                                                | Yes                                         | Depends on object           |
| Address operator                  | Allowed                                           | Historically prohibited for register objects      | Allowed                                     | Allowed for object          |


### 3.2.7 Scope, lifetime and linkage


[EXAM SUPPORT]

These three concepts are related but are not interchangeable.

- **Scope:** The region of source code where an identifier can be used.
- **Storage duration:** The period during program execution when an object exists.
- **Linkage:** Whether declarations in different scopes or translation units refer to the same entity.

Example:

```
#include <stdio.h>

int globalValue = 100;

void display(void)
{
    static int calls = 0;

    calls++;

    printf("Global = %d, Calls = %d\n",
           globalValue, calls);
}

int main(void)
{
    display();
    display();

    return 0;
}
```

**Output:**

```
Global = 100, Calls = 1
Global = 100, Calls = 2
```


## CHAPTER 3.3: STRUCTURES IN C



### 3.3.1 Introduction to structures


[DIRECTLY IN NOTES]

A **structure** is a user-defined data type that groups related variables of potentially different data types under one name.

For example, a student record may contain:

- Roll number: integer
- Name: character array
- Marks: floating-point value

A structure makes it possible to represent all these related fields as one logical record.


### 3.3.2 Structure declaration


**Syntax:**

```
struct structure_name
{
    data_type member1;
    data_type member2;
    data_type member3;
};
```

Example:

```
struct Student
{
    int roll;
    char name[50];
    float marks;
};
```

This declares a structure type named `struct Student`.

It does not, by itself, create a variable.


### 3.3.3 Declaring structure variables


Variables can be declared after the structure definition:

```
struct Student s1, s2;
```

Or alongside the structure definition:

```
struct Student
{
    int roll;
    float marks;
} s1, s2;
```


### 3.3.4 Accessing structure members


[DIRECTLY IN NOTES]

The dot operator `.` accesses a member of a structure object.

```
s1.roll
s1.marks
```

Example:

```
#include <stdio.h>

struct Student
{
    int roll;
    char name[50];
    float marks;
};

int main(void)
{
    struct Student s1 = {101, "Aman", 92.5f};

    printf("Roll Number: %d\n", s1.roll);
    printf("Name: %s\n", s1.name);
    printf("Marks: %.2f\n", s1.marks);

    return 0;
}
```

**Output:**

```
Roll Number: 101
Name: Aman
Marks: 92.50
```


### 3.3.5 Structure memory layout


[DIRECTLY IN NOTES]

Structure members are stored as part of the same structure object, but padding may be inserted between members or at the end to satisfy alignment requirements.

Consider:

```
struct Example
{
    char a;
    int b;
    char c;
};
```

A possible layout on a system where `char` has size 1, `int` has size 4, and `int` alignment is 4:

```
Offset      Contents
------      ----------------------------
0           a (1 byte)
1           Padding (3 bytes)
4           b (4 bytes)
8           c (1 byte)
9-11        Tail padding (3 bytes)

Total size = 12 bytes
```

Illustrative layout only. The C standard does not prescribe these exact sizes or padding amounts.

### Why does structure padding exist?

Processors and application binary interfaces often require objects to be placed at addresses that satisfy alignment rules.

For example, if an `int` requires 4-byte alignment, placing it at an offset divisible by 4 may improve or be necessary for correct access on that platform.

⚠ **Examiner’s flag:** Never assume `sizeof(struct Example)` is exactly the sum of its member sizes. Use `sizeof` to determine the actual size on the target implementation.


### 3.3.6 Accessing structure members using pointers


[DIRECTLY IN NOTES]

When a pointer points to a structure, the arrow operator `->` accesses its members.

```
pointer->member
```

It is equivalent to:

```
(*pointer).member
```

Example:

```
#include <stdio.h>

struct Student
{
    int roll;
    float marks;
};

int main(void)
{
    struct Student s = {101, 88.5f};

    struct Student *ptr = &s;

    printf("Roll: %d\n", ptr->roll);
    printf("Marks: %.2f\n", ptr->marks);

    return 0;
}
```

**Output:**

```
Roll: 101
Marks: 88.50
```

⚠ **Examiner’s flag:** `*ptr.roll` is not the correct way to access a member through a structure pointer. Use `ptr->roll` or `(*ptr).roll`.


### 3.3.7 Array of structures


[DIRECTLY IN NOTES]

An array of structures stores multiple records of the same structure type.

Example:

```
#include <stdio.h>

struct Student
{
    int roll;
    char name[30];
    float marks;
};

int main(void)
{
    struct Student s[3] =
    {
        {101, "Aman", 85.5f},
        {102, "Riya", 91.0f},
        {103, "Karan", 78.5f}
    };

    for (int i = 0; i < 3; i++)
    {
        printf("%d %s %.2f\n",
               s[i].roll,
               s[i].name,
               s[i].marks);
    }

    return 0;
}
```

**Output:**

```
101 Aman 85.50
102 Riya 91.00
103 Karan 78.50
```


### 3.3.8 Nested structures


[EXAM SUPPORT]

A structure can contain another structure as a member.

```
#include <stdio.h>

struct Date
{
    int day;
    int month;
    int year;
};

struct Student
{
    int roll;
    char name[30];
    struct Date dob;
};

int main(void)
{
    struct Student s =
    {
        101,
        "Aman",
        {15, 8, 2006}
    };

    printf("Name: %s\n", s.name);
    printf("Date of Birth: %02d-%02d-%04d\n",
           s.dob.day,
           s.dob.month,
           s.dob.year);

    return 0;
}
```

**Output:**

```
Name: Aman
Date of Birth: 15-08-2006
```


### 3.3.9 Passing structures to functions


[EXAM SUPPORT]

A structure can be passed to a function by value or through a pointer.

### Passing by value

```
#include <stdio.h>

struct Student
{
    int roll;
    float marks;
};

void display(struct Student s)
{
    printf("Roll = %d\n", s.roll);
    printf("Marks = %.2f\n", s.marks);
}

int main(void)
{
    struct Student s1 = {101, 90.5f};

    display(s1);

    return 0;
}
```

The function receives a copy of the structure object.

### Passing by pointer

```
#include <stdio.h>

struct Student
{
    int roll;
    float marks;
};

void update(struct Student *s)
{
    s->marks = 95.0f;
}

int main(void)
{
    struct Student s1 = {101, 80.0f};

    update(&s1);

    printf("%.2f\n", s1.marks);

    return 0;
}
```

**Output:**

```
95.00
```


### 3.3.10 Structure assignment


[RESTORED STANDARD EQUATION / CODE]

Structure objects of compatible structure type can be assigned directly.

```
#include <stdio.h>

struct Point
{
    int x;
    int y;
};

int main(void)
{
    struct Point p1 = {10, 20};
    struct Point p2;

    p2 = p1;

    printf("%d %d\n", p2.x, p2.y);

    return 0;
}
```

**Output:**

```
10 20
```

Structure assignment copies the member values. If a member is a pointer, its pointer value is copied, not the object it points to.

⚠ **Examiner’s flag:** C does not support direct comparison of two structure objects using `==` or `!=`. Compare their members individually.


### 3.3.11 Structure versus array


| Structure                                                 | Array                                 |
| --------------------------------------------------------- | ------------------------------------- |
| Groups members that may have different types              | Stores elements of one element type   |
| Members are accessed by names                             | Elements are accessed by index        |
| Uses `.` or `->` for member access                        | Uses `[]` for indexing                |
| Represents a record                                       | Represents a sequence of elements     |
| Structure assignment is allowed for compatible structures | Whole-array assignment is not allowed |


## CHAPTER 3.4: UNIONS IN C



### 3.4.1 Introduction to unions


[DIRECTLY IN NOTES]

A **union** is a user-defined data type in which all members share the same memory location.

Unlike a structure, a union stores its members in overlapping memory.

**Syntax:**

```
union union_name
{
    data_type member1;
    data_type member2;
    data_type member3;
};
```

Example:

```
union Data
{
    int i;
    float f;
    char ch;
};
```


### 3.4.2 Union memory layout


Consider:

```
union Data
{
    int i;
    float f;
    char ch;
};
```

Conceptual memory:

```
          UNION DATA
      +-------------------+
      |                   |
      |    Shared memory  |
      |                   |
      +-------------------+
        |       |       |
        i       f       ch
      int     float    char
```

The union must have enough storage for its largest member, with any additional padding required by alignment.

\\[ \operatorname{sizeof}(\text{union}) \geq \max(\operatorname{sizeof}(m_1),\ldots,\operatorname{sizeof}(m_n)) \\]

This is a lower bound, not a guarantee that the union's size equals the largest member's size.


### 3.4.3 Accessing union members


Example:

```
#include <stdio.h>

union Data
{
    int i;
    float f;
    char ch;
};

int main(void)
{
    union Data d;

    d.i = 100;
    printf("Integer: %d\n", d.i);

    d.f = 25.5f;
    printf("Float: %.2f\n", d.f);

    d.ch = 'A';
    printf("Character: %c\n", d.ch);

    return 0;
}
```

**Output:**

```
Integer: 100
Float: 25.50
Character: A
```

Each assignment stores a new value in the shared storage.

⚠ **Examiner’s flag:** Do not assume all union members retain independent values. Writing one member can change the stored representation used by the others.


### 3.4.4 Structure versus union


[DIRECTLY IN NOTES]

| Feature           | Structure                                      | Union                                                |
| ----------------- | ---------------------------------------------- | ---------------------------------------------------- |
| Memory allocation | Separate storage for each member, plus padding | Shared storage for members, plus possible padding    |
| Values            | Members can hold values simultaneously         | Normally one member's value is stored at a time      |
| Size              | At least enough for all members and padding    | At least enough for the largest member and alignment |
| Member addresses  | Members occupy distinct subobjects             | Members begin at the same address                    |
| Main purpose      | Group related data                             | Share storage between alternative representations    |


### 3.4.5 Practical use of unions


Unions are useful when a program needs to store one of several alternative data types.

For example:

```
#include <stdio.h>

enum DataType
{
    TYPE_INT,
    TYPE_FLOAT,
    TYPE_CHAR
};

struct Value
{
    enum DataType type;

    union
    {
        int i;
        float f;
        char ch;
    } data;
};

int main(void)
{
    struct Value v;

    v.type = TYPE_FLOAT;
    v.data.f = 45.75f;

    if (v.type == TYPE_FLOAT)
    {
        printf("Float value = %.2f\n", v.data.f);
    }

    return 0;
}
```

**Output:**

```
Float value = 45.75
```

This is called a **tagged union** or **discriminated union** design: the `type` field indicates which union member is currently intended to be used.


## CHAPTER 3.5: BIT-FIELDS, TYPEDEF AND ENUM



### 3.5.1 Bit-fields


[DIRECTLY IN NOTES]

A bit-field is a structure or union member with a specified number of bits.

It can be useful for representing small integer values or compact flags.

**Syntax:**

```
struct Flags
{
    unsigned int flag1 : 1;
    unsigned int flag2 : 1;
    unsigned int mode  : 3;
};
```

Here:

- `flag1` has a declared width of 1 bit.
- `flag2` has a declared width of 1 bit.
- `mode` has a declared width of 3 bits.

Example:

```
#include <stdio.h>

struct Status
{
    unsigned int isOn : 1;
    unsigned int isReady : 1;
    unsigned int mode : 2;
};

int main(void)
{
    struct Status s = {1, 0, 2};

    printf("On: %u\n", s.isOn);
    printf("Ready: %u\n", s.isReady);
    printf("Mode: %u\n", s.mode);

    return 0;
}
```

**Output:**

```
On: 1
Ready: 0
Mode: 2
```

A 1-bit unsigned field can represent:

\\[ 0 \text{ or } 1 \\]

A 2-bit unsigned field can represent:

\\[ 0,1,2,3 \\]

In general, an unsigned bit-field of width \\(n\\) can represent:

\\[ 0 \text{ through } 2^n-1 \\]

⚠ **Examiner’s flag:**

- Bit-field allocation order within a storage unit is implementation-defined.
- The exact size and alignment of a structure containing bit-fields are implementation-dependent.
- You cannot apply `&` to a bit-field because a bit-field is not addressable in the ordinary way.
- Do not assume a bit-field layout is portable across compilers or hardware architectures.


### 3.5.2 Typedef


[DIRECTLY IN NOTES]

The `typedef` keyword creates an alternative name, or alias, for an existing type.

**Syntax:**

```
typedef existing_type new_name;
```

Example:

```
#include <stdio.h>

typedef unsigned int uint;

int main(void)
{
    uint age = 20;

    printf("%u\n", age);

    return 0;
}
```

**Output:**

```
20
```

### Typedef with structures

Without `typedef`:

```
struct Student
{
    int roll;
};

struct Student s1;
```

With `typedef`:

```
typedef struct
{
    int roll;
} Student;

Student s1;
```

Complete example:

```
#include <stdio.h>

typedef struct
{
    int roll;
    float marks;
} Student;

int main(void)
{
    Student s1 = {101, 89.5f};

    printf("%d %.2f\n", s1.roll, s1.marks);

    return 0;
}
```

**Output:**

```
101 89.50
```

⚠ **Examiner’s flag:** `typedef` does not create a new, distinct data type in the same sense as defining a new structure or enumeration. It introduces an alias for an existing type.


### 3.5.3 Enumeration


[DIRECTLY IN NOTES]

An enumeration, declared using `enum`, defines a set of named integer constants.

**Syntax:**

```
enum enum_name
{
    constant1,
    constant2,
    constant3
};
```

Example:

```
#include <stdio.h>

enum Day
{
    MONDAY,
    TUESDAY,
    WEDNESDAY,
    THURSDAY,
    FRIDAY
};

int main(void)
{
    enum Day today = WEDNESDAY;

    printf("%d\n", today);

    return 0;
}
```

**Output:**

```
2
```

By default, enumeration constants start at zero and increase by one.

```
MONDAY     = 0
TUESDAY    = 1
WEDNESDAY  = 2
THURSDAY   = 3
FRIDAY     = 4
```

### Explicit enumeration values

```
enum Status
{
    FAILED = 0,
    PASSED = 1,
    PENDING = 5
};
```

Example:

```
#include <stdio.h>

enum Status
{
    FAILED = 0,
    PASSED = 1,
    PENDING = 5
};

int main(void)
{
    enum Status result = PENDING;

    printf("%d\n", result);

    return 0;
}
```

**Output:**

```
5
```

⚠ **Examiner’s flag:** An enum constant is an integer constant. Printing an enum value with `%d` is appropriate after the usual integer promotions.


## CHAPTER 3.6: DYNAMIC MEMORY ALLOCATION



### 3.6.1 Introduction


[DIRECTLY IN NOTES]

**Dynamic Memory Allocation (DMA)** allows a program to request memory during execution rather than requiring every memory size to be fixed at compile time.

The standard C library provides dynamic memory allocation functions in:

```
#include <stdlib.h>
```

The four key functions are:

1. `malloc()`
2. `calloc()`
3. `realloc()`
4. `free()`

Dynamic allocation is useful when:

- The number of elements is not known in advance.
- Memory requirements depend on user input.
- Data structures need to grow or shrink.
- The program must manage memory during execution.


### 3.6.2 Heap memory concept


[EXAM SUPPORT]

A simplified conceptual process-memory diagram:

```
+----------------------------------+
|              Stack               |
|       Local automatic data       |
|                                  |
+----------------------------------+
|                                  |
|               Heap               |
|     Dynamically allocated data   |
|                                  |
+----------------------------------+
|             Data area            |
|     Global and static objects    |
+----------------------------------+
|             Code area            |
|      Program instructions        |
+----------------------------------+
```

Simplified conceptual diagram. Actual process memory layout varies by operating system, executable format, compiler and runtime.


### 3.6.3 malloc() function


[DIRECTLY IN NOTES]

`malloc()` allocates a block of memory of the requested size.

**Syntax:**

```
ptr = malloc(number_of_bytes);
```

The return type is `void *`.

In C, a `void *` can be assigned to an object pointer without an explicit cast.

Example:

```
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    int *ptr;
    int n = 5;

    ptr = malloc(n * sizeof *ptr);

    if (ptr == NULL)
    {
        printf("Memory allocation failed.\n");
        return 1;
    }

    for (int i = 0; i < n; i++)
    {
        ptr[i] = (i + 1) * 10;
    }

    for (int i = 0; i < n; i++)
    {
        printf("%d ", ptr[i]);
    }

    free(ptr);

    return 0;
}
```

**Output:**

```
10 20 30 40 50
```

Important characteristics:

- Allocates a block of memory.
- Returns a pointer to the allocated block on success.
- Returns `NULL` if allocation fails.
- The allocated bytes have indeterminate contents.
- The memory must eventually be released using `free()` when no longer needed.

⚠ **Examiner’s flag:** Do not assume memory returned by `malloc()` is initialized to zero.


### 3.6.4 calloc() function


[DIRECTLY IN NOTES]

`calloc()` allocates memory for an array of elements and initializes all allocated bytes to zero.

**Syntax:**

```
ptr = calloc(number_of_elements, size_of_each_element);
```

Example:

```
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    int n = 5;

    int *ptr = calloc(n, sizeof *ptr);

    if (ptr == NULL)
    {
        printf("Memory allocation failed.\n");
        return 1;
    }

    for (int i = 0; i < n; i++)
    {
        printf("%d ", ptr[i]);
    }

    free(ptr);

    return 0;
}
```

**Output:**

```
0 0 0 0 0
```

### malloc() versus calloc()

| Feature        | `malloc()`                                | `calloc()`                          |
| -------------- | ----------------------------------------- | ----------------------------------- |
| Arguments      | One                                       | Two                                 |
| Allocation     | One block of specified bytes              | Space for an array of elements      |
| Initialization | Allocated bytes have indeterminate values | All allocated bytes are set to zero |
| Return type    | `void *`                                  | `void *`                            |
| Failure        | Returns `NULL`                            | Returns `NULL`                      |

⚠ **Examiner’s flag:** `calloc()` zeroes bytes. Although this commonly produces zero-valued integers and floating-point values on modern systems, the C standard's guarantee is about the bytes, not a universal semantic initialization of every possible object type.


### 3.6.5 realloc() function


[DIRECTLY IN NOTES]

`realloc()` changes the size of an existing dynamically allocated block.

**Syntax:**

```
new_ptr = realloc(old_ptr, new_size);
```

It may:

- Extend the existing block.
- Shrink the existing block.
- Move the block to a new location.
- Fail, leaving the original allocation unchanged.

Example:

```
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    int *ptr;
    int n = 3;

    ptr = malloc(n * sizeof *ptr);

    if (ptr == NULL)
    {
        printf("Initial allocation failed.\n");
        return 1;
    }

    for (int i = 0; i < n; i++)
    {
        ptr[i] = (i + 1) * 10;
    }

    int newSize = 5;

    int *temp = realloc(ptr, newSize * sizeof *ptr);

    if (temp == NULL)
    {
        printf("Reallocation failed.\n");
        free(ptr);
        return 1;
    }

    ptr = temp;

    ptr[3] = 40;
    ptr[4] = 50;

    for (int i = 0; i < newSize; i++)
    {
        printf("%d ", ptr[i]);
    }

    free(ptr);

    return 0;
}
```

**Output:**

```
10 20 30 40 50
```

### Safe realloc() pattern

[RESTORED STANDARD EQUATION / CODE]

Always store the result of `realloc()` in a temporary pointer.

```
int *temp = realloc(ptr, new_size);

if (temp != NULL)
{
    ptr = temp;
}
else
{
    /* Original ptr remains valid. */
}
```

⚠ **Examiner’s flag:** Writing `ptr = realloc(ptr, new_size);` directly can lose the original pointer if reallocation fails, causing a memory leak.

For a nonzero requested size, if `realloc()` fails, the original allocation remains valid and unchanged.

The special case of `realloc(ptr, 0)` has portability and version-specific complications. Prefer explicit `free(ptr)` when you intend to release the allocation.


### 3.6.6 free() function


[DIRECTLY IN NOTES]

`free()` releases memory previously allocated dynamically.

**Syntax:**

```
free(ptr);
```

Example:

```
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    int *ptr = malloc(5 * sizeof *ptr);

    if (ptr == NULL)
    {
        return 1;
    }

    ptr[0] = 100;

    printf("%d\n", ptr[0]);

    free(ptr);
    ptr = NULL;

    return 0;
}
```

**Output:**

```
100
```

After calling `free()`, the pointer must not be dereferenced.

Setting the pointer to `NULL` can prevent accidental reuse through that pointer variable.

⚠ **Examiner’s flag:** Setting one pointer to `NULL` does not automatically set other pointers that refer to the same allocation to `NULL`.


### 3.6.7 Dynamic memory allocation comparison


| Function    | Purpose                      | Initialization                                                     |
| ----------- | ---------------------------- | ------------------------------------------------------------------ |
| `malloc()`  | Allocate a block             | Indeterminate bytes                                                |
| `calloc()`  | Allocate an array-like block | All bytes zero                                                     |
| `realloc()` | Resize a block               | Preserves existing contents up to the smaller of old and new sizes |
| `free()`    | Release a block              | Not applicable                                                     |


### 3.6.8 Common dynamic memory errors


[EXAM SUPPORT]

| Error              | Meaning                                                            |
| ------------------ | ------------------------------------------------------------------ |
| Memory leak        | Allocated memory is never released                                 |
| Dangling pointer   | Pointer refers to an object whose lifetime has ended               |
| Double free        | Same allocation is released more than once                         |
| Invalid free       | Passing a pointer not returned by a compatible allocation function |
| Buffer overflow    | Accessing beyond allocated memory                                  |
| Use after free     | Accessing memory after it has been released                        |
| Allocation failure | Not checking whether allocation returned `NULL`                    |

### Example of a memory leak

```
int *p = malloc(10 * sizeof *p);

/* Use p */

p = NULL;   /* Memory address lost: allocation leaked */
```

Correct approach:

```
int *p = malloc(10 * sizeof *p);

if (p != NULL)
{
    /* Use p */

    free(p);
    p = NULL;
}
```


### 3.6.9 Dynamic memory allocation versus static allocation


| Static/fixed allocation                                                   | Dynamic allocation                                     |
| ------------------------------------------------------------------------- | ------------------------------------------------------ |
| Size is generally determined before execution or fixed by the declaration | Size can be selected during execution                  |
| Managed according to declared storage duration                            | Managed explicitly through allocation and deallocation |
| Examples: fixed-size local arrays, global arrays                          | Examples: memory from `malloc()` and `calloc()`        |
| No explicit `free()` for ordinary declared objects                        | Must release allocated memory when no longer required  |


# UNIT 3: EXAM-ORIENTED PROGRAMMING PRACTICE


The following programs combine pointers, arrays, functions, structures, unions, storage classes and dynamic memory allocation. They are written in standard C style and include input validation where it is important.


## CHAPTER 3.7: 15 SOLVED HIGH-YIELD C PROGRAMS



### Program 1: Swap two numbers using pointers


**Concepts:** Pointers, dereferencing, function arguments.

**Problem:** Write a C program to swap two numbers using a function and pointers.

**Logic:** Pass the addresses of the two variables. The function uses dereferencing to modify the original variables.

```
#include <stdio.h>

void swap(int *a, int *b)
{
    int temp = *a;

    *a = *b;
    *b = temp;
}

int main(void)
{
    int x, y;

    printf("Enter two numbers: ");

    if (scanf("%d %d", &x, &y) != 2)
    {
        printf("Invalid input.\n");
        return 1;
    }

    printf("Before swapping: x = %d, y = %d\n", x, y);

    swap(&x, &y);

    printf("After swapping: x = %d, y = %d\n", x, y);

    return 0;
}
```

**Sample input:**

```
10 20
```

**Output:**

```
Before swapping: x = 10, y = 20
After swapping: x = 20, y = 10
```

**Dry run:**

| Step        | `*a` | `*b` | `temp`       |
| ----------- | ---- | ---- | ------------ |
| Initial     | 10   | 20   | Not assigned |
| `temp = *a` | 10   | 20   | 10           |
| `*a = *b`   | 20   | 20   | 10           |
| `*b = temp` | 20   | 10   | 10           |

**Complexity:**

\\[ T(n)=O(1),\qquad S(n)=O(1) \\]


### Program 2: Find the sum and average of an array using pointers


**Concepts:** Array-pointer relationship, pointer arithmetic, loops.

```
#include <stdio.h>

int main(void)
{
    int n;
    int arr[100];
    int sum = 0;

    printf("Enter number of elements: ");

    if (scanf("%d", &n) != 1 || n < 1 || n > 100)
    {
        printf("Invalid size.\n");
        return 1;
    }

    printf("Enter elements:\n");

    for (int i = 0; i < n; i++)
    {
        if (scanf("%d", &arr[i]) != 1)
        {
            printf("Invalid input.\n");
            return 1;
        }
    }

    int *ptr = arr;

    for (int i = 0; i < n; i++)
    {
        sum += *(ptr + i);
    }

    double average = (double)sum / n;

    printf("Sum = %d\n", sum);
    printf("Average = %.2f\n", average);

    return 0;
}
```

**Sample input:**

```
5
10 20 30 40 50
```

**Output:**

```
Sum = 150
Average = 30.00
```

**Dry run:**

| Iteration | `*(ptr+i)` | Sum |
| --------- | ---------- | --- |
| 0         | 10         | 10  |
| 1         | 20         | 30  |
| 2         | 30         | 60  |
| 3         | 40         | 100 |
| 4         | 50         | 150 |

**Complexity:**

\\[ T(n)=O(n),\qquad S(n)=O(1) \\]

The fixed-size array has capacity 100. The algorithm uses constant auxiliary space.


### Program 3: Reverse an array using pointers


**Concepts:** Pointers, two-pointer technique, swapping.

```
#include <stdio.h>

int main(void)
{
    int n;
    int arr[100];

    printf("Enter number of elements: ");

    if (scanf("%d", &n) != 1 || n < 1 || n > 100)
    {
        printf("Invalid size.\n");
        return 1;
    }

    printf("Enter elements:\n");

    for (int i = 0; i < n; i++)
    {
        if (scanf("%d", &arr[i]) != 1)
        {
            printf("Invalid input.\n");
            return 1;
        }
    }

    int *left = arr;
    int *right = arr + n - 1;

    while (left < right)
    {
        int temp = *left;

        *left = *right;
        *right = temp;

        left++;
        right--;
    }

    printf("Reversed array:\n");

    for (int i = 0; i < n; i++)
    {
        printf("%d ", arr[i]);
    }

    printf("\n");

    return 0;
}
```

**Sample input:**

```
5
10 20 30 40 50
```

**Output:**

```
50 40 30 20 10
```

**Dry run:**

| Step    | Left value | Right value | Array          |
| ------- | ---------- | ----------- | -------------- |
| Initial | 10         | 50          | 10 20 30 40 50 |
| 1       | 10         | 50          | 50 20 30 40 10 |
| 2       | 20         | 40          | 50 40 30 20 10 |
| Stop    | 30         | 30          | 50 40 30 20 10 |

**Complexity:**

\\[ T(n)=O(n),\qquad S(n)=O(1) \\]


### Program 4: Find the largest element using a pointer


**Concepts:** Pointers, array traversal, comparison.

```
#include <stdio.h>

int main(void)
{
    int n;
    int arr[100];

    printf("Enter number of elements: ");

    if (scanf("%d", &n) != 1 || n < 1 || n > 100)
    {
        printf("Invalid size.\n");
        return 1;
    }

    printf("Enter elements:\n");

    for (int i = 0; i < n; i++)
    {
        if (scanf("%d", &arr[i]) != 1)
        {
            printf("Invalid input.\n");
            return 1;
        }
    }

    int *ptr = arr;
    int largest = *ptr;

    for (int i = 1; i < n; i++)
    {
        if (*(ptr + i) > largest)
        {
            largest = *(ptr + i);
        }
    }

    printf("Largest element = %d\n", largest);

    return 0;
}
```

**Sample input:**

```
5
12 45 23 67 34
```

**Output:**

```
Largest element = 67
```

**Dry run:**

| Current element | Largest |
| --------------- | ------- |
| 12              | 12      |
| 45              | 45      |
| 23              | 45      |
| 67              | 67      |
| 34              | 67      |

**Complexity:**

\\[ T(n)=O(n),\qquad S(n)=O(1) \\]


### Program 5: Demonstrate static storage class


**Concepts:** Static local variable, lifetime, function calls.

```
#include <stdio.h>

void countCalls(void)
{
    static int count = 0;

    count++;

    printf("Function called %d times\n", count);
}

int main(void)
{
    countCalls();
    countCalls();
    countCalls();
    countCalls();
    countCalls();

    return 0;
}
```

**Output:**

```
Function called 1 times
Function called 2 times
Function called 3 times
Function called 4 times
Function called 5 times
```

**Dry run:**

| Function call | Initial count | After increment |
| ------------- | ------------- | --------------- |
| 1             | 0             | 1               |
| 2             | 1             | 2               |
| 3             | 2             | 3               |
| 4             | 3             | 4               |
| 5             | 4             | 5               |

**Complexity per call:**

\\[ T(n)=O(1),\qquad S(n)=O(1) \\]


### Program 6: Store and display student records using structures


**Concepts:** Structures, arrays of structures, member access.

```
#include <stdio.h>

struct Student
{
    int roll;
    char name[50];
    float marks;
};

int main(void)
{
    struct Student s[100];
    int n;

    printf("Enter number of students: ");

    if (scanf("%d", &n) != 1 || n < 1 || n > 100)
    {
        printf("Invalid number of students.\n");
        return 1;
    }

    for (int i = 0; i < n; i++)
    {
        printf("\nStudent %d\n", i + 1);

        printf("Enter roll number: ");

        if (scanf("%d", &s[i].roll) != 1)
        {
            printf("Invalid roll number.\n");
            return 1;
        }

        printf("Enter name (one word): ");

        if (scanf("%49s", s[i].name) != 1)
        {
            printf("Invalid name.\n");
            return 1;
        }

        printf("Enter marks: ");

        if (scanf("%f", &s[i].marks) != 1)
        {
            printf("Invalid marks.\n");
            return 1;
        }
    }

    printf("\nStudent Records\n");

    for (int i = 0; i < n; i++)
    {
        printf("%d %s %.2f\n",
               s[i].roll,
               s[i].name,
               s[i].marks);
    }

    return 0;
}
```

**Sample input:**

```
2
101
Aman
85.5
102
Riya
91
```

**Output:**

```
Student Records
101 Aman 85.50
102 Riya 91.00
```

**Complexity:**

\\[ T(n)=O(n),\qquad S(n)=O(n) \\]

The program stores \\(n\\) student records.


### Program 7: Calculate total and average marks using a structure


**Concepts:** Structure members, arrays, aggregation.

```
#include <stdio.h>

struct Student
{
    int roll;
    char name[50];
    float marks[5];
    float total;
    float average;
};

int main(void)
{
    struct Student s;

    s.total = 0.0f;

    printf("Enter roll number: ");

    if (scanf("%d", &s.roll) != 1)
    {
        printf("Invalid input.\n");
        return 1;
    }

    printf("Enter name (one word): ");

    if (scanf("%49s", s.name) != 1)
    {
        printf("Invalid name.\n");
        return 1;
    }

    printf("Enter marks in five subjects:\n");

    for (int i = 0; i < 5; i++)
    {
        if (scanf("%f", &s.marks[i]) != 1)
        {
            printf("Invalid marks.\n");
            return 1;
        }

        s.total += s.marks[i];
    }

    s.average = s.total / 5.0f;

    printf("\nRoll Number: %d\n", s.roll);
    printf("Name: %s\n", s.name);
    printf("Total: %.2f\n", s.total);
    printf("Average: %.2f\n", s.average);

    return 0;
}
```

**Sample input:**

```
101
Aman
80 90 85 95 100
```

**Output:**

```
Roll Number: 101
Name: Aman
Total: 450.00
Average: 90.00
```

**Formula:**

\\[ \text{Total}=\sum\_{i=1}^{5}m_i \\]

\\[ \text{Average}=\frac{\text{Total}}{5} \\]

**Complexity:**

\\[ T(n)=O(1),\qquad S(n)=O(1) \\]

The number of subjects is fixed at five.


### Program 8: Demonstrate structure pointer and arrow operator


**Concepts:** Structure pointer, `->` operator, dereferencing.

```
#include <stdio.h>

struct Employee
{
    int id;
    float salary;
};

int main(void)
{
    struct Employee e = {1001, 35000.0f};

    struct Employee *ptr = &e;

    printf("Employee ID: %d\n", ptr->id);
    printf("Salary: %.2f\n", ptr->salary);

    ptr->salary = 40000.0f;

    printf("Updated Salary: %.2f\n", e.salary);

    return 0;
}
```

**Output:**

```
Employee ID: 1001
Salary: 35000.00
Updated Salary: 40000.00
```

Equivalent member-access expressions:

```
ptr->salary
(*ptr).salary
```

**Complexity:**

\\[ T(n)=O(1),\qquad S(n)=O(1) \\]


### Program 9: Demonstrate union memory sharing


**Concepts:** Union declaration, shared memory, member access.

```
#include <stdio.h>

union Data
{
    int i;
    float f;
    char ch;
};

int main(void)
{
    union Data d;

    printf("Size of union = %zu bytes\n", sizeof d);

    d.i = 100;
    printf("Integer = %d\n", d.i);

    d.f = 25.5f;
    printf("Float = %.2f\n", d.f);

    d.ch = 'A';
    printf("Character = %c\n", d.ch);

    return 0;
}
```

**Output:** The values are:

```
Integer = 100
Float = 25.50
Character = A
```

The size line depends on the implementation.

**Conceptual dry run:**

| Operation     | Active member intended by the program | Stored value |
| ------------- | ------------------------------------- | ------------ |
| `d.i = 100`   | `i`                                   | 100          |
| `d.f = 25.5f` | `f`                                   | 25.5         |
| `d.ch = 'A'`  | `ch`                                  | A            |

⚠ **Examiner’s flag:** Do not print `d.i` after writing `d.f` and assume the previous integer value is still available. Union members overlap.


### Program 10: Demonstrate typedef and enum


**Concepts:** Type alias, enumeration constants, switch.

```
#include <stdio.h>

typedef enum
{
    RED = 1,
    GREEN,
    BLUE
} Color;

int main(void)
{
    Color selected = GREEN;

    switch (selected)
    {
        case RED:
            printf("Red selected\n");
            break;

        case GREEN:
            printf("Green selected\n");
            break;

        case BLUE:
            printf("Blue selected\n");
            break;

        default:
            printf("Invalid color\n");
    }

    return 0;
}
```

**Output:**

```
Green selected
```

**Dry run:**

```
RED   = 1
GREEN = 2
BLUE  = 3

selected = GREEN
selected = 2

switch(2)
    -> case GREEN
    -> print "Green selected"
```

**Complexity:**

\\[ T(n)=O(1),\qquad S(n)=O(1) \\]


### Program 11: Allocate an integer array using malloc()


**Concepts:** Dynamic memory allocation, `malloc()`, `free()`.

```
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    int n;

    printf("Enter number of elements: ");

    if (scanf("%d", &n) != 1 || n <= 0)
    {
        printf("Invalid size.\n");
        return 1;
    }

    int *arr = malloc((size_t)n * sizeof *arr);

    if (arr == NULL)
    {
        printf("Memory allocation failed.\n");
        return 1;
    }

    printf("Enter elements:\n");

    for (int i = 0; i < n; i++)
    {
        if (scanf("%d", &arr[i]) != 1)
        {
            printf("Invalid input.\n");
            free(arr);
            return 1;
        }
    }

    printf("Array elements:\n");

    for (int i = 0; i < n; i++)
    {
        printf("%d ", arr[i]);
    }

    printf("\n");

    free(arr);
    arr = NULL;

    return 0;
}
```

**Sample input:**

```
4
10 20 30 40
```

**Output:**

```
Array elements:
10 20 30 40
```

**Memory concept:**

```
arr
 |
 v
+------+------+------+------+
|  10  |  20  |  30  |  40  |
+------+------+------+------+
   Dynamically allocated memory

After free(arr):
The allocation is released.
arr is then set to NULL.
```

**Complexity:**

\\[ T(n)=O(n),\qquad S(n)=O(n) \\]


### Program 12: Calculate the sum and average using calloc()


**Concepts:** `calloc()`, zero-initialized bytes, dynamic array.

```
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    int n;
    long long sum = 0;

    printf("Enter number of elements: ");

    if (scanf("%d", &n) != 1 || n <= 0)
    {
        printf("Invalid size.\n");
        return 1;
    }

    int *arr = calloc((size_t)n, sizeof *arr);

    if (arr == NULL)
    {
        printf("Memory allocation failed.\n");
        return 1;
    }

    printf("Enter elements:\n");

    for (int i = 0; i < n; i++)
    {
        if (scanf("%d", &arr[i]) != 1)
        {
            printf("Invalid input.\n");
            free(arr);
            return 1;
        }

        sum += arr[i];
    }

    printf("Sum = %lld\n", sum);
    printf("Average = %.2f\n", (double)sum / n);

    free(arr);

    return 0;
}
```

**Sample input:**

```
4
10 20 30 40
```

**Output:**

```
Sum = 100
Average = 25.00
```

**Complexity:**

\\[ T(n)=O(n),\qquad S(n)=O(n) \\]


### Program 13: Resize an array using realloc()


**Concepts:** `realloc()`, temporary pointer, memory resizing.

```
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    int n, newSize;

    printf("Enter initial size: ");

    if (scanf("%d", &n) != 1 || n <= 0)
    {
        printf("Invalid size.\n");
        return 1;
    }

    int *arr = malloc((size_t)n * sizeof *arr);

    if (arr == NULL)
    {
        printf("Allocation failed.\n");
        return 1;
    }

    printf("Enter elements:\n");

    for (int i = 0; i < n; i++)
    {
        if (scanf("%d", &arr[i]) != 1)
        {
            printf("Invalid input.\n");
            free(arr);
            return 1;
        }
    }

    printf("Enter new size: ");

    if (scanf("%d", &newSize) != 1 || newSize <= 0)
    {
        printf("Invalid new size.\n");
        free(arr);
        return 1;
    }

    int *temp = realloc(
        arr,
        (size_t)newSize * sizeof *arr
    );

    if (temp == NULL)
    {
        printf("Reallocation failed.\n");
        free(arr);
        return 1;
    }

    arr = temp;

    if (newSize > n)
    {
        printf("Enter %d additional elements:\n", newSize - n);

        for (int i = n; i < newSize; i++)
        {
            if (scanf("%d", &arr[i]) != 1)
            {
                printf("Invalid input.\n");
                free(arr);
                return 1;
            }
        }
    }

    printf("Updated array:\n");

    for (int i = 0; i < newSize; i++)
    {
        printf("%d ", arr[i]);
    }

    printf("\n");

    free(arr);

    return 0;
}
```

**Sample input:**

```
3
10 20 30
5
40 50
```

**Output:**

```
Updated array:
10 20 30 40 50
```

**Complexity:**

- Reading and displaying elements: \\(O(n+m)\\), where \\(m\\) is the new size.
- Reallocation: implementation-dependent; it may move the block and copy data.
- Auxiliary space: \\(O(1)\\), excluding the dynamically allocated array.


### Program 14: Find the sum of two matrices using dynamic memory allocation


**Concepts:** Two-dimensional arrays, dynamic memory, pointer-to-pointer representation.

This program allocates each row separately.

```
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    int rows, cols;

    printf("Enter rows and columns: ");

    if (scanf("%d %d", &rows, &cols) != 2 ||
        rows <= 0 || cols <= 0)
    {
        printf("Invalid dimensions.\n");
        return 1;
    }

    int **a = malloc((size_t)rows * sizeof *a);
    int **b = malloc((size_t)rows * sizeof *b);
    int **sum = malloc((size_t)rows * sizeof *sum);

    if (a == NULL || b == NULL || sum == NULL)
    {
        printf("Memory allocation failed.\n");
        free(a);
        free(b);
        free(sum);
        return 1;
    }

    int allocatedA = 0;
    int allocatedB = 0;
    int allocatedSum = 0;

    for (int i = 0; i < rows; i++)
    {
        a[i] = NULL;
        b[i] = NULL;
        sum[i] = NULL;
    }

    for (int i = 0; i < rows; i++)
    {
        a[i] = malloc((size_t)cols * sizeof *a[i]);
        if (a[i] == NULL)
        {
            printf("Allocation failed.\n");
            goto cleanup;
        }
        allocatedA++;

        b[i] = malloc((size_t)cols * sizeof *b[i]);
        if (b[i] == NULL)
        {
            printf("Allocation failed.\n");
            goto cleanup;
        }
        allocatedB++;

        sum[i] = malloc((size_t)cols * sizeof *sum[i]);
        if (sum[i] == NULL)
        {
            printf("Allocation failed.\n");
            goto cleanup;
        }
        allocatedSum++;
    }

    printf("Enter first matrix:\n");

    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            if (scanf("%d", &a[i][j]) != 1)
            {
                printf("Invalid input.\n");
                goto cleanup;
            }
        }
    }

    printf("Enter second matrix:\n");

    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            if (scanf("%d", &b[i][j]) != 1)
            {
                printf("Invalid input.\n");
                goto cleanup;
            }
        }
    }

    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            sum[i][j] = a[i][j] + b[i][j];
        }
    }

    printf("Sum matrix:\n");

    for (int i = 0; i < rows; i++)
    {
        for (int j = 0; j < cols; j++)
        {
            printf("%d ", sum[i][j]);
        }

        printf("\n");
    }

cleanup:

    for (int i = 0; i < allocatedA; i++)
        free(a[i]);

    for (int i = 0; i < allocatedB; i++)
        free(b[i]);

    for (int i = 0; i < allocatedSum; i++)
        free(sum[i]);

    free(a);
    free(b);
    free(sum);

    return 0;
}
```

**Sample input:**

```
2 2
1 2
3 4
5 6
7 8
```

**Output:**

```
Sum matrix:
6 8
10 12
```

**Formula:**

\\[ C\_{ij}=A\_{ij}+B\_{ij} \\]

**Complexity:**

\\[ T(r,c)=O(rc),\qquad S(r,c)=O(rc) \\]

⚠ **Examiner’s flag:** This implementation uses separately allocated rows. It is not one contiguous two-dimensional array allocation. A pointer-to-pointer matrix and a true two-dimensional array are different memory layouts.


### Program 15: Demonstrate a structure containing a dynamically allocated string


**Concepts:** Structures, pointers, `malloc()`, `free()`, dynamic string storage.

```
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

struct Student
{
    int roll;
    char *name;
};

int main(void)
{
    struct Student s;

    s.roll = 101;

    char input[100];

    printf("Enter student name: ");

    if (scanf("%99s", input) != 1)
    {
        printf("Invalid input.\n");
        return 1;
    }

    size_t length = strlen(input);

    s.name = malloc((length + 1) * sizeof *s.name);

    if (s.name == NULL)
    {
        printf("Memory allocation failed.\n");
        return 1;
    }

    strcpy(s.name, input);

    printf("Roll Number: %d\n", s.roll);
    printf("Name: %s\n", s.name);

    free(s.name);
    s.name = NULL;

    return 0;
}
```

**Sample input:**

```
Aman
```

**Output:**

```
Roll Number: 101
Name: Aman
```

**Memory diagram:**

```
Structure object s
+----------------------+
| roll = 101           |
| name = address ------+------+
+----------------------+      |
                              v
                       Dynamic memory
                       +---+---+---+---+---+
                       | A | m | a | n |\0 |
                       +---+---+---+---+---+
```

The structure contains a pointer. The characters are stored in a separate dynamically allocated block.

**Complexity:**

For a name of length \\(n\\):

\\[ T(n)=O(n),\qquad S(n)=O(n) \\]


## CHAPTER 3.8: COMMON MISTAKES AND DEBUGGING TRAPS


This section collects frequent errors in C programming, particularly those that appear in practical examinations, output-prediction questions, debugging questions and viva examinations.


### 3.8.1 Pointer-related mistakes


| Incorrect code              | Problem                                          | Correct approach                                |
| --------------------------- | ------------------------------------------------ | ----------------------------------------------- |
| `int *p; *p = 10;`          | Dereferencing an uninitialized pointer           | Initialize `p` with a valid address             |
| `int *p = NULL; *p = 5;`    | Dereferencing a null pointer                     | Allocate or assign a valid object address       |
| `p = x;`                    | Assigning an integer value to an integer pointer | Use `p = &x;`                                   |
| `printf("%d", p);`          | Wrong format specifier for an address            | Use `printf("%p", (void *)p);`                  |
| `arr++;`                    | Array name is not a modifiable pointer           | Use a separate pointer variable                 |
| `*p++;`                     | Increments the pointer after dereferencing       | Use `(*p)++;` to increment the pointed-to value |
| `p + 1` treated as one byte | Incorrect pointer arithmetic assumption          | It advances by `sizeof(*p)` bytes               |
| `free(p); *p = 5;`          | Use after free                                   | Do not access the allocation after freeing it   |

### Important operator-precedence trap

Compare these expressions:

```
*p++;
(*p)++;
*++p;
++*p;
```

| Expression | Meaning                                                          |
| ---------- | ---------------------------------------------------------------- |
| `*p++`     | Access current pointed-to value, then advance `p`                |
| `(*p)++`   | Increment the value pointed to by `p`                            |
| `*++p`     | Advance `p`, then access the new pointed-to value                |
| `++*p`     | Increment the pointed-to value and produce the incremented value |

Example:

```
#include <stdio.h>

int main(void)
{
    int a[] = {10, 20, 30};
    int *p = a;

    printf("%d\n", *p++);
    printf("%d\n", *p);

    return 0;
}
```

**Output:**

```
10
20
```

The first expression prints the original value and then advances the pointer.


### 3.8.2 Array-related mistakes


| Mistake                                       | Explanation                                                  |
| --------------------------------------------- | ------------------------------------------------------------ |
| Accessing `arr[n]` in an array of size `n`    | Valid indexes are `0` through `n-1`                          |
| Writing `i <= n` in a traversal loop          | Usually causes one extra access                              |
| Using an uninitialized array                  | Reading indeterminate elements can cause undefined behaviour |
| Forgetting array capacity                     | Input may exceed available storage                           |
| Using `sizeof(arr)` inside an array parameter | The parameter is adjusted to a pointer type                  |
| Assigning one array to another using `a = b`  | Whole-array assignment is not allowed                        |

Correct traversal:

```
for (int i = 0; i < n; i++)
{
    printf("%d ", arr[i]);
}
```

Incorrect traversal:

```
for (int i = 0; i <= n; i++)
{
    printf("%d ", arr[i]);
}
```

⚠ **Examiner’s flag:** An out-of-bounds array access is undefined behaviour. It may appear to work, print unexpected data, corrupt memory or crash.


### 3.8.3 String-related mistakes


| Mistake                             | Problem                                            | Correction                                          |
| ----------------------------------- | -------------------------------------------------- | --------------------------------------------------- |
| `char name[5] = "Hello";`           | Requires space for six characters including `'\0'` | Use `char name[6]`                                  |
| `name1 = name2;`                    | Arrays cannot be assigned directly                 | Use `strcpy()` with sufficient destination capacity |
| `strcmp(a,b) == 1` to test equality | `strcmp()` is not guaranteed to return exactly 1   | Test `strcmp(a,b) == 0`                             |
| `gets(name);`                       | Unsafe and removed from modern standard C          | Use `fgets()`                                       |
| Forgetting the null terminator      | String functions may read beyond the array         | Ensure the string ends with `'\0'`                  |
| Using `%s` for a full sentence      | Input stops at whitespace                          | Use `fgets()`                                       |

⚠ **Examiner’s flag:** The destination array in `strcpy()` must be large enough for the source string and its null terminator.


### 3.8.4 Function-related mistakes


| Mistake                                                 | Explanation                                                               |
| ------------------------------------------------------- | ------------------------------------------------------------------------- |
| Calling a function without a valid declaration          | May cause a diagnostic or constraint violation                            |
| Returning no value from a non-void function             | Invalid if the caller uses the missing result                             |
| Returning a local variable's address                    | The local object's lifetime ends when the function returns                |
| Confusing actual and formal arguments                   | Actual arguments appear in calls; formal parameters appear in definitions |
| Expecting call by value to modify the caller's variable | The function receives a copy                                              |
| Missing `break` in a switch                             | Execution may fall through to later cases                                 |

Example of a dangerous return:

```
int *getValue(void)
{
    int x = 10;

    return &x;  /* Invalid lifetime: dangling pointer */
}
```

Safer alternative:

```
int getValue(void)
{
    int x = 10;

    return x;
}
```

Or use dynamically allocated memory when the caller is responsible for releasing the returned allocation.


### 3.8.5 Storage-class mistakes


| Mistake                                               | Correction                                                               |
| ----------------------------------------------------- | ------------------------------------------------------------------------ |
| Assuming an automatic local variable starts at zero   | Initialize it explicitly                                                 |
| Assuming a static local variable resets on every call | It retains its value                                                     |
| Assuming `register` guarantees CPU-register storage   | It is only a request                                                     |
| Assuming `extern` creates a new variable              | It normally declares an object defined elsewhere                         |
| Confusing scope with lifetime                         | Scope is where a name is visible; lifetime is how long the object exists |


### 3.8.6 Structure and union mistakes


| Mistake                                                | Correction                                             |
| ------------------------------------------------------ | ------------------------------------------------------ |
| Using `.` with a structure pointer                     | Use `->` or `(*ptr).member`                            |
| Assuming structure size equals the sum of member sizes | Account for possible padding                           |
| Assuming all union members store independent values    | They share storage                                     |
| Comparing structures directly with `==`                | Compare members individually                           |
| Forgetting a structure variable declaration            | A structure definition alone does not create an object |
| Taking the address of a bit-field                      | Bit-fields are not addressable in the ordinary way     |


### 3.8.7 Dynamic memory mistakes


| Mistake                                               | Consequence                       | Correct approach                                |
| ----------------------------------------------------- | --------------------------------- | ----------------------------------------------- |
| Not checking `malloc()`                               | Possible null-pointer dereference | Check against `NULL`                            |
| Forgetting `free()`                                   | Memory leak                       | Release allocations when finished               |
| Freeing the same pointer twice                        | Undefined behaviour               | Free each allocation exactly once               |
| Using memory after `free()`                           | Undefined behaviour               | Stop accessing the allocation                   |
| Losing the original pointer during failed `realloc()` | Memory leak                       | Use a temporary pointer                         |
| Allocating too few bytes                              | Buffer overflow                   | Calculate size using `sizeof`                   |
| Freeing a local array                                 | Invalid free                      | Only free a valid dynamically allocated pointer |

Recommended allocation pattern:

```
int *ptr = malloc(n * sizeof *ptr);

if (ptr == NULL)
{
    printf("Allocation failed.\n");
    return 1;
}

/* Use allocated memory */

free(ptr);
ptr = NULL;
```


### 3.8.8 Compiler warnings and debugging


[EXAM SUPPORT]

Compile C programs with warnings enabled:

```
gcc -std=c11 -Wall -Wextra -Wpedantic program.c -o program
```

For additional runtime checks during development, when supported:

```
gcc -std=c11 -Wall -Wextra -g \
-fsanitize=address,undefined \
program.c -o program
```

Run:

```
./program
```

These options can help identify:

- Invalid memory accesses.
- Buffer overflows.
- Use-after-free errors.
- Some forms of undefined behaviour.
- Type mismatches and suspicious expressions.

They do not prove that a program is correct.

### Practical debugging procedure

1. Read the complete compiler error message.
2. Identify the exact line and column.
3. Check missing semicolons, braces and parentheses.
4. Check variable declarations and data types.
5. Verify loop initialization, condition and update.
6. Check array boundaries.
7. Check pointer initialization and validity.
8. Verify that every allocation is checked.
9. Verify that dynamically allocated memory is released.
10. Test normal, boundary and invalid inputs.


## CHAPTER 3.9: QUICK-REVISION CHEAT SHEET



### 3.9.1 Pointer syntax


| Expression  | Meaning                             |
| ----------- | ----------------------------------- |
| `int *p;`   | Declare integer pointer             |
| `p = &x;`   | Store address of `x`                |
| `*p`        | Access value pointed to by `p`      |
| `&x`        | Address of `x`                      |
| `p++`       | Move to next pointed-to element     |
| `p--`       | Move to previous pointed-to element |
| `p + n`     | Move forward by `n` elements        |
| `p - n`     | Move backward by `n` elements       |
| `int **p;`  | Pointer to pointer                  |
| `void *p;`  | Generic object pointer              |
| `p == NULL` | Check whether pointer is null       |


### 3.9.2 Pointer and array formulas


For a one-dimensional array:

\\[ arr[i]=\*(arr+i) \\]

For an element size of \\(w\\) bytes:

\\[ \operatorname{Address}(arr[i]) = \operatorname{BaseAddress}+i\times w \\]

For a two-dimensional array stored in row-major order:

\\[ \operatorname{Address}(A[i][j]) = B+(i\times C+j)\times w \\]

Where:

- \\(B\\) = base address
- \\(C\\) = number of columns
- \\(w\\) = size of each element in bytes
- \\(i\\) = row index
- \\(j\\) = column index

For a two-dimensional array declared as `A[R][C]`, the compiler uses row-major storage in C.


### 3.9.3 Storage-class quick table


| Keyword    | Main purpose                            | Key exam point                                    |
| ---------- | --------------------------------------- | ------------------------------------------------- |
| `auto`     | Ordinary local variable                 | Automatic storage duration                        |
| `register` | Register storage request                | Address operator restriction for register objects |
| `static`   | Persistent storage or internal linkage  | Local static retains value                        |
| `extern`   | Declaration of external object/function | Definition is elsewhere or later                  |


### 3.9.4 Structure and union quick table


| Feature                    | Structure                    | Union                                   |
| -------------------------- | ---------------------------- | --------------------------------------- |
| Memory                     | Separate member storage      | Shared member storage                   |
| Size                       | Includes members and padding | Enough for largest member and alignment |
| Simultaneous member values | Yes                          | Not generally independent               |
| Access operator            | `.`                          | `.`                                     |
| Pointer access             | `->`                         | `->`                                    |

Remember:

```
struct Student s;
struct Student *p = &s;

s.roll = 101;
p->roll = 102;
```


### 3.9.5 Dynamic memory allocation quick table


| Function    | Syntax                | Purpose                 |
| ----------- | --------------------- | ----------------------- |
| `malloc()`  | `malloc(bytes)`       | Allocate memory         |
| `calloc()`  | `calloc(count, size)` | Allocate and zero bytes |
| `realloc()` | `realloc(ptr, bytes)` | Resize allocation       |
| `free()`    | `free(ptr)`           | Release allocation      |

**Recommended allocation size expression:**

```
int *p = malloc(n * sizeof *p);
```

This is preferable to hardcoding the size of the pointed-to type.


### 3.9.6 Important string functions


Include:

```
#include <string.h>
```

| Function        | Purpose                                |
| --------------- | -------------------------------------- |
| `strlen(s)`     | Returns string length excluding `'\0'` |
| `strcpy(d,s)`   | Copies string into destination         |
| `strcat(d,s)`   | Appends source to destination          |
| `strcmp(a,b)`   | Compares two strings                   |
| `strchr(s,c)`   | Finds first occurrence of a character  |
| `strstr(s,sub)` | Finds a substring                      |

⚠ `strcpy()` and `strcat()` do not automatically resize their destination arrays. The destination must have sufficient capacity.


### 3.9.7 Format specifiers


[EXAM SUPPORT]

| Data type                   | Format specifier |
| --------------------------- | ---------------- |
| `char`                      | `%c`             |
| `int`                       | `%d`             |
| `unsigned int`              | `%u`             |
| `long int`                  | `%ld`            |
| `long long int`             | `%lld`           |
| `float`                     | `%f`             |
| `double` in `printf()`      | `%f`             |
| `double` in `scanf()`       | `%lf`            |
| `long double` in `printf()` | `%Lf`            |
| `char[]` string             | `%s`             |
| Pointer address             | `%p`             |
| `size_t`                    | `%zu`            |
| `ptrdiff_t`                 | `%td`            |

⚠ **Examiner’s flag:** In `printf()`, a `float` argument is promoted to `double`, so `%f` is used for both `float` and `double`. In `scanf()`, `%f` expects `float *`, while `%lf` expects `double *`.


### 3.9.8 Operator precedence quick reference


[EXAM SUPPORT]

The following table gives a useful simplified order from higher to lower precedence.

| Priority | Operators                                         | Description    | Associativity |
| -------- | ------------------------------------------------- | -------------- | ------------- |
| 1        | `()`, `[]`, `.`, `->`, `x++`, `x--`               | Postfix        | Left to right |
| 2        | `++x`, `--x`, `!`, `~`, `*`, `&`, `sizeof`, casts | Unary          | Right to left |
| 3        | `*`, `/`, `%`                                     | Multiplicative | Left to right |
| 4        | `+`, `-`                                          | Additive       | Left to right |
| 5        | `<<`, `>>`                                        | Shift          | Left to right |
| 6        | `<`, `<=`, `>`, `>=`                              | Relational     | Left to right |
| 7        | `==`, `!=`                                        | Equality       | Left to right |
| 8        | `&`                                               | Bitwise AND    | Left to right |
| 9        | `^`                                               | Bitwise XOR    | Left to right |
| 10       | `\\|`                                             | Bitwise OR     | Left to right |
| 11       | `&&`                                              | Logical AND    | Left to right |
| 12       | `\\|\\|`                                          | Logical OR     | Left to right |
| 13       | `?:`                                              | Conditional    | Right to left |
| 14       | `=`, `+=`, `-=`, `*=`, `/=`                       | Assignment     | Right to left |
| 15       | `,`                                               | Comma          | Left to right |

⚠ **Examiner’s flag:** Precedence determines grouping, not necessarily the order in which operands are evaluated. Do not assume that every expression evaluates strictly from left to right.


### 3.9.9 Time complexity reference table


[EXAM SUPPORT]

| Complexity       | Name         | Typical example             |
| ---------------- | ------------ | --------------------------- |
| \\(O(1)\\)       | Constant     | Accessing an array element  |
| \\(O(\log n)\\)  | Logarithmic  | Binary search               |
| \\(O(n)\\)       | Linear       | Traversing an array         |
| \\(O(n\log n)\\) | Linearithmic | Merge sort                  |
| \\(O(n^2)\\)     | Quadratic    | Bubble sort, selection sort |
| \\(O(n^3)\\)     | Cubic        | Basic matrix multiplication |
| \\(O(2^n)\\)     | Exponential  | Naive recursive Fibonacci   |
| \\(O(n!)\\)      | Factorial    | Generating all permutations |

### Sorting algorithm comparison

| Algorithm                   | Best case        | Average case     | Worst case       | Auxiliary space            |
| --------------------------- | ---------------- | ---------------- | ---------------- | -------------------------- |
| Bubble sort with early exit | \\(O(n)\\)       | \\(O(n^2)\\)     | \\(O(n^2)\\)     | \\(O(1)\\)                 |
| Selection sort              | \\(O(n^2)\\)     | \\(O(n^2)\\)     | \\(O(n^2)\\)     | \\(O(1)\\)                 |
| Insertion sort              | \\(O(n)\\)       | \\(O(n^2)\\)     | \\(O(n^2)\\)     | \\(O(1)\\)                 |
| Merge sort                  | \\(O(n\log n)\\) | \\(O(n\log n)\\) | \\(O(n\log n)\\) | \\(O(n)\\)                 |
| Quick sort                  | \\(O(n\log n)\\) | \\(O(n\log n)\\) | \\(O(n^2)\\)     | Depends on recursion depth |


### 3.9.10 Essential formulas from Units 1, 2 and 3


### Number and array formulas

\\[ \text{Average}=\frac{\text{Sum of elements}}{\text{Number of elements}} \\]

\\[ \text{Array address}=B+i\times w \\]

### Two-dimensional array address

\\[ \operatorname{Address}(A[i][j]) = B+(iC+j)w \\]

### Matrix addition

\\[ C\_{ij}=A\_{ij}+B\_{ij} \\]

### Matrix multiplication

\\[ C\_{ij}=\sum\_{k=0}^{n-1}A\_{ik}B\_{kj} \\]

For matrices \\(A\\) of size \\(m\times n\\) and \\(B\\) of size \\(n\times p\\), the product \\(C\\) has size \\(m\times p\\).

### Matrix transpose

\\[ A^T\_{ij}=A\_{ji} \\]

### Factorial

\\[ n!=n(n-1)(n-2)\cdots 1 \\]

\\[ 0!=1 \\]

### Fibonacci sequence

\\[ F_0=0,\qquad F_1=1 \\]

\\[ F_n=F\_{n-1}+F\_{n-2} \\]

### Euclidean GCD

\\[ \gcd(a,b)=\gcd(b,a\bmod b) \\]

### Tower of Hanoi

\\[ T(n)=2T(n-1)+1 \\]

\\[ T(n)=2^n-1 \\]

### Pointer-based array access

\\[ arr[i]=\*(arr+i) \\]

### Dynamic allocation

\\[ \text{Required bytes}=n\times\operatorname{sizeof}(T) \\]

# FINAL EXAM PREPARATION CHECKLIST

Use this checklist to verify that you can handle the core syllabus concepts without relying only on memorized code.


# UNIT 1: PROBLEM SOLVING AND C FUNDAMENTALS


- Define a problem, algorithm and flowchart.
- Explain the characteristics of a good algorithm.
- Identify flowchart symbols.
- Explain the basic structure of a C program.
- Identify tokens, keywords, identifiers and constants.
- Declare variables and explain fundamental data types.
- Use input and output functions correctly.
- Explain arithmetic, relational, logical and assignment operators.
- Apply operator precedence and associativity.
- Write programs using `if`, `if-else`, nested `if` and `switch`.


## Unit 2: Loops, Arrays, Strings, Functions and Recursion


- Differentiate `for`, `while` and `do-while`.
- Write programs using nested loops.
- Perform array traversal and element manipulation.
- Implement linear search and binary search.
- Implement bubble, selection and insertion sort.
- Explain two-dimensional array memory layout.
- Perform matrix addition, multiplication and transpose.
- Explain string termination and string input.
- Use standard string library functions.
- Implement manual string operations.
- Explain function declaration, definition and calling.
- Differentiate actual and formal arguments.
- Explain call by value and pointer-based modification.
- Explain local and global scope.
- Write recursive factorial, Fibonacci and GCD programs.
- Explain the Tower of Hanoi recurrence.



# UNIT 3: POINTERS, STORAGE CLASSES, STRUCTURES, UNIONS & DYNAMIC MEMORY ALLOCATION



- Declare and initialize pointers.
- Explain `&` and `*`.
- Perform pointer arithmetic.
- Explain the relationship between pointers and arrays.
- Explain pointer to pointer and void pointer.
- Differentiate null, wild and dangling pointers.
- Explain `auto`, `register`, `static` and `extern`.
- Differentiate scope, lifetime and linkage.
- Declare structures and access their members.
- Use arrays of structures and nested structures.
- Explain structure padding and alignment.
- Access structures through pointers.
- Differentiate structures and unions.
- Explain bit-fields, typedef and enum.
- Use `malloc()`, `calloc()`, `realloc()` and `free()`.
- Identify memory leaks and invalid memory accesses.

# HIGH-PRIORITY EXAM QUESTIONS

The following are useful questions to practise before the examination.

## Theory and output-prediction questions

1. What is a pointer? Explain pointer declaration and initialization with an example.
2. Differentiate between `&` and `*`.
3. Explain pointer arithmetic with a memory diagram.
4. What is a pointer to pointer? Explain with an example.
5. Differentiate between null, wild and dangling pointers.
6. Explain the relationship between arrays and pointers.
7. Explain the four traditional storage classes.
8. Differentiate between automatic and static local variables.
9. Define a structure. Explain its declaration and member access.
10. Explain structure padding and memory alignment.
11. Differentiate between structures and unions.
12. Explain bit-fields with a suitable example.
13. What is `typedef`? Explain with a structure.
14. What is an enumeration? Explain default and explicitly assigned values.
15. Explain dynamic memory allocation.
16. Differentiate between `malloc()` and `calloc()`.
17. Explain the purpose of `realloc()` and `free()`.
18. What is a memory leak?
19. What is the difference between scope and lifetime?
20. Explain the use of a pointer to a structure.

## Programming questions to practise

1. Swap two numbers using pointers.
2. Find the sum of array elements using pointers.
3. Reverse an array using pointers.
4. Find the largest and smallest elements using pointers.
5. Demonstrate a static variable inside a function.
6. Store and display student records using structures.
7. Calculate total and average marks using a structure.
8. Demonstrate a pointer to a structure.
9. Demonstrate union memory sharing.
10. Use `typedef` and `enum` in a program.
11. Allocate and display an array using `malloc()`.
12. Initialize an array using `calloc()`.
13. Resize an array using `realloc()`.
14. Add two matrices using dynamic memory allocation.
15. Store a dynamically allocated string inside a structure.

# FINAL EXAMINER'S NOTES

1. **Do not confuse the address with the value.** `p` stores an address, while `*p` accesses the object at that address.
2. **C uses pass-by-value.** Passing a pointer copies the pointer value, but allows the function to modify the pointed-to object.
3. **Array indexing begins at zero.** For an array of size \\(n\\), the final valid index is \\(n-1\\).
4. **Strings require a null terminator.** Always reserve space for `'\0'`.
5. **A static local variable retains its value.** It is initialized once and persists for the program's execution.
6. **Structure members can have different types.** Padding may affect the total size.
7. **Union members share memory.** Do not assume their values are stored independently.
8. **Always check dynamic allocation.** `malloc()`, `calloc()` and `realloc()` can fail.
9. **Release allocated memory.** Use `free()` when the allocation is no longer required.
10. **Use correct format specifiers.** A wrong `printf()` or `scanf()` format can cause incorrect behaviour or undefined behaviour.
11. **Do not ignore compiler warnings.** Warnings often reveal errors before the program is run.
12. **Dry-run every loop.** Trace initialization, condition, body and update carefully.


**The three-part C programming compendium is now complete in this conversation.**

The material covered:

- **Part 1:** Problem solving, algorithms, flowcharts and C fundamentals.
- **Part 2:** Looping, arrays, searching, sorting, matrices, strings, functions and recursion.
- **Part 3:** Pointers, storage classes, structures, unions, bit-fields, typedef, enum, dynamic memory allocation, 15 solved programs, debugging traps and quick revision.

**Final revision advice:** Prioritize writing programs without looking at the solutions, tracing pointer and array expressions manually, and explaining memory diagrams in your own words. Those three skills are especially valuable for C programming practicals, output-prediction questions and viva examinations.
