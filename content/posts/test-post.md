---
title: "Test Post"
date: 2022-12-26T22:14:58Z
draft: true
slug: test
toc: true
categories:
    - "mentee or client"
summary: Testing how the post looks like.
tags:
    - intro
---

# Arrays & Slices

## Arrays

### Syntax

```go
variable := [size_of_array]data_type{initialise_values**}
```

E.g.

```go
grades := [3]int{98, 99, 97}
```

- An array can only store one type of data.
- Data type of an array must be specified when defining an array.

If you are going to initialise values in when declaring an array, you do not need to explicitly state the size; you can use the following syntax example:

```go
grades := [...]int{98, 99, 87, 85, 86}
```

### Assignment

```go
array_name[index] = value
```

### Note

- The length of the array is found using the `len` function.

Copying arrays in Go will create an entirely new set of arrays. (This could potentially slow down your program).

```go
a := [...]int{1, 2, 3}
b := a
```

The value, `b` is assigned a copy of the value, `a`. The way to deal with this behaviour is to make use of pointers.

```go
b := &a
```

What this does is to point to the address of `a`. `a` and `b` now points to the same data.

## Slices

### Syntax

```go
var slice_name = []data_type{initialise_values**}
```

- Slices do not have a fixed length like arrays.
- Slices are referenced data types. This means assigning a slice to a variable will point to the same memory address.

### Using `make()` To Create Slices

```go
var slice_name = make(slice_obj, length, capacity)

# Example

nums := make([]int, 2, 15)
```

### Adding Elements To A Slice

```go
slice_name = append(slice_name, values**)

// e.g.
a = append(a, 1, 2, 3, 4, 5)
```

### Appending Slices (Spreading)

```go
slice = append(slice, slice...)

// e.g.
a = append(a, []int{2, 3, 4, 5}...)
```
