---
title: "The Key to Studying Multiple Languages"
date: 2023-05-15T03:24:07Z
draft: false
toc: true
featured_image: https://images.pexels.com/photos/3767411/pexels-photo-3767411.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1
summary: Programming languages are tools, not solutions
tags:
    - basics
    - programming
    - keys
---

## Introduction

The learning curve of studying programming languages is exponential rather than linear. It is common for students to say, "I don't get all this", "Why can't everything be done in python?"; "Why do I need C/C++", or "Java is the worst". These are valid thoughts for students, but ultimately this happens because we forget or are not taught the essence of programming. Programming was invented to solve problems. If this fundamental truth is lost, we tend to see programming languages as the solution rather than a tool. Let's explore how we can understand use these tools.

{{< quote-center >}}
*"The ultimate goal of programming is to solve problems. If this fundamental truth is lost, we tend to see programming languages as a solution rather than a tool."* - **DaveSaah**
{{< /quote-center >}}

## Disclaimer

This article is a guide on how to study programming languages. It seeks to show the reader the core concepts of programming languages and how to apply them to any language. This article is subjective to my experience and understanding of programming languages, not an absolute truth.

## The Structure of Programming Languages

All programming languages are built on the core principles of problem-solving and the fundamental concepts of logic. This article will highlight the features of programming languages and break them down for us to understand.

We can look at the structure of programming languages in four categories:

1. Basics.
2. Intermediate.
3. Language-specific features.
4. Advanced.

## Basics

The basic concepts under programming language structure include:

- Data types / primitives.
- Data structures / collection types.
- Operators.
- Expressions & statements.
- Assignments & variables.
- Constants.
- Input/output statements.
- Conditionals.
- Loops.
- Functions.

### Data types / Primitives

The first thing to study about a programming language is to know what data types are. It is essential because it helps you understand how to store and manipulate data in your programs.

A data type specifies a set of values with the same operations defined for them. Let's consider an integer which is a data type. This means that any value specified as an integer has a defined set of operations that can be performed on it. An example is addition.

Though operations might overlap between various data types, their behaviours are always different. For instance, addition operation on strings is defined in ***python***, but its behaviour is different from that of integers. The later joins the strings together to form a new string while the former adds two integers together to get a single result.

Data types can either be primitive or a collection. A **primitive** is a data type that cannot be decomposed into other data types while **collection** data types can be decomposed into 'smaller' data types.

Examples of primitive data types are:

- **Integers:** Positive and negative whole numbers including 0. E.g. 1, 2, 3, ...
- **Floats:** Numbers with decimal points. E.g. 0.1, 1.2, 1.0, ...
- **Boolean:** Values that represents true or false.
- **Char:** Single characters including letters, symbols and numbers. They are often represented with single quotes (`''`). E.g. 'a', '1', '$', ...

### Data structures / collection types

We earlier stated that a data type can either be primitive or a collection. Collection data types can be called data structures. A collection data type or a data structure is a collection of data types (mostly primitives) arranged in a specific order.

Most programming languages come with pre-defined collection data types. The table below give examples of pre-defined collection data types in Go and python.

| Go | Python |
| --- | --- |
| Slices | Dictionaries |
| Arrays | Tuples |
| Maps | Lists |
| Structs | Sets |

A more advanced concept will be custom data structures. Examples of those include stacks, linked lists, trees, etc ... but those are outside the scope of this article.

You might be asking why the need for collection data types? Well, two of the most valuable resources for a computer program are **time** and **memory**. The knowledge of data structures will allow you to choose the right data types and a way of arrangement (type of data structure) such that the data you're working with can be accessed and updated efficiently.

### Operators

If you recall, data types have a set of operations defined for them. These operations perfomed on data are represented by operators. Operators can be categorised into 4:

1. **Arithmetic operators:** These represent arithmetic operations like addition, subtraction and multiplication.
2. **Comparison / Relational Operators** These operators are used for comparison operations. They return a truth value. Examples include equality operations, greater than operations, etc.
3. **Logical operators:** They perform operations on boolean values. In the mathematical sense, they are used to form compound boolean expressions.
4. **Bitwise operators:** They perform operations on individual bits (i.e. 0s and 1s) within a binary representation of data.

