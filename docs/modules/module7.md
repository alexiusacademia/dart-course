# Module 7: Exception Handling

In this module, we will explore exception handling in Dart, which is used to handle errors and unexpected situations in a program.

<br/>

## Exceptions

An exception is an error that occurs during the execution of a program. In Dart, exceptions are represented by objects that contain information about the error. Here's an example of how to throw an exception in Dart:

```C
void divide(int a, int b) {
  if (b == 0) {
    throw new Exception('Cannot divide by zero');
  }
  print(a / b);
}
```

You can catch an exception using a try-catch block:

```C
try {
  divide(10, 0);
} catch (e) {
  print(e);
}
```

You can also catch specific types of exceptions using the "on" keyword:

```C
try {
  divide(10, 0);
} on Exception catch (e) {
  print(e);
}
```

<br/>

## Finally Blocks

A finally block is used to execute code after a try-catch block, regardless of whether an exception was thrown or not. Here's an example of how to use a finally block in Dart:

```C
try {
  divide(10, 0);
} catch (e) {
  print(e);
} finally {
  print('Done');
}
```

<br/>

## Custom Exceptions

You can also create custom exceptions in Dart by extending the "Exception" class or one of its subclasses. Here's an example of how to create a custom exception in Dart:

```C
class MyException implements Exception {
  String message;

  MyException(this.message);

  @override
  String toString() {
    return message;
  }
}

void throwError() {
  throw new MyException('This is my custom exception');
}

try {
  throwError();
} catch (e) {
  print(e);
}
```

In the next module, we will explore asynchronous programming in Dart.