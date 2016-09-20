# Introduction to Programming with C++ 的笔记

标签（空格分隔）： Intro

---
## 1.5 History of C++
*Page 33*
> C is portable and hardware independent, thus widely used for developing oerating systems.

## 1.6 A Simple C++ Program
*Page 34*
> Normally programs from different sources will be used in a project. The scope of identifiers may overlap with each other, which results in naming conflicts. By using **namespaces** this problem can be avoided. 

## 1.8 Programming Style and Documentation
*Page 40*
```c++
// Next-line style for C++
int main( )
{
  cout << "Hello World!" << endl;
  return 0;
}
// End-of-line style for Java
int main( ) {
  cout << "Hello World!" << endl;
  return 0;
}
```

## 2.2 Writing a Simple Program
*Page 52*
> Variables correspond to memory locations. Every variable has a name, type, size, and value.

## 2.3 Reading Input from the Keyboard
*Page 53*
> C++ automatically converts the input data from keyboard to the type of the variable.

## 2.5 Variables
*Page 56*
> The variable declaration tells the compiler to allocate appropriate memory space for the variable based on its data type.

## 2.6 Assignment Statements and Assignment Expressions
*Page 58*
```c++
cout << (x = 1);
// is equivalent to
x = 1;
cout << x;

i = j = k = 1;
// is equivalent to
k = 1;
j = k;
i = j;
// which means that assignment operator is right-associative.
```

## 2.8 Numeric Data Types and Operations
*Page 63*
> * To perform regular mathematical division, one of the operands must be a floating-point number.
> * In C++ % operator works only with integer operands.
> * The behavior of the % operator involving negative integers is compiler-dependent.

*Page 71*
> * For most binary operators, C++ does not specify the operand evaluation order. (Normally assume that left evaluated before right.)

*Page 73*
> * Casting does not change the variable being cast.
```C++
#include <iomanip>
#include <iostream>
using namespace std;
int main()
{
	double x = 12345.6789;
	// to get value with 2 digits after the decimal point
	cout << setprecision(7) << (static_cast<int>(x * 100) / 100.0) << endl;
	return 0;
}
```

## 3.2 The bool Data Type
*Page 93*
> * Internally and display 1 for true and 0 for false
> * Any nonzero value (e.g. -1.5) evaluates to true and zero value evaluates to false

## 3.5 Nested if and Multi-Way if-else Statements
> A condition is tested only when all the condition that comes before it are false

