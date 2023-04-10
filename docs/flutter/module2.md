# Lesson 2: Building Flutter UIs

In this lesson, we will dive deeper into building Flutter UIs. You will learn how to use different types of widgets, how to create layouts, and how to handle user input.

## Understanding Flutter Widgets

In Flutter, everything is a widget. Widgets are the building blocks of a Flutter app and can be either structural or stylistic. Structural widgets define the layout and hierarchy of your app, while stylistic widgets define the appearance of your app.

Flutter comes with a rich set of pre-built widgets that you can use to build your app. These widgets are organized into categories based on their functionality. Some of the most commonly used widget categories include:

Text and Typography: Used for displaying text in your app.
Buttons: Used for creating clickable buttons in your app.
Input and Selection: Used for accepting user input and making selections, such as text fields, radio buttons, and checkboxes.

Containers: Used for creating visual elements in your app, such as boxes, images, and icons.
Layouts: Used for arranging widgets on the screen, such as rows, columns, and grids.
Creating Layouts
In Flutter, you can create layouts using a combination of structural widgets. The most commonly used structural widgets for layout are Row, Column, and Container.

Here is an example of a simple layout created using Row and Column widgets:

```
import 'package:flutter/material.dart';

void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('My First Flutter Layout'),
        ),
        body: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            Row(
              mainAxisAlignment: MainAxisAlignment.center,
              children: <Widget>[
                Container(
                  width: 50,
                  height: 50,
                  color: Colors.red,
                ),
                Container(
                  width: 50,
                  height: 50,
                  color: Colors.blue,
                ),
                Container(
                  width: 50,
                  height: 50,
                  color: Colors.green,
                ),
              ],
            ),
            SizedBox(height: 30),
            Text(
              'Hello, World!',
              style: TextStyle(fontSize: 24),
            ),
          ],
        ),
      ),
    ),
  );
}
```

In this example, we create a Column widget that contains two child widgets: a Row widget and a Text widget. The Row widget contains three child widgets, each represented by a Container widget with a different color.

## Handling User Input

In Flutter, you can handle user input using input widgets such as TextField, Checkbox, and Radio. Here is an example of a simple form created using TextField and RaisedButton widgets:

```
import 'package:flutter/material.dart';

void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('My First Flutter Form'),
        ),
        body: Padding(
          padding: EdgeInsets.all(16),
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
            children: <Widget>[
              TextField(
                decoration: InputDecoration(labelText: 'Name'),
              ),
              SizedBox(height: 16),
              TextField(
                decoration: InputDecoration(labelText: 'Email'),
              ),
              SizedBox(height: 16),
              RaisedButton(
                child: Text('Submit'),
                onPressed: () {},
              ),
            ],
          ),
        ),
      ),
    ),
  );
}
```

In this example, we create a form with two TextFields and a RaisedButton. The TextFields allow the user to input their name and email, and the RaisedButton is used to submit the form.