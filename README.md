# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 9.2.26
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
```
#include <stdio.h>

int main() {
    printf("Integer literal: %d\n", 100);
    printf("Float literal: %.2f\n", 3.14);
    printf("Character literal: %c\n", 'A');
    printf("String literal: %s\n", "Hello, C");
    return 0;
}
```
# Output:
<img width="383" height="304" alt="Screenshot (444)" src="https://github.com/user-attachments/assets/26bed5c4-d55d-4b84-b5c8-2d9380fa67ca" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 9.2.26
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
```
#include <stdio.h>

// Macro constant
#define PI 3.14159

int main() {
    // Constant variable
    const int MAX = 100;

    printf("Value of macro constant PI = %.5f\n", PI);
    printf("Value of constant variable MAX = %d\n", MAX);

    // Uncommenting the next line will cause an error
    // MAX = 200; // Cannot modify a constant variable

    return 0;
}
```

# Output:
<img width="1920" height="1080" alt="Screenshot (445)" src="https://github.com/user-attachments/assets/8d53a7af-8c72-48b2-a578-6e90bce87b2b" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 9.2.26
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
```
#include <stdio.h>

int main() {
    // Different data types
    int a = 10;
    float b = 5.75;
    double c = 19.123456;
    char d = 'G';

    // Display values using printf
    printf("Integer value (int) a = %d\n", a);
    printf("Floating-point value (float) b = %.2f\n", b);
    printf("Double value (double) c = %.6lf\n", c);
    printf("Character value (char) d = %c\n", d);

    return 0;
}
```
# Output:
<img width="1920" height="1080" alt="Screenshot (446)" src="https://github.com/user-attachments/assets/538bc247-bcb4-4c2a-9841-d5eb0a44eef5" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 9.2.26
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
```
#include <stdio.h>

int main() {
    int a, b;

    // Input two integers
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    // Arithmetic operations
    printf("\nArithmetic Operations:\n");
    printf("Addition: %d + %d = %d\n", a, b, a + b);
    printf("Subtraction: %d - %d = %d\n", a, b, a - b);
    printf("Multiplication: %d * %d = %d\n", a, b, a * b);
    if(b != 0) {
        printf("Division: %d / %d = %d\n", a, b, a / b);
        printf("Remainder: %d %% %d = %d\n", a, b, a % b);
    } else {
        printf("Division and remainder by zero is not allowed.\n");
    }

    // Bitwise operations
    printf("\nBitwise Operations:\n");
    printf("%d & %d = %d\n", a, b, a & b);  // AND
    printf("%d | %d = %d\n", a, b, a | b);  // OR
    printf("%d ^ %d = %d\n", a, b, a ^ b);  // XOR
    printf("%d << 1 = %d\n", a, a << 1);    // Left shift a by 1
    printf("%d >> 1 = %d\n", a, a >> 1);    // Right shift a by 1
    printf("~%d = %d\n", a, ~a);            // NOT a
    printf("~%d = %d\n", b, ~b);            // NOT b

    return 0;
}
```
# Output:
<img width="1920" height="1080" alt="Screenshot (447)" src="https://github.com/user-attachments/assets/536aebc9-8c3e-4d91-aae5-3b6f07e054c5" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 9.2.26
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
```
#include <stdio.h>

int main() {
    char ch;

    // Input character
    printf("Enter a character: ");
    scanf("%c", &ch);

    // Check and display using ternary operators
    ( (ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z') ) ?
        ( (ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'||ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u') ?
            printf("%c is a vowel.\n", ch) :
            printf("%c is a consonant.\n", ch) ) :
        ( (ch >= '0' && ch <= '9') ?
            printf("%c is a digit.\n", ch) :
            printf("%c is a special symbol.\n", ch) );

    return 0;
}
```
# Output:
<img width="1920" height="1080" alt="Screenshot (448)" src="https://github.com/user-attachments/assets/0b060a0d-3ead-4c78-a368-55bb16da547d" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


