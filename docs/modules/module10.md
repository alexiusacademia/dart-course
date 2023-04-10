# Module 10: Packages and Dependencies

In this module, we will explore how to use packages and dependencies in Dart, which is used to add functionality and reuse code from other libraries.

<br/>

## Packages

A package is a collection of libraries and assets that can be reused in other projects. In Dart, you can create your own packages or use existing packages from the Dart package repository.

To use a package, you need to add it to your project's "pubspec.yaml" file:

```yaml
dependencies:
  http: ^0.13.4
```

In this example, we are adding the "http" package to our project. We are using the "^" symbol to indicate that we want to use the latest version of the package that is compatible with our current version.

You can then run the "pub get" command to install the package:

```bash
$ pub get
```

You can then import the package and use its functionality in your code:

```C
import 'package:http/http.dart' as http;

void main() async {
  var response = await http.get(Uri.parse('https://jsonplaceholder.typicode.com/posts/1'));
  print(response.body);
}
```

In this example, we are using the "http" package to make an HTTP request and print the response.

<br/>

## Dependencies

A dependency is a package that is required by another package. In Dart, you can specify dependencies in the "pubspec.yaml" file using the "dependencies" and "dev_dependencies" keys.

Here's an example of how to declare a dependency in the "pubspec.yaml" file:

```yaml
dependencies:
  http: ^0.13.4

dev_dependencies:
  test: ^1.16.8
```

In this example, we are adding the "test" package as a dev dependency. Dev dependencies are only used during development and are not included in the production code.

You can then run the "pub get" command to install the dependencies:

```bash
$ pub get
```

You can then use the dependencies in your code and tests:

```C
import 'package:test/test.dart';

void main() {
  test('adds 1 + 2 to equal 3', () {
    expect(1 + 2, equals(3));
  });
}
```

In this example, we are using the "test" package to write and run tests for our code.

That's it for this course! With the knowledge gained from these modules, you should be well-equipped to start developing applications using Dart. Happy coding!