# Functions

Functions are basically independent block of code. You can use it anytime you want. To call it inside a function We write it's name and pass down the real arguments to it. 
To define a function in C++ we use 

```cpp
int Name() {
//Body of function 
}
```

There are two types of function. Normal function and Lambda functions.
# Lambda

This is an anonymous Function used anonymously.
Its syntax is like this
```cpp
[capture list of arguments] (parameters) -> return_type {
};

// or

auto me = [](){};
cout << me ;

```
where we put surrounding variables in the capture list .

These lambda functions improve readabilty of code and are useful for functional programming.

# Pointers

So pointers are basically objects that point to the variable stored in RAM. They contain the addresss of variable. These Pointers have their own memory in RAM.

There are two types of Pointers. 
Raw type and Smart Pointers.

Raw Pointers are what we use regularly.
While smart pointers are basically pointers with a set of functions listed onto them so that memory management is improved.

```cpp
using namespace std;
int yo = 5;
int* hey = &yo;
cout << *(hey); // 5
```
# Memory Management

There are various memory models in C++ :
1) Heap
2) Stack
3) Code Segment
4) Data Segment

# Heap 

This is a type of memory model that stores stuff that have been declared with (new)  keyword. 
```cpp
int* hey = new int;
```

# Stack 
This stores stuff in LIFO order.


# Code Segments 

This is the type of memory model that stores Machine Code.

# Data segment

This is the type of memory model that stores Source code. 
It has two types.


