# Module 4: Functions

In this module, we will explore functions in Dart, which are used to encapsulate a block of code and reuse it throughout a program.

<br/>

## Function Declaration and Invocation

A function is declared using the "function" keyword, followed by the function name, parameters (if any), and the function body enclosed in curly braces. Here's an example of a function that takes two parameters and returns their sum:

```C
int add(int a, int b) {
  return a + b;
}
```

The function can then be invoked by calling its name and passing the required arguments:

```C
int result = add(2, 3);
print(result); // 5
```

<br/>

## Function Parameters

Functions can take zero or more parameters, which are used to pass values to the function. In Dart, there are two types of parameters: positional parameters and named parameters.

<br/>

## Positional Parameters

Positional parameters are the most common type of parameters in Dart. They are passed to the function in the order they are declared. Here's an example of a function that takes two positional parameters:

```C
void greet(String name, String message) {
  print('$name says $message');
}

greet('John', 'Hello'); // John says Hello
```

<br/>

## Named Parameters

Named parameters are used to pass values to a function by name, rather than by position. They are enclosed in curly braces {} and are declared using the "required" or "optional" keyword. Here's an example of a function that takes two named parameters:

```C
void greet({required String name, String message = 'Hello'}) {
  print('$name says $message');
}

greet(name: 'John'); // John says Hello
greet(name: 'John', message: 'Hi'); // John says Hi
```

Functions can also have optional positional parameters by enclosing them in square brackets [].

<br/>

## Function Return Values

Functions can also return values using the "return" keyword. The return type is declared before the function name. Here's an example of a function that returns the sum of two integers:

```C
int add(int a, int b) {
  return a + b;
}

int result = add(2, 3);
print(result); // 5
```

In the next module, we will explore collections in Dart.