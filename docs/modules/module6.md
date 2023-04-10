# Module 6: Classes and Objects

In this module, we will explore classes and objects in Dart, which are used to model real-world entities and encapsulate data and behavior.

<br/>

## Classes and Objects

A class is a blueprint for creating objects that define the properties and behavior of the object. An object is an instance of a class that contains data and behavior. Here's an example of how to declare a class in Dart:

```C
class Person {
  String name;
  int age;

  void sayHello() {
    print('Hello, my name is $name');
  }
}
```

You can create an object of a class using the "new" keyword and the class constructor:

```C
Person john = new Person();
john.name = 'John';
john.age = 30;
john.sayHello(); // Hello, my name is John
```

<br/>

## Constructors

A constructor is a special method that is called when an object is created. It is used to initialize the object's properties. In Dart, there are two types of constructors: default constructors and parameterized constructors. Here's an example of how to declare a parameterized constructor in Dart:

```C
class Person {
  String name;
  int age;

  Person(String name, int age) {
    this.name = name;
    this.age = age;
  }

  void sayHello() {
    print('Hello, my name is $name');
  }
}
```

You can create an object using the parameterized constructor:

```C
Person john = new Person('John', 30);
john.sayHello(); // Hello, my name is John
```

<br/>

## Inheritance

Inheritance is a mechanism that allows a class to inherit properties and behavior from a parent class. In Dart, a class can inherit from a single parent class using the "extends" keyword. Here's an example of how to declare a class that inherits from another class in Dart:

```C
class Student extends Person {
  String major;

  Student(String name, int age, String major) : super(name, age) {
    this.major = major;
  }

  void sayMajor() {
    print('My major is $major');
  }
}
```

You can create an object of the child class and access its properties and behavior:

```C
Student jane = new Student('Jane', 20, 'Computer Science');
jane.sayHello(); // Hello, my name is Jane
jane.sayMajor(); // My major is Computer Science
```

<br/>

## Getters and Setters

Getters and setters are special methods that are used to access and modify the properties of an object. In Dart, you can declare getters and setters using the "get" and "set" keywords. Here's an example of how to declare a getter and a setter for a property in Dart:

```C
class Person {
  String _name;
  
  String get name => _name;
  
  set name(String value) => _name = value;

  void sayHello() {
    print('Hello, my name is $name');
  }
}
```

You can access the getter and setter using the property name:

```C
Person john = new Person();
john.name = 'John';
print(john.name); // John
```

In the next module, we will explore exception handling in Dart.