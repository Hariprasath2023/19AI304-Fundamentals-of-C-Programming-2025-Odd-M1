# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```asm
#include <stdio.h>

int main() {
    int intLiteral = 10;
    float floatLiteral = 3.14;
    char charLiteral = 'A';
    char stringLiteral[] = "Hello C";

    printf("Integer literal: %d, Size: %lu bytes\n", intLiteral, sizeof(intLiteral));
    printf("Float literal: %f, Size: %lu bytes\n", floatLiteral, sizeof(floatLiteral));
    printf("Character literal: %c, Size: %lu bytes\n", charLiteral, sizeof(charLiteral));
    printf("String literal: %s, Size: %lu bytes\n", stringLiteral, sizeof(stringLiteral));

    return 0;
}
```
# Output:
<img width="627" height="217" alt="image" src="https://github.com/user-attachments/assets/29fd4467-c38f-4976-a82d-2f9b7f6730c4" />


# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```asm
#include <stdio.h>

#define PI 3.14159

int main() {
    // Declare a constant variable
    const int DAYS = 7;

    // Display the values
    printf("Value of Macro Constant PI: %.5f\n", PI);
    printf("Value of Constant Variable DAYS: %d\n", DAYS);

    return 0;
}
```
# Output:
Value of Macro Constant PI: 3.14159
Value of Constant Variable DAYS: 7
# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```asm
#include <stdio.h>

int main() {
    // Declaration and Initialization
    int integerVar = 42;
    float floatVar = 3.14f;
    double doubleVar = 12345.6789;
    char charVar = 'Z';

    // Displaying values
    printf("Integer value: %d\n", integerVar);
    printf("Float value: %f\n", floatVar);
    printf("Double value: %lf\n", doubleVar);
    printf("Character value: %c\n", charVar);

    return 0;
}
```
# Output:
Integer value: 42
Float value: 3.140000
Double value: 12345.678900
Character value: Z


# Result: 

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```asm
#include <stdio.h>

int main() {
    int a, b;

    // Input
    printf("Enter value for a: ");
    scanf("%d", &a);
    printf("Enter value for b: ");
    scanf("%d", &b);

    printf("\n--- Arithmetic Operations ---\n");
    printf("Addition (a + b): %d\n", a + b);
    printf("Subtraction (a - b): %d\n", a - b);
    printf("Multiplication (a * b): %d\n", a * b);
    if(b != 0) {
        printf("Division (a / b): %d\n", a / b);
        printf("Remainder (a %% b): %d\n", a % b);
    } else {
        printf("Division and Remainder by zero is not possible.\n");
    }

    printf("\n--- Bitwise Operations ---\n");
    printf("Bitwise AND (a & b): %d\n", a & b);
    printf("Bitwise OR (a | b): %d\n", a | b);
    printf("Bitwise XOR (a ^ b): %d\n", a ^ b);
    printf("Left Shift (a << b): %d\n", a << b);
    printf("Right Shift (a >> b): %d\n", a >> b);
    printf("Bitwise NOT (~a): %d\n", ~a);
    printf("Bitwise NOT (~b): %d\n", ~b);

    return 0;
}
```
# Output:
Enter value for a: 10
Enter value for b: 2

--- Arithmetic Operations ---
Addition (a + b): 12
Subtraction (a - b): 8
Multiplication (a * b): 20
Division (a / b): 5
Remainder (a % b): 0

--- Bitwise Operations ---
Bitwise AND (a & b): 2
Bitwise OR (a | b): 10
Bitwise XOR (a ^ b): 8
Left Shift (a << b): 40
Right Shift (a >> b): 2
Bitwise NOT (~a): -11
Bitwise NOT (~b): -3

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```asm
#include <stdio.h>

int main() {
    char ch;

    // Input
    printf("Enter any character: ");
    scanf("%c", &ch);

    // Using Ternary Operator to classify the character
    (ch >= '0' && ch <= '9') ? printf("'%c' is a Digit.\n", ch) : 
        ((ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z')) ? 
            ((ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' || 
              ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') ? 
              printf("'%c' is a Vowel.\n", ch) : printf("'%c' is a Consonant.\n", ch)) 
        : printf("'%c' is a Special Symbol.\n", ch);

    return 0;
}
```
# Output:
Enter any character: E
'E' is a Vowel.
Enter any character: 7
'7' is a Digit.
# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


