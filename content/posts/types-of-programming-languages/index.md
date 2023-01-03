---
title: "Types of Programming Languages"
date: 2023-01-03T06:35:47Z
draft: false
toc: true
featured_image: https://images.pexels.com/photos/879109/pexels-photo-879109.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1
categories:
  - mentee or client
summary: The types of programming languages and why each style is important
tags:
  - programming
  - theory
---

<!--
TODO:
- Building a right perspective
- Understanding from people who are in the field how things work and how you can be successful.
- Some encouragement: "Don't allow people's insecurities become your limitations."
- Programming terms.
- Data abstraction & problem solving.
-->

Yesterday, we looked at how computers have evolved through the years. In this article, we will learn about how programming languages have progressed. But before we delve into the various categories and types of programming languages, let's look at what programming means.

## What is Programming

Martin O'Hanlon says, **"Programming is how you get computers to solve problems"**. How can you get a computer to solve problems? By giving it instructions for it to execute. These instructions are what we refer to as computer programs.

## Programming's Evolution

Computers are electronic machines, meaning they do not understand human language -- they communicate through electric currents. In the early stages of programming, it was nothing more than using switches to turn on/off currents to get a computer to solve a problem.

{{< notice info >}}
Electric current has only two states: _on_ or _off_. For this reason, computers only knew how to execute programs in binary (i.e. 0s and 1s). However, humans do not understand binary :thinking:
{{< /notice >}}

### Why Were Programming Languages Created

Computer engineers were doing just fine creating complex circuit systems to understand, read and compute data from memory. However, if the programmer needed to perform another task, they needed to reconfigure the whole circuit, which was very laborious and time-consuming.

John Von Neumann designed the Von Neumann architecture to cater for this complexity.

![Von Neumann architecture. Credit: Wikipedia](https://upload.wikimedia.org/wikipedia/commons/e/e5/Von_Neumann_Architecture.svg)

The architecture design comprised of:

- A Central Processing Unit with an Arithmetic Logic Unit (ALU) and processor registers.
- A Control Unit that included an instruction register and a program counter.
- Memory to store data and instructions for the computer.
- Input/output mechanisms.

{{< notice info >}}

- A processor register is a quickly accessible location available to a computer's CPU.
- An instruction register is the part of the control unit that holds the instruction currently being executed.

{{< /notice >}}

{{< notice success >}}
Von Neumann's architecture is still the blueprint for modern computers today.
{{< /notice >}}

Still, it wasn't enough. Consequent innovations like plug boards and punched paper could not handle the complexity and did not allow programmers to take full advantage of what computers could do. What was needed was a simpler way to give instructions to the computer. This gave birth to programming languages.

## Fundamental Types Of Programming Languages

At its core, programming languages can be categorised two:

1. Low-level languages
2. High-level languages

### Low-level Languages

These are languages that are closer to a computer's hardware. They are difficult for humans to understand and provide little to no abstraction from a system's architecture. Machine code and assembly language are types of low-level languages.

**Machine Language:** It is the language the computer speaks and understands. It consists of binary or hexadecimal instructions for the computer to execute. Machine language is hardware dependent. This means machine code written for one type of hardware cannot work on any other hardware.

{{< youtube aPHAxFAwC7g >}}
{{< align center "Hello World in x86 machine code" >}}

**Assembly Language:** Assembly language uses mnemonics, numbers and symbols instead of 0s and 1s for designing computer programs. It is machine-dependent. This means the program can work on only the type of computer it was designed for. For example, the Assembly language for Intel computers is different for Apple computers.

```asm
; ----------------------------------------------------------------
; Writes "Hello, World" to the console using only system calls.
; Runs on 64-bit Linux only. To assemble and run:
;
;     nasm -felf64 hello.asm && ld hello.o && ./a.out
; ----------------------------------------------------------------

          global    _start

          section   .text
_start:   mov       rax, 1                  ; system call for write
          mov       rdi, 1                  ; file handle 1 is stdout
          mov       rsi, message            ; address of string to output
          mov       rdx, 13                 ; number of bytes
          syscall                           ; invoke operating system to do the write
          mov       rax, 60                 ; system call for exit
          xor       rdi, rdi                ; exit code 0
          syscall                           ; invoke operating system to exit

          section   .data
message:  db        "Hello, World", 10      ; note the newline at the end
```

{{< align center "Hello World program for 64-bit Linux systems" >}}
Check out the assembly code variations on different types of computers [here.](https://cs.lmu.edu/~ray/notes/x86assembly/)

{{< notice info >}}
Choosing between machine language and assembly language has its pros and cons. [Learn more.](https://www.geeksforgeeks.org/difference-between-machine-language-and-assembly-language/)
{{< /notice >}}

### High-level Lanaguages

High-level languages are programming languages that allow a programmer to write instructions for the computer to execute, independent of a particular type of computer. It abstracts the details of the computer from the programmer. Consequently, they are closer to human language.

High-level languages can be further broken down into different categories based on their paradigm (i.e. patterns):

- Imperative languages.
  - Procedural languages.
  - Object-oriented languages.
- Declarative languages.
  - Functional languages.
  - Logic languages.

Some languages are multi-paradigm (i.e. they support more than one programming paradigm).

Examples of high-level programming languages include: Python, Java, C++, Go, Ruby, Perl, BASIC, Pascal and FORTRAN.

> Most programming languages support more than one programming paradigm to allow programmers to use the most suitable programming style and associated language constructs to solve a specific problem.

{{< notice info >}}
**Is C/C++ a low-level language?:** They are high-level languages because programs written in C/C++ are independent of a particular type of computer. They are closer to the user than a computer's hardware. The level of abstraction defines how "high-level" a language is. In general, C/C++ are high-level languages but compared to languages like python, which has a stronger abstraction, they can be viewed as low-level languages.
{{< /notice >}}

## Fun Facts

- The largest punch card program was from the 1950's SAGE Air Defence System, which used 62,500 punched cards. At its peak, it employed about 20% of the world's programmers.

## Conclusion

The next article will focus on high-level languages and their subcategories.
