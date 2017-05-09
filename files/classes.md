# Classes

## C++
### Defining
In C++ we define a class as follows:

    class foo
    {
      public:
        int someInt; // Public integer variable
	foo(int x = 0) // Constructor, defaults x to be zero if no X provided
        {
            someInt = x;
        }

        void SetSomeOtherInt(int x) // Allows modifying the private variable
        {
            _someOtherInt = x;
        }
    
      private:
        int _someOtherInt; // Private variable
    };

### Creating new instances
Using the above class:

    foo newInstance = new foo(1337); // Creates new foo instance and sets someInt to 1337 during construction.
 
### Constructing/initializing
When instantiating a class, you can send parameters as above to call a matching constructor, or nothing which calls the default constructor. The default constructor lets you create an instance and leave it uninitialized.

### Destructing/de-initializing
An optional destructor can be specified by prepending the constructor with '~', like so:

    ~foo()
    {
        delete[] somePtr;
    }

This will automatically call the defined destructor before the program exits normally, so it's useful for de-allocating memory and freeing shared resources, if you use them. AKA manual garbage collection.

## Python
### Defining
In Python, a class is defined as follows:

    class foo
        'Optional class documentation string'
        number1 = 0
        name = 'Ezekiel'
        def __init__(self, name, number1):
            self.name = name
            self.number1 = number1 + 1

### Creating new instances
Using the above class:

    myFoo = foo('Andrew', 34) # Creates an instance of foo

### Constructing/initializing
Constructing a class in Python is similar to C++, except instead of the constructor being named the same as the class, it is named __init__. A peculiarity of functions within a class, including the constructor, is that their first argument must be 'self', but you do not need to call 'self' when you use a function, it is added for you. In a way, this is more complicated than C++.

### Destructing/de-initializing
Python fully supports garbage collection, so destructing is handled automatically by the interpreter. There is no need to manually free memory space.