{{< align center "**Table of Operations**" >}}

| Arithmetic Operator | Operation |
| --- | --- |
| Addition (+) | Adds two values together. Also used in some languages to concantenate (i.e. join) strings. |
| Subtraction (-) | Gets the difference between two values |
| Multiplication (\*) | Multiplies two values together |
| Division (/) | Finds the quotient of two values |
| Modulus (%) | Finds the remainder of an integer value |

{{< notice info >}}
Some programming languages may have slightly different behaviour of operations based on the data type. For example, Java performs integer division when `/` operator is used with integers, whereas `//` operator is used in python to perform integer division regardless of the number being an integer or a float.
{{</ notice >}}

| Relational Operator | Operation |
| --- | --- |
| > | Greater than |
| < | Less than |
| >= | Greater than or equals |
| <= | Less than or equals |
| == | Equality |
| != | Not equal |

{{< notice info >}}
An operand is a value used in a operation. For example, an addition operation is denoted by 1 + 2, where 1 and 2 are the operands.
{{</ notice >}}

| Logical Operators | Operation |
| --- | --- |
|`\|\|` | Boolean OR; returns *true* if at least one of its operands are true, else it returns *false* |
| `&&` | Boolean AND; returns *true* if both of its operands are *true*, else it returns *false* |
| `!` | NOT; reverses the truth value of a boolean expression |

{{< notice info >}}

- The above tables are not exhaustive. A few operations like exponentiation is represented differently across various programming languages. Nonetheless, the concept of how they work remains the same.
- Bitwise operations are slighly advanced and do not fit in the basic category. There is a separate section for it later in this article.

{{</ notice >}}

### Expressions & Statements

The next step is combining values and operators to get a certain value. This gives birth to expressions. An expression is a combination of values, operators or variables that represents a single result. Examples of expressions: `1 + 1` and `12 * 4`.

In general, when code is written, it is to instruct the computer on what to do. These chunks of instructions can be separated into statements. A statement can use expressions in its construct. A statement is defined as a section of code that represents a command or an action. Examples are if-statement and loops.

### Assignments & Variables

At this stage we can say that a program is a series of statements. But then we have a problem. Each time we need a certain value, we need to hard code the value, or define an expression that represents it every time. Things start to get messy when you have many lines of code. In this situation, variables become very handy.

A variable is a name that represents a value. It allows values or expressions to be stored under a name that can be referenced throughout the life cycle of a computer program. Each programming language have naming conventions for variables. The default rule of thumb is that a variable name must be descriptive of the value it holds.

{{< notice info >}}

- Variables can change in the lifecycle of a program.
- Values are stored in a variable via an assignment statement.
- Just like naming conventions, different programming languages have different ways of assigning values to variables.

{{</ notice >}}

### Constants

A constant is a special type of variable that does not change.

### Input/Output statements

We will not always define values in our program. There are times (if not most of the time), inputs are taken from a user and processed for further operations. After computation, a response needs to be given. These responses are output statements.

### Conditionals

After learning how to write programs as a sequence of statements, the next thing to look at is conditionals. Conditionals are statements that execute lines of code based on a specified condition. Conditionals are implemented in programming languages as **if-statements** and **switch** cases.

{{< notice info >}}
Using conditionals in a program can also be referred to as branching. Since they control the flow of a program, they are also called control flow statements.
{{</ notice >}}

### Loops

Loops allow a block of code to run continously till a condition is met. They also fall under control flow statements. The difference between loops and conditionals is that the former runs a block of code more than once, while the later runs a block of code only once.

When the endpoint of a loop is known, it can be specified at the start of the loop. This type of loop is called a **for statement**. However, if the endpoint of loop is not known, but based on a condition, the loop is implemented as a **while statement**.

{{< notice info >}}
The for loop can perform the work of a while loop and vice versa. They were implemented to solve different problems in code design. Take time to explore them.
{{</ notice >}}

### Functions

The last concept under the basic structure of programming languages are functions. Just like in Math, a function can take an input and return a certain output. The inputs of a function are its arguments and the output of a function is its return value.

