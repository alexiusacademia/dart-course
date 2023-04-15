# Module 9: Files and Streams

In this module, we will explore how to work with files and streams in Dart, which is used to read and write data from and to files and other sources.

<br/>

## Working with Files

In Dart, you can read and write data to and from files using the "dart:io" library. Here's an example of how to read data from a file in Dart:

```C
import 'dart:io';

void main() {
  File file = new File('data.txt');
  Future<String> future = file.readAsString();
  future.then((value) {
    print(value);
  }).catchError((error) {
    print(error);
  });
}
```

You can also write data to a file:

```C
import 'dart:io';

void main() {
  File file = new File('data.txt');
  file.writeAsString('Hello, World').then((value) {
    print('Data written successfully');
  }).catchError((error) {
    print(error);
  });
}
```

<br/>

## Working with Streams

In Dart, streams are used to read and write data asynchronously. Here's an example of how to create and use a stream in Dart:

```C
import 'dart:async';

void main() {
  StreamController<String> controller = new StreamController<String>();
  Stream<String> stream = controller.stream;
  stream.listen((value) {
    print(value);
  });

  controller.add('Hello');
  controller.add('World');
  controller.close();
}
```

In this example, we create a stream controller and a stream. We then add two values to the stream and close the controller.

You can also use the async/await syntax with streams:

```C
import 'dart:async';

void main() async {
  StreamController<String> controller = new StreamController<String>();
  Stream<String> stream = controller.stream;
  await for (String value in stream) {
    print(value);
  }

  controller.add('Hello');
  controller.add('World');
  controller.close();
}
```

In this example, we use the "await for" syntax to listen to the stream asynchronously.

In the final module, we will explore how to use packages and dependencies in Dart.