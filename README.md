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

### ODR

This is Simple Every Class, function , identifier should be defined only once.





<h1 style="text-align:center;">Found any Error <a href="#" style="text-align:center;">Report Here</a>!</h1> 