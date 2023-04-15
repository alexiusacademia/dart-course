# Module 5: Collections

In this module, we will explore collections in Dart, which are used to store and manipulate groups of values.

<br/>

## Lists

A list is an ordered collection of objects, where each object can be accessed by an index. In Dart, lists can contain objects of any type, including other lists. Here's an example of how to declare and initialize a list in Dart:

```C
List<String> fruits = ['Apple', 'Banana', 'Orange'];
```

You can access an element in the list using its index:

```C
print(fruits[0]); // Apple
```

You can also add or remove elements from the list:

```C
fruits.add('Mango');
print(fruits); // [Apple, Banana, Orange, Mango]

fruits.removeAt(1);
print(fruits); // [Apple, Orange, Mango]
```

<br/>

## Sets

A set is an unordered collection of objects that does not allow duplicates. In Dart, sets can contain objects of any type, including other sets. Here's an example of how to declare and initialize a set in Dart:

```C
Set<int> numbers = {1, 2, 3, 4};
```

You can add or remove elements from the set:

```C
numbers.add(5);
print(numbers); // {1, 2, 3, 4, 5}

numbers.remove(2);
print(numbers); // {1, 3, 4, 5}
```

<br/>

## Maps

A map is a collection of key-value pairs, where each key maps to a value. In Dart, maps can have keys and values of any type, including other maps. Here's an example of how to declare and initialize a map in Dart:

```C
Map<String, String> capitals = {
  'USA': 'Washington D.C.',
  'Canada': 'Ottawa',
  'Mexico': 'Mexico City'
};
```

You can access a value in the map using its key:

```C
print(capitals['USA']); // Washington D.C.
```

You can also add or remove key-value pairs from the map:

```C
capitals['France'] = 'Paris';
print(capitals); // {USA: Washington D.C., Canada: Ottawa, Mexico: Mexico City, France: Paris}

capitals.remove('Mexico');
print(capitals); // {USA: Washington D.C., Canada: Ottawa, France: Paris}
```

In the next module, we will explore classes and objects in Dart.