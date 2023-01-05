---
title: "Types of High Level Languages"
date: 2023-01-04T13:47:40Z
draft: false
featured_image: https://wallpapercave.com/wp/wp7457469.png
toc: true
categories:
  - "mentee or client"
summary: Get to know the inspiration behind the design of programming languages.
tags:
  - programming
  - theory
  - paradigms
  - basics
---

<!--
TODO:
- Building a right perspective
- Understanding from people who are in the field how things work and how you can be successful.
- Some encouragement: "Don't allow people's insecurities become your limitations."
- Programming terms.
- Data abstraction & problem solving.
-->

## What is a High-level Language

High-level languages allow a programmer to write instructions for the computer to execute, independent of a particular type of computer. It abstracts the details of the computer from the programmer. Their syntax is more understandable by humans.

Unlike low-level languages, the programmer does not need to focus on the computer's hardware, register names or any details about how a computer works. Due to the layers of abstraction introduced by high-level languages, programmers can solve very complex problems.

In the previous article, we mentioned that high-level languages can be broken down into two main categories based on paradigms (i.e. patterns):

- Imperative languages.
- Declarative languages.

{{< notice info >}}
In 1957, FORTRAN (Formula Translation) was introduced by IBM. John Backus, the program director of FORTRAN, said: _"Much of my work have come from being lazy. I didn't like writing programs, and so, I started work on a programming system to make it easier to write programs."_
{{< /notice >}}

{{< notice success >}}
A programmer's laziness has been the backbone of many significant technological breakthroughs.
{{< /notice >}}

## Imperative Languages

An imperative programming paradigm specifies the sequence of steps the computer must take to complete a task. Imperative language design allows a programmer to describe how a program operates step by step rather than giving high-level descriptions of expected results. E.g. FORTRAN, COBOL, BASIC and Pascal.

{{< notice info >}}
The programming paradigm used to build programs for almost all computers typically follows an **imperative model**.
{{< /notice >}}

Imperative languages can be further broken down into two types:

- Procedural languages.
- Object-oriented languages.

### Procedural Languages

Procedural programming is a type of imperative programming in which the program is built from one or more procedures. Procedural language design focuses on grouping instructions into procedures. These procedures can be called at any point during a program's execution. E.g. COBOL and BASIC.

Let's take a journey to calculus. Suppose one wanted to determine the definite integral of a function. In that case, one must check for specific conditions and apply a suitable formula. In procedural programming, the instructions to test for each condition can be grouped into _procedures_. In solving the main problem, finding the definite integral, the _procedures_ are called to execute their part in calculating the definite integral.

To solve the problem above, one needs to follow a step-by-step procedure to get the desired result. For this reason, procedural languages are considered imperative languages.

### Object-oriented Languages

Another type of an imperative language is object-oriented language. These languages use _objects_ rather than procedures to group and execute instructions. The behaviour of _objects_ is described by methods under a single interface called a _class_. Examples of Object-oriented Programming languages are Simula, C++, Java and Python.

Let's assume our entire body is a program to better understand how object-oriented languages work. In our program, we have classes which could be likened to the systems in our bodies. To narrow our scope, let's take the digestive system as a focus. In the digestive system, we have organs which perform various functions with the same goal of digesting food.

{{< notice info >}}
**Note:** In a class, all the objects perform different functions. Still, they are related to each other to achieve a common goal or to solve a particular problem.
{{< /notice >}}

Organs like the stomach, oesophagus, pancreas and small intestine can be our methods. The way they function describes the behaviour of an _object_. For instance, the stomach has a step-by-step procedure to digest proteins and break down bones with HCL. If an object is created from the _digestive system_ class, it has access to the _methods_, which in this case are the _organs in the digestive system_. If we want the _object_ to digest protein and dissolve bones, we can call on the _stomach_ method. The _stomach_ method executes step-by-step instructions to solve that problem.

Since methods instruct the computer step by step on what to do, it is considered an imperative language.

## Declarative Languages

