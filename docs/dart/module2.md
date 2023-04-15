# Module 2: Basic Data Types and Variables

In this module, we will explore the basic data types in Dart and how to declare and use variables.

<br/>

## Numeric Data Types

Dart supports two main types of numeric data types: integers and floating-point numbers.

## Integers
Integers represent whole numbers without any decimal point. In Dart, integers can be either signed (positive or negative) or unsigned (positive only). Dart provides several types of integers, including:

- int: A signed 64-bit integer. The range of values is -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807.
- int8: A signed 8-bit integer. The range of values is -128 to 127.
- int16: A signed 16-bit integer. The range of values is -32,768 to 32,767.
- int32: A signed 32-bit integer. The range of values is -2,147,483,648 to 2,147,483,647.
- int64: A signed 64-bit integer. The range of values is -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807.
- uint8: An unsigned 8-bit integer. The range of values is 0 to 255.
- uint16: An unsigned 16-bit integer. The range of values is 0 to 65,535.
- uint32: An unsigned 32-bit integer. The range of values is 0 to 4,294,967,295.
- uint64: An unsigned 64-bit integer. The range of values is 0 to 18,446,744,073,709,551,615.

Here's an example of how to declare and initialize an integer variable in Dart:

```C
int age = 30;
```

<br/>

## Floating-Point Numbers

Floating-point numbers represent decimal values. In Dart, there are two types of floating-point numbers: float and double. Float is a 32-bit floating-point number, and double is a 64-bit floating-point number. Here's an example of how to declare and initialize a double variable in Dart:

```C
double salary = 50000.0;
```

<br/>

## String Data Type

Strings represent a sequence of characters. In Dart, strings are enclosed in single or double quotes. Here's an example of how to declare and initialize a string variable in Dart:

```C
String name = 'John Doe';
```

<br/>

## Boolean Data Type

Boolean represents a logical value, either true or false. Here's an example of how to declare and initialize a boolean variable in Dart:

```C
bool isEmployed = true;
```

<br/>

## Variables and Constants

In Dart, you can declare variables and constants using the var, final, and const keywords. The var keyword is used to declare a variable with an inferred type, which means that the type is determined based on the assigned value. The final keyword is used to declare a variable that can only be assigned once, and its value is determined at runtime. The const keyword is used to declare a variable that is a compile-time constant, and its value is determined at compile time.

Here's an example of how to declare and initialize a variable and a constant in Dart:

```C
var age = 30;
final salary = 50000.0;
const pi = 3.14;
```

<br/>

## Operators

Dart provides a variety of operators for performing arithmetic, comparison, and logical operations. Some common operators include:

- Arithmetic Operators: +, -, *, /, %
- Comparison Operators: ==, !=, <, >, <=
- Logical Operators: &&, ||, !

Here's an example of how to use operators in Dart:

```C
int a = 10;
int b = 5;

// Arithmetic Operators
print(a + b); // 15
print(a - b); // 5
print(a * b); // 50
print(a / b); // 2.0
print(a % b); // 0

// Comparison Operators
print(a == b); // false
print(a != b); // true
print(a > b); // true
print(a < b); // false
print(a >= b); // true
print(a <= b); // false

// Logical Operators
print(a > b && a < 20); // true
print(a < b || b < 0); // false
print(!(a > b)); // false
```

In the next module, we will explore control structures in Dart.