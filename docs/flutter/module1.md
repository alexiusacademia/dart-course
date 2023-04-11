# Lesson 1: Getting Started with Flutter

In this lesson, we will introduce you to Flutter and help you set up your development environment. By the end of this lesson, you will have a basic understanding of Flutter and be ready to start building your first app.

## What is Flutter?

Flutter is an open-source mobile application development framework created by Google. It allows developers to build high-quality, native apps for both Android and iOS using a single codebase. Flutter uses Dart as its programming language and comes with a rich set of pre-built widgets and tools to help you create beautiful and responsive user interfaces.

## Flutter Architecture

Flutter uses a reactive programming model, where the UI is built as a function of the application state. The application state is stored in widgets, which are the building blocks of a Flutter UI. Widgets can be either stateless or stateful. Stateless widgets are immutable and do not have any internal state, while stateful widgets have mutable state that can change over time.

## Flutter Widgets

Widgets are the basic building blocks of a Flutter UI. Widgets can be either stateful or stateless and can be arranged in a hierarchical tree structure. Each widget can have a parent and one or more children, which are also widgets. The parent widget determines the layout and positioning of its children widgets.

## Flutter Layout System

Flutter uses a flexible and powerful layout system that allows developers to create responsive and adaptive UIs. The layout system is based on the concept of constraints, which are the minimum and maximum dimensions that a widget can have. The layout system determines the size and position of a widget based on its constraints and the constraints of its parent widget.

## Setting up your Development Environment

To start developing with Flutter, you will need to set up your development environment. Here are the steps to get started:

### Install Flutter

Download and install the Flutter SDK from the official website (https://flutter.dev/docs/get-started/install). Follow the instructions for your operating system.

### Install Android Studio or Visual Studio Code

Flutter supports both Android Studio and Visual Studio Code as IDEs. Choose one of the two and install it on your machine.

### Install the Flutter and Dart plugins

Once you have installed your IDE, install the Flutter and Dart plugins. These plugins provide support for developing Flutter applications in your IDE.

### Verify your installation

Open a new terminal window and run the following command:

```
flutter doctor
```

This command will verify that your Flutter installation is set up correctly and will check for any dependencies that you may need to install.

## Creating your First Flutter App

Now that you have set up your development environment, it's time to create your first Flutter app. Here are the steps to create a new Flutter app:

Open your IDE and create a new Flutter project. You can do this by selecting "New Flutter Project" from the IDE menu.

Give your project a name and select a location to save it.

Choose a Flutter template for your app. You can choose from several templates, including a basic app, a material design app, or a Cupertino-style app.

Wait for your project to be created. This may take a few minutes.

Once your project is created, open the main.dart file. This is where you will write your first Flutter code.

Replace the default code in main.dart with the following code:

```
import 'package:flutter/material.dart';

void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('My First Flutter App'),
        ),
        body: Center(
          child: Text('Hello, World!'),
        ),
      ),
    ),
  );
}
```

Save your changes and run your app by clicking the "Run" button in your IDE.

Congratulations! You have created your first Flutter app. You should see a simple app with an AppBar and a centered text that says "Hello, World!".