---
title: "The Two Main Skills for Programming"
date: 2023-01-08T17:44:37Z
draft: false
toc: true
categories:
    - "mentee or client"
summary: If you want to stand out as a programmer, master these skills
featured_image: https://images.pexels.com/photos/4974915/pexels-photo-4974915.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1
tags:
    - skills
    - programming
    - top-secret
refs:
    - link: https://www.verywellmind.com/what-is-abstract-reasoning-5181522
---

## Introduction

I wrote my first code in 2018 (It was in HTML). My first "Hello, World!" program was in BASIC in the same year. My software development journey has been self-taught. I learnt a lot by asking people for help, making use of Google, YouTube, documentations, as well as learning by trial and error. From BASIC, I learned Javascript, C++, Python, Java, and Go, just to name a few. From my experience, I realised that two fundamental skills are needed to be a good programmer.



{{< notice info >}}
**BASIC** stands for Beginners' All-purpose Symbolic Instruction Code
{{< /notice >}}

These skills are {{< color "orange" "problem-solving" >}} and {{< color "orange" "abstract thinking" >}}.

## Problem Solving

I define problem-solving as breaking down complex problems into simpler ones. Solving the simpler problems becomes the building blocks to solving the complex problem. There is no standard way of solving problems. However, the process involves understanding the problem, describing the requirements, and the steps needed to implement the solution.


The thought process of problem-solving is primarily expressed as algorithms.



{{< notice info >}}
An algorithm is a sequence of intructions used to complete a task. It can be expressed in 3 forms: pseudocode, flowcharts, and actual code.
{{< /notice >}}

### Why is Problem Solving Important?

As a software developer, your job is to write programs. But what is a program :thinking:? A **computer program** is a {{< color "green" "sequence of instructions" >}} for a computer to execute. Wait!!! An **algorithm** is a {{< color "green" "set of instructions" >}} used to complete a task. That's not all. The thought process of **problem-solving** is expressed in algorithms.

{{< notice success >}}
Writing software is basically problem-solving; nothing more, nothing less.
{{< /notice >}}

Building this skill allows you to focus more on solving a problem than on a programming language's features. It gives you the perspective of seeing a programming language as a tool rather than a solution.

## Abstract Thinking

As an introvert, I am naturally wired with this skill. I didn't know that it made me understand problems and derive solutions easier in ways people would not have ordinarily thought of. You do not need to be an introvert to think abstractly. It is a skill that can be learnt. But what is abstract thinking in the first place?

**Abstract thinking** is the ability to understand complex concepts that, while real, are not tied to concrete experiences, objects, people or situations[$^{[1]}$](https://www.verywellmind.com/what-is-abstract-reasoning-5181522). There are many concepts and technologies you'll need to work with that will not make sense to you if you try to reason them out.

{{< notice info >}}
In abstract thinking, it is more important to:

- See *why* something is.
- Focus on the bigger picture rather than the specifics of a situation.

{{< /notice >}}

### How Does Abstract Thinking Fit Into Programming?

Let's use an example of an interface design. Let's say we need to develop a calculator. The natural approach will be to write numerous functions for each mathematical operation. That is good, but maintenance becomes problematic. The abstract thinker will look at the bigger picture of what a calculator does.

![](https://images.pexels.com/photos/8371719/pexels-photo-8371719.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)

{{< align center "**An example of my thought process**" >}}

- Calculators perform different mathematical operations.
- We can separate these operations into functions.
- However, if I want to update functions or extend the capability of the calculator, I'll have to write more functions. If I'm working with others, or if I have to maintain this myself, I need to make it easier to understand.
- What can I do? Okay, mathematical operations fall under different categories. They can arithmetic calculations, vector calculations, matrix calculations, differentials, integrals and a lot more.
- Let's group the functions that fall under the same category into classes. So if someone want to work on an addition function, the person doesn't have to go through the whole code base, they just have to find the `arithmetic` class.
- Do the same classification for the rest of the functions.
- Still, everything is in one place. We can break the classes into different files. This way we can share the tasks in the team where individual developers can work with different parts of the code without tampering with the main program.
- If we decide to expand the calculator more, the relationships keeps expanding. What we can do is to group the class files under a common folder name that reflects the type of mathematical operations in there.
- With this put in place, we can write a separate code for the user interface and build a bridge for our logical part of the program to speak with the user interface.

Wow, that was organic and a mouthful.

If you're familiar with some of the concepts in software development, you will realise that these are seen in my thought process:

- Modularity
- Object Oriented Programming
- Abstraction
- Separation of concerns

{{< notice info >}}
Can you identify more concepts in the example above?
{{< /notice >}}

## How It Proves Useful

From the example above, we gave high-level descriptions of how we want to solve the problem of building a calculator. With the skill of abstract thinking, we looked at the problem on a larger scale than just writing code. We focused on why we needed to make certain decisions and how that will influence our programming style.


With our thought processes clearly laid out, we can leverage our problem-solving skills to break down complex independent problems into simpler ones to solve. Realise that writing code is the last thing to be done.


One of the many challenges I see beginners face is the temptation to write code before thinking about a solution. Trying to think of a solution while writing code simultaneously diverges the mind. In most instances, the person gets stuck. Here's my advice: Lay out an algorithm to solve the problem before writing code -- It will save you a lot of time and your program a lot of bugs.

## Conclusion

There is more to problem-solving and abstract thinking than what is described in this article. Remember that these skills can be learnt and mastered through consistent practice.


There are more skills and other types of thinking that will guide you on your software development journey. Such skills include convergent thinking, divergent thinking, critical thinking, creative thinking, testing, data structures and algorithms, etc.


Building your problem-solving and abstract thinking skills is a good place to start.

{{< quote-center >}}
*Knowledge is of no value unless you put it into practice.* -- **Anton Chekhov**
{{< /quote-center >}}
