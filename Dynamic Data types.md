# Dynamic Data

The data types that changes dynamically during runtime of program and is decided by computer is called Dynamic Data type.

Following are the methods to perform Dynamic data typing :

# void* :

This basically creates a pointer of any data type. Inorder to use it , we use ```static_cast``` keyword. Some syntax and examples are below : 

### Syntax 
```
void* name = address of a variable ;

```
## Disadvantages 

<p> One disadvantage of void pointers is that they discard type safety. It's easy to make mistakes when casting them, leading to undefined behavior and potential crashes. Void pointers also require manual type checking and casting, which can make the code less readable and more prone to errors </p>


### Examples 

```cpp
int me = 8;
float Drago = 8.14;
void* you;
you = &me;

cout << *(static_cast<int*> (you)) ; // 8
you = &Drago;
cout << *(static_cast<float*> (you)) ; // 8.14
```

### Note 
```
The changed data type can only beused before changing it to another data type.
Like if  you = &Drago was put after ```you = &me``` then logical error would have occured.
```

# std::any 
To use this , we need to include <any> header file . 
This does the sasme thing as void*.
std::any is a combination of void* , type discrimination, value-semantics, and object management. It is a far more complex structure than a simple void* . It would be an overstatement to say that std::any is a replacement of void* in all situations.

### Examples 
```cpp
 std::any any_value;

    any_value = 42;
    std::cout << "int value: " << std::any_cast<int>(any_value) << std::endl;

    any_value = 3.14;
    std::cout << "double value: " << std::any_cast<double>(any_value) << std::endl;

    any_value = std::string("Hello, world!");
    std::cout << "string value: " << std::any_cast<std::string>(any_value) << std::endl;

```

## Benefits 

The class any describes a type-safe container for single values of any copy constructible type
1) An object of class any stores an instance of any type that satisfies the constructor requirements or is empty, and this is referred to as the state of the class any object.
