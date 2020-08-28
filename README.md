# C++ Reference

This Document is served as a Compilation of cppreference in my words. This doc does not represents any completion but are points that i thinks mostly used.

[TOC]

# Comments

There are Two Type of comments

1. Single Line comment

   ```c++
   // This is Comment
   ```

2. Multi Line Comment

   ```c++
   /**
    * This is Comment
    */
   
   ```

# Names - Identifiers

A Name of Identifiers should Begin with Small or Capital Letter or Underscore followed by any alphabet or Number. All Identifiers with Underscore are reserved by compiler.

# Types 

coming soon....

# Fundamental Types

| Type           | alias                                 | Description                                    |
| -------------- | ------------------------------------- | ---------------------------------------------- |
| void           |                                       | Type for Function that Does not Return Anyting |
| std::nullptr_t | `typedef decltype(nullptr) nullptr_t` | Null Pointer                                   |
| bool           |                                       | Boolean                                        |
| int            |                                       | Integer                                        |
| char           |                                       | Character                                      |
| wchar_t        |                                       | Wide Character                                 |
| char16_t       |                                       | UTF-16 Characters                              |
| char32_t       |                                       | UTF-32 Characters                              |
| char8_t        |                                       | UTF-8 Characters                               |
| float          |                                       | Floating Point Numbers                         |
| double         |                                       | Double Precision Numbers                       |



# Definition and ODR

Definition is anything that defines what the declaration is going to do. 

```c++
// Example
int i; // Declaration
i = 32 // Defination what is i
int add(int, int); // Declaration
int add (int a, int a) { // Defination
    return a + b;
}
```

## ODR

This is Simple Every Class, function , identifier should be defined only once.

# Name Lookup

Name lookup is a process when program searches for name of variable under his scope.

There are two kind of lookup

1. Qualified 
2. Unqualified

more coming soon....



# Statements

There are Following Statements

1. if
2. switch
3. while
4. do..while
5. for
6. ranged for
7. continue
8. break
9. goto
10. return

## if

if statement contains two kinds of statement

1. if
2. if.. else

if statement is a conditional statement with controls which statement of program should next be executed. if condition is false else in below program is executed

```c++
if(condition) {
    // if condition is true
} else {
    // if condition is false
}
```

During compilation you can discard the  else statement using `constexpr if statement`

```c++
if constexpr (condition) {
    // if condition is true
}else {
    // if condition is false
}
```

in Above clause if condition is true else part is discarded and vice-versa

## switch

The switch syntax is as follows

```c++
switch(value) {
    case match-1:{
        // if value == match-1
        break;
    }
    case match-2:{
        // if value == match-2
    }
    default:{
        // default if no matched
    }
}
```

## for

for statement is used to loop arrays

```c++
for(initialization; condition; expression) {
    // code block
}
```

Below is Example

```c++
for(int i = 0; i< 10; i++) {
    std::cout<< i << std::endl;
}
//
// 1
// 2
// .
// .
// 9
```

## Ranged for

Ranged for Loop is a addition to c++ in c++11. it is used to iterate over elements. Since programmer don't have to keep track of array bounding program is safer than regular for loop

```c++
int nums[] = {1,2,3,4,5}
for(int item: num) {
    // process item
}
```



## while

While statement is similar to regular for loop statement.

```c++
init statement
while(condition) {
  	...
    increment
}
```



```c++
int i = 0;
while(i < 10) {
    // Code goes here
    i++;
}
```



## do..while

Do while statement is used in condition in which you want to iterate first time any equation but wanted to iterate further if certain conditions met.

```c++
do {
    // code
}while(condition)
```



Example

```c++
do {
    int i = 0;
    i++;
}while(i < 10)
```



## break, continue, goto, return

Break is used to break out of loop , goto i used to goto any label in program , continue is used to skip current iteration of loop and return is used to return value from function

# Classes

Class is might be the selling factor of c++. Before Knowing Anything about Classes you Should be Familiar with OOP Concepts

## 

# Union

Coming soon....













<h1 style="text-align:center;">Found any Error <a href="#" style="text-align:center;">Report Here</a>!</h1> 