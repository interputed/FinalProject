# Name spaces

## C++
### How are name spaces implemented?
Name spaces in C++ are used to organize code into logical groups and to prevent name collisions. Creating a namespace is as follows:

    namespace foo
    {
        int bar = 0;
    }

### How are name spaces used?
To use the namespace above, anything defined within the namespace simply prepends the namespace name, followed by two full-colons, then the object name, like so:

    int newBar = foo::bar; // Assigning to the namespace defined above.

Alternatively, you can use the using directive to tell an entire block of code to reference named items in the chosen name space:

    using namespace foo;
    int newBar = bar; // No foo:: required!

## Python
### How are name spaces implemented?
Automatically! Name spaces in Python are not determined by the programmer, but set by the interpreter automatically at runtime to avoid naming conflicts. The automatically made namespaces can have lifetimes of varying scope depending on how it is used. More simply, you don't get to declare it so don't worry about it.

### How are name spaces used?
They are used automatically when there is a naming conflict. Example:

    foo = 'Hello'
    def func():
        foo = 'Goodbye'
        print(foo) # This will print Goodbye
    
    print(foo) # However, this will print Hello!

