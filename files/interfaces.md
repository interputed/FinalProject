# Interfaces / Protocols

## C++

### What does the language support?
C++ does not directly support interfaces. However, any class that contains a virtual method becomes an abstract class. The virtual methods must be implemented for the class to be usable, so the class functionally becomes the same as an interface.

### What abilities does it have?
A C++ abstract class is basically the same as an interface as we know it from Java. Any class can be declared as virtual and have only a return type and parameter list definition, but not an actual implementation, so potentially anything can be done with this class. It lacks the restrictions of a Java interface, you can inherit as many interfaces as you want for example.

### How is it used?
To use a abstract class you must create a class that implements it, and defines all of its virtual methods before it can be used.
Example:
    
    class foo {
        virtual int getVal();
    };

    class bar : foo { // Implements foo, so must define getVal
        int getVal() { // Since defined, can use this class now.
            return 0;
        }
    };


## Python

### What does the language support?
While Python does have the technical ability of writing abstract classes, it supports multiple-inheritance and duck typing, there is no need to use interfaces at all.