Functions in programming are used for more than just input and output. Earlier we mentioned that we cannot be hardcoding values throughout our program -- things could get messy. In the same light imagine writing the same blocks of code over and over again in your program. This is known as code duplication and is strongly discouraged in software developement. Just like variables, we can group this statement under a common name. This name is the name of a function.

Does it mean that we can group any series of statements as a function? No! A function group a series of statements that perform a common function. For example, validating if a person is an adult, calculating the area of polygons, etc.

{{< notice info >}}
The concept of grouping blocks of code together under a common name is called **encapsulation**
{{</ notice >}}

## Intermediate

The intermediate concepts under programming language structure include:

- Data streams. E.g. files.
- Error handling.
- Pointers.
- Testing.

### Data streams

"Data streams" might not be the best phrase to use, but I use it to refer to other means of accessing and manipulating data apart from variables. Good examples are files and databases.

### Error handling

Another intermediate concept is error handling. This is useful for handling issues with conflicting data types, type conversion and input validation.

### Pointers

A pointer gets the address of variable stored in memory. Common use cases of pointers are:

- It enables programmers to manipulate and update large streams of data without repopulating the entire data in memory.
- It allows faster access to data in memory with the use of pointer arithmetic.
- It enforces API consistency.

### Testing

<!-- Find a quote about bugs and testing -->
There is no perfect software, else programmers would be out of jobs. Testing can be thought of as compound error handling. Syntax and data errors are easier to spot, but testing are useful for semantic errors.

{{< notice info >}}
A semantic error occurs if a program does not crash but does not perform the task it was designed for. It is an error in the meaning of an instruction.
{{</ notice >}}

## Language Specific Features

Aside the core concepts that all programming languages share, there are some implementations that are specific to a programming language. We can call them language specific features. Some of these features are:

- Built-in functions / libraries. E.g. `print()` in Python, `System.out.println()` in Java.
- Data structures. E.g. Lists in Python is synonymous to ArrayLists in Java.

{{< notice warn >}}
The list above is not exhaustive. Language specific features can be found in the documentation of the respective programming language.
{{</ notice >}}

## Advanced

### Bitwise Operations

Though bitwise operations falls under the categories of operators, it is a slightly advanced concept that deals with the binary manipulation of data. It is common in low-level languages, but seldom used in modern programming languages. Nonetheless, the table below describes the common bitwise operators and their operations.

| Bitwise Operators | Operation |
| --- | --- |
| Bitwise AND (`&`) | Compares two binary numbers bit by bit and returns 1 if both bits are 1,
| | otherwise, it returns 0 |
| Bitwise OR (`\|`) | Compares two binary numbers bit by bit and returns 1 if at least one of the bits is 1,
| | otherwise, it returns 0 |
| Bitwwise XOR (`^`) | Compares two binary numbers bit by bit and returns 1 if the bits are different,
| | else it returns 0 |
| Bitwise NOT (`~`) | Takes a single operand and inverts its bit (i.e. from 0 to 1 and vice versa) |
| Left shift (`<<`) | Shifts the bits of a binary number to the left by a specified number of positions. |
| Right shift (`>>`) | Shifts the bits of a binary number to the right by a specified number of positions. |

{{< notice info >}}
Some of the bitwise operator symbols may vary in different languages.
{{</ notice >}}

To keep this article short, we will not go into the details of other advanced concepts. However, we will list them below:

- Package Management & Modules
- Build Tools
- The use of frameworks
- Design patterns

## Concluding Thoughts

Have the layers of abstraction introduced into programming languages caused more harm than good? It's hard to say. The computer got powerful through many layers of abstraction. Programmers can utilise the power of a computer because of the layers of abstraction present in modern-day languages. However, there is a cost -- the foundation can get lost.

### The Way Forward

Do we have to understand how everything works under the hood? That would be great, but it is not so practical. Of course, some programmers understand how everything works, and learning multiple languages is a breeze. However, we are all not the same. Programming in multiple languages is a skill that can be learned. Sometimes, all we need is a guide, and this article seeks to fill that gap.

Until we meet in the next article, keep solving problems.
