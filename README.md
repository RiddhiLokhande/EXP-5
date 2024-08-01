# EXP-5
## Aim

- To implement and study C++ Dcision making statements.

## Software required-

You need to have a C++ compiler installed on your system. Common options include:


- [Microsoft Visual C++](https://visualstudio.microsoft.com/vs/features/cplusplus/)

## Theory
To study and implement decision-making statements in C++, it's important to understand their syntax, usage, and behavior.
##### Overview of Decision-Making Statements
if Statement
if-else Statement
if-else if-else Statement
switch Statement
Ternary (Conditional) Operator
Detailed Explanation and Examples
1. if Statement:
The if statement evaluates a condition and executes a block of code if the condition is true.
2. if-else Statement:
The if-else statement provides an alternative block of code to execute if the condition is false.
3. switch Statement:
The switch statement allows you to select one of many code blocks to execute.
4. Nested if-else Statements:
 Practice creating nested conditions.
 5. Nested if statements:
 nested if statement is simply an if statement inside another if statement. This allows for more complex decision-making logic.

![image](https://github.com/user-attachments/assets/edd01ed0-ed7e-4d9b-9750-c7908653f404)

## CODE 1 IF STATEMENT
```cpp

//RIDDHI LOKHANDE
//ENTC B2
//23070123107
//EXP 5 A
#include <iostream>

int main() {
    int number;

    std::cout << "Enter an integer: ";
    std::cin >> number;
   if (number > 0) {
        std::cout << "The number is positive." << std::endl;
    }

    return 0;
}
```

### Output
![image](https://github.com/user-attachments/assets/02e7ee49-4f9c-409a-8338-4c8069d540e6)

## CODE 2 IF-ELSE STATEMENT
```cpp

//RIDDHI LOKHANDE 
//ENTC B2
//23070123107
//EXP 5 CODE 1
#include <iostream>
using namespace std;
int main() {
    double n1, n2, n3;
    cout << "Enter three numbers: ";
    cin >> n1 >> n2 >> n3;
    if(n1 >= n2 && n1 >= n3)
        cout << "Largest number: " << n1;
    else if(n2 >= n1 && n2 >= n3)
        cout << "Largest number: " << n2;
    else 
        cout << "Largest number: " << n3;
    return 0;
}
```
### Output
![image](https://github.com/user-attachments/assets/ec759201-81b2-4e28-b160-b0b84e23907b)

## CODE 3 NESTED IF-ELSE STATEMENT
```cpp

/RIDDHI LOKHANDE 
//ENTC B2
//23070123107
//EXP 5 CODE 2
#include <iostream>
using namespace std;
int main() {
    double n1, n2, n3;
    cout << "Enter three numbers: ";
    cin >> n1 >> n2 >> n3;
    if (n1 >= n2) {
        if (n1 >= n3)
            cout << "Largest number: " << n1;
        else
            cout << "Largest number: " << n3;
    }
    else {
        if (n2 >= n3)
            cout << "Largest number: " << n2;
        else
            cout << "Largest number: " << n3;
    }
    return 0;
}
```
### Output
![image](https://github.com/user-attachments/assets/a353c05e-56db-4b44-aef0-0f693108c99a)
## CODE 4 SWITCH AND BREAK STATEMENT
```cpp

//RIDDHI LOKHANDE 
//ENTC B2
//23070123107
//EXP 5 CODE 3
#include<iostream>
using namespace std;

int main() {
    int choice;
    cout << "1. Monday" << endl
         << "2. Tuesday" << endl
         << "3. Wednesday" << endl
         << "4. Thursday" << endl
         << "5. Friday" << endl
         << "6. Saturday" << endl
         << "7. Sunday" << endl;
    cout << "Enter your choice: ";
    cin >> choice;
    
    switch(choice) {
        case 1:
            cout << "Monday" << endl;
            break;
        case 2:
            cout << "Tuesday" << endl;
            break;
        case 3:
            cout << "Wednesday" << endl;
            break;
        case 4:
            cout << "Thursday" << endl;
            break;
        case 5:
            cout << "Friday" << endl;
            break;
        case 6:
            cout << "Saturday" << endl;
            break;
        case 7:
            cout << "Sunday" << endl;
            break;
        default:
            cout << "Wrong Input" << endl;
            break;
    }
    
    return 0;
}
```
### OUTPUT
![image](https://github.com/user-attachments/assets/4177eeda-38d5-4e13-a69c-15e938a7b0f2)
## CODE 5 WRITING CALCULATOR CODE USING DECISION MAKING STATEMENTS
```cpp
//RIDDHI LOKHANDE 
//ENTC B2
//23070123107
//EXP 5 CODE 4
#include<iostream>
using namespace std;

int main() {
    char oper;
    float num1, num2;

    cout << "Enter an operator (+, -, *, /): ";
    cin >> oper;
    cout << "Enter two numbers: " << endl;
    cin >> num1 >> num2;

    switch (oper) {
        case '+':
            cout << num1 << " + " << num2 << " = " << num1 + num2 << endl;
            break;
        case '-':
            cout << num1 << " - " << num2 << " = " << num1 - num2 << endl;
            break;
        case '*':
            cout << num1 << " * " << num2 << " = " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 != 0)
                cout << num1 << " / " << num2 << " = " << num1 / num2 << endl;
            else
                cout << "Error! Division by zero." << endl;
            break;
        default:
            cout << "Error! The operator is not correct" << endl;
            break;
    }

    return 0;
}
```
### OUTPUT
![image](https://github.com/user-attachments/assets/6ac2205e-0873-4ff8-8573-00e6f37061cb)





## Conclusion
We learnt the implementation and study of decision making statements C++ language.
