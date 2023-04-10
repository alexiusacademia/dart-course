# Module 8: Asynchronous Programming

In this module, we will explore asynchronous programming in Dart, which is used to handle long-running tasks and prevent blocking the main thread.

<br/>

## Asynchronous Programming

Asynchronous programming is a programming paradigm that allows a program to execute multiple tasks concurrently. In Dart, asynchronous programming is achieved using futures and async/await.

<br/>

## Futures

A future is an object that represents the result of a long-running task. In Dart, futures are used to handle asynchronous tasks. Here's an example of how to create a future in Dart:

```C
Future<String> fetchData() {
  return Future.delayed(Duration(seconds: 1), () {
    return 'Data fetched successfully';
  });
}
```

You can then use the future to handle the result of the task:

```C
fetchData().then((value) {
  print(value);
}).catchError((error) {
  print(error);
});
```

<br/>

## Async/Await

Async/await is a syntactic sugar for working with futures in Dart. It allows you to write asynchronous code that looks synchronous. Here's an example of how to use async/await in Dart:

```C
Future<String> fetchData() async {
  await Future.delayed(Duration(seconds: 1));
  return 'Data fetched successfully';
}

void main() async {
  String data = await fetchData();
  print(data);
}
```

You can also handle errors using the try-catch block:

```C
Future<String> fetchData() async {
  await Future.delayed(Duration(seconds: 1));
  throw new Exception('Failed to fetch data');
}

void main() async {
  try {
    String data = await fetchData();
    print(data);
  } catch (e) {
    print(e);
  }
}
```

In the next module, we will explore how to work with files and streams in Dart.