# Types

## C++
### What types does the language support?
* Character Types
    * char
    * char16_t
    * char32_t
    * wchar_t
* Integer Types (signed)
    * signed char
    * short
    * int
    * long
    * long long
* Integer Types (unsigned)
    * unsigned char
    * unsigned short
    * unsigned
    * unsigned long
    * unsigned long long
* Floating-point types
    * float
    * double
    * long double
* Boolean type
    * bool
* Void type
    * void
* Null pointer
    * decltype(nullptr)

### Are both reference and value types supported?
Yes, C++ is perhaps the best example of a language that supports both reference and value types. Any type can be created as an address pointing to that type(reference), or variable holding a value. The dereference operator is used to specify you wish to create a variable containing a memory address that points to a specific value type.

    int foo = 4; // Creates a variable holding the value 4
    int *bar = &foo; // Creates a pointer referencing the memory address to foo

### Can new value types be created?
Yes, in C++ it is very easy to define a custom type using the typedef operator.
Example:

    typedef unsigned char uchar; // Creates new type 'uchar' 
    uchar foo = 12; // Uses uchar variable


## Python
### What types does the language support?
Python has dynamic typing, which means it doesn't use strict built-in data types in a similar manner to how C++ does. Each variable stores the type of value along with the value and does not check to ensure appropriate things for the type are being done. The principal type the interpreter assigns each variable can be numeric types, sequences, sets and mappings.

### Are both reference and value types supported?
Python actually creates all type variables as references and does not support value-only types. Compounding the confusing, you cannot manually set a variable address. Every variable contains the type of value it is, and an address pointing to that value. There's no way to create a variable without the associated type and reference.

### Can new value types be created?
Sort of? Since you aren't declaring a variable to be a specific type in Python, you can essentially use a variable to contain whatever type of data you want, and it's type is saved along with it. There is no need to define a custom type in advance. Example:
    
    # This creates an array containing 3 different types with no need to pre-define
    foo = [1, 'Andrew', false]
   
 
