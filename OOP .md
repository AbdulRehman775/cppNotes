# OOP

<p> Object Oriented Principle is abasically a type of technique to make your code more modular and more readable than before. Though one should try to use functions more than OOP principle. Using OOP in every situation is a bad practice. </p>

In C++ programming language , there are following concepts of OOP : 

1) Classes
2) Inheritance
3) Polymorphism (Function overloading)
4) Function Overriding
5) Abstraction
6) Encapsulation

# Class

Class is basically a user defined Data type in C++ . It is defined by the user like what purpose does this data type server ? 
Class is basically like a structure where function and variables are stores as a property of that class and inside other functions we can 
make objects and give them the ```data type``` of  that class

Once an object with that data type has been created then that object can use all the properties and functions of that class. 

To  define  a class you can use the keyword ```class```. 
For example , 
```cpp
#include <iostream>

class MyNAme {
int me = 5;
public :
void print () {
 std::cout << "Hello Mom!";
}
};
int main(){
MyNAme Person ;
Person.print(); // Hello Mom!
retunr 0;
}
```
The integer me has the scope of private. 
In a class , if we don't specify the code with public keyword then that code falls into private  scope. 
This is part of ```Encapsulation``` 
Encapsulation is basically giving your code a title from  a hierarchy.
There are three titles : 
1) private
2) public
3) protected

Here if we don't write public in the baove code then that function will fall into private zone so what this means is that when an instance of that class is created then we can't access the private variables or functions.

The protected access modifier is relevant in cases where classes form an inheritance hierarchy. If an element (function, data member) with the protected access modifier is declared in a class, then the following rules apply to it:

 •  A class element is not accessible from any external method if this method is not friendly
 
 •  The class element is accessible from the internal methods of the class 
 
 •  It should be noted here that a protected-element of a class is also accessible from an instance of a class, if this instance is declared in an internal method of the class;

 •  The element of the class is accessible from the friendly functions of the class 
 
 •  A class element is accessible from methods of a friendly class

 •  The class element is accessible from the methods of the inherited class 
 
 •  This rule does not apply to “friendly” methods and methods of “friendly” classes


 
