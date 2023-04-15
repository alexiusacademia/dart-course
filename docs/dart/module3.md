# Module 3: Control Structures

In this module, we will explore control structures in Dart, which are used to control the flow of execution in a program.

<br/>

## Conditional Statements

Conditional statements are used to execute a block of code based on a condition. In Dart, there are two types of conditional statements: if statements and switch statements.

<br/>

## If Statements

An if statement executes a block of code if a condition is true. Here's an example of an if statement in Dart:

```C
int age = 30;

if (age > 18) {
  print('You are an adult');
} else {
  print('You are a minor');
}
```

<br/>

## Switch Statements

A switch statement executes a block of code based on the value of a variable. Here's an example of a switch statement in Dart:

```C
String grade = 'A';

switch (grade) {
  case 'A':
    print('Excellent');
    break;
  case 'B':
    print('Good');
    break;
  case 'C':
    print('Average');
    break;
  case 'D':
    print('Below Average');
    break;
  default:
    print('Fail');
}
```

<br/>

## Looping Statements

Looping statements are used to execute a block of code repeatedly. In Dart, there are three types of looping statements: for loops, while loops, and do-while loops.

<br/>

## For Loops

A for loop is used to execute a block of code a fixed number of times. Here's an example of a for loop in Dart:

```C
Copy code
for (int i = 0; i < 10; i++) {
  print(i);
}
```

<br/>

## While Loops

A while loop is used to execute a block of code while a condition is true. Here's an example of a while loop in Dart:

```C
int i = 0;

while (i < 10) {
  print(i);
  i++;
}
```

<br/>

## Do-While Loops

A do-while loop is similar to a while loop, but the block of code is executed at least once, even if the condition is false. Here's an example of a do-while loop in Dart:

```C
int i = 0;

do {
  print(i);
  i++;
} while (i < 10);
```

<br/>

## Break and Continue Statements

The break and continue statements are used to control the flow of execution in a loop. The break statement is used to terminate the loop, while the continue statement is used to skip the current iteration and move to the next iteration. Here's an example of using break and continue statements in a for loop in Dart:

```C
for (int i = 0; i < 10; i++) {
  if (i == 5) {
    break;
  }
  if (i == 3) {
    continue;
  }
  print(i);
}
```

In the next module, we will explore functions in Dart.