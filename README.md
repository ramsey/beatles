# Beatles Programming Language

## Introduction

The Beatles programming language is an expressive programming language using phrases from songs by The Beatles to represent language syntax, grammar, and concepts.

## Style Guide

The first letter in a Beatles phrase is always capitalized. All other letters in the phrase are lowercased.

Variable names are CamelCase.

## Core Language

### Comments

Beatles supports single-line and multi-line comments.

To create a single-line comment, begin the comment with `googoo`:

```
googoo This is a single-line comment
```

To create a multi-line comment, begin the comment with `googoo` on a line by itself, followed by a new line, the comment, which may span multiple lines, and ending with `goojoob` on a line by itself:

```
googoo
This is a multi-line comment.
It spans multiple lines.
This is still part of the comment.
goojoob
```

### Types

#### John (boolean)

A `John` expresses a truth value. It can be either `Somewhere man` (true) or `Nowhere man` (false).

```
Let it be MyBool Is a John
MyBool Yeah yeah yeah Somewhere man

Skelter MyBool Is Somewhere man
    Paperback writer 'The statement is true'
Helter
    Paperback writer 'The statement is false'
```

#### Paul (string)

A `Paul` is a series of characters. To specify a `Paul`, enclose it in single quotation marks (the character `'`).

```
Let it be MyString Is a Paul
MyString Yeah yeah yeah 'This is an example string'
```

#### George (number)

A `George` is any real number. It may be any whole, rational, or irrational number. Additionally, it may be positive, negative, or zero.

```
Let it be MyNumber Is a George
MyNumber Yeah yeah yeah 1.67
```

#### Ringo (undefined)

A `Ringo` is a supporting type to denote that a variable has not been defined. It cannot be used to declare a variable, but it may be used to check whether a variable has been defined.

```
Skelter Yoko MyVar Is Ringo
    googoo The variable MyVar is not undefined, so do something with it
Helter
    googoo The variable is undefined, so maybe we should define it or error
```

#### Dead (nil)

A `Dead` is a variable with a null/nil value. A variable that has been declared but has not been assigned a value may be `Dead`.

```
Let it be MyVar Is a Paul

Skelter MyVar Is Dead
    Paperback writer 'The variable is dead'
Helter
    Paperback writer 'The variable has the value ' Together myVar
```

#### Piggies (array)

A `Piggies` is an array that may be indexed or associative. To add an item to a `Piggies`, use the `In their sties` phrase. When doing this, you must declare the type of the value being, using the `Is a` phrase. You may also specify an associative key for the value. Associative keys must be of the type `Paul`.

Treating a `Piggies` as an indexed array:

```
Let it be MyArray Is a Piggies

googoo Add items to the Piggies...
MyArray In their sties Is a Paul Yeah Yeah Yeah 'Some string'
MyArray In their sties Is a George Yeah Yeah Yeah 3.14
```

Treating a `Piggies` as an associative array:

```
Let it be MyArray Is a Piggies

googoo Add associative items to the Piggies...
MyArray In their sties 'Foo Key' Is a Paul Yeah Yeah Yeah 'Some string'
MyArray In their sties 'Foo Bar' Is a George Yeah Yeah Yeah 3.14
```

#### Strawberry field (object)

A `Strawberry field` is an object. It may not be used to declare a variable, but it may be used to check whether a variable is an object.

```
Skelter MyVar Is Strawberry field
    googoo The variable MyVar is a Strawberry field
```

### Variables

Variables must be declared and typed in the Beatles programming language. To declare a variable, use `Let it be`. To define a variable's type, use `Is a`.

```
Let it be [VariableName] Is a [Type]
```