Aside from imperative languages, there is another category called declarative languages. Unlike imperative languages, they do not instruct the computer on what to exactly do. Instead, they express the logic of a computation. Declarative languages deal with what the program must accomplish and not how to accomplish it. Examples of declarative languages are SQL, HTML, Markdown, and Prolog.

Declarative languages can also be broken down into two types:

- Functional languages.
- Logic languages.

### Functional Languages

These languages, as the name suggests, are based on functions to transform some input into a specific output without having to specify every step of the process. What sets functional languages apart from imperative languages is that they never change the original data or program state, whereby their counterpart's goal is mainly to specify steps to change the state of the program to solve a problem.

In a more technical sense, functional programming language design deals with defining expressions that map values to other values rather than a sequence of imperative statements which update the running state of a program.

A good example is the quadratic formula in maths. The formula does not tell the student what to do. Instead, it defines an expression such that if the student puts in a value, they get another value based on the defined expression.

Examples of functional programming languages include Common Lisp, OCaml and Haskell.

{{< align center "**Double a number lisp**" >}}

```lisp
(defeun double (x) (* x 2))
(double 2)
;;; Outputs 4
```

### Logic Languages

Logic languages are designed to define a set of facts and rules about a problem domain instead of how to solve it. The _"what to do"_ is left for the computer to figure out. An example of a logic language is Prolog (PROgramming in LOGic).

{{< align center "**Sample program in prolog**" >}}

```prolog
/*  This is a sample code in prolog to determine if Tom will eat Jerry
    source: Wikipedia https://en.wikipedia.org/wiki/Declarative_programming
*/

% cat is an animal
animal(cat)

% mouse is an animal
animal(mouse)

% Tom is a cat
cat(tom)

% Jerry is a mouse
mouse(jerry)

% cat is big
big(cat)

% mouse is small
small(mouse)

% Mouse eats cheese
eat(mouse, cheese)

% Big animals eat small animals
eat(big, small)

% Question for our program: Will Tom eat Jerry?
?- eat(tom, jerry)
```

{{< notice warn >}}
What do you think the output of the code will be? \
Will Tom eat Jerry?
{{< /notice >}}

In the program above, instead of defining steps for the computer to follow to know if Tom will eat Jerry, a series of facts and rules were given to the computer to enable it to make the decision.

## How Computers Run High-level Languages

The caveat here is, computers do not understand high-level languages directly, so they had to be transformed into a format that the computer can understand and execute. These programs are called translators.

{{< color "orange" "**Translators**" >}} are programs that convert source code into a format that the computer can understand. A translator can take many forms depending on its function and the type of source code. If the source code is written in assembly language, then the translator is called an {{< color "orange" "**assembler**" >}}. If the source code is converted into binary format line by line, then the translator is called an {{< color "orange" "**interpreter**" >}}. Finally, if the entire source code is converted into binary format (which is called the object code), then the translator is called a {{< color "orange" "**compiler**" >}}.

{{< notice info >}}
Grace Hopper built the first compiler in 1952.
{{< /notice >}}

Examples of languages that can be intrepreted are Python and julia.

Examples of languages that can be compiled are C/C++, Java and Go.

{{< notice success >}}
The programming community was sceptical about the performance of high-level languages in the early years. Nonetheless, since they could write code more quickly, it made it an easy choice economically. Trading a slight increase in computation time for a significant decrease in programming time was worth it.
{{< /notice >}}

## Some Hello World Programs

### BASIC

```basic
PRINT "Hello, World!"
```

### Python

```python
print("Hello, World!")
```

### Javascript

```js
console.log("Hello, World!");
```

### C++

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, World!";
}
```

### Java

```java
class Hello {
    public static void main(String[] args){
        System.out.println("Hello World!");
        }
}
```

### Julia

```julia
println("Hello, World!")
```

### Go

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

## Conclusion

Most programming languages in use today are multi-paradigm -- meaning they overlap in the categories of high-level languages. Knowing the different paradigms is essential as it will enable you to benefit from the features and opportunities each style offers. That is the key to coding with maximum effectiveness.
