# Comparisons of references and values

## C++
### How are values compared? (i.e. comparing two strings)
When comparing values in C++, the method to do so varies depending on the type. String's contain a method which compares them by value. For example:

    std::string str1 ("green apple");
    std::string str2 ("red apple");
    if (str1.compare(str2) != 0)
        std::cout << str1 << " is not " << str2 << '\n';

Most other types have their comparison methods setup as an operator overload. If we were to define a custom string class, we could also define the '=' operator to do the above comparison whenever 'str1 == str2' was performed. This is a very handy and powerful feature of C++.

## Python
### How are values compared?
Python on the other hand, simply uses the normal <=, ==, >=, != operators to function on strings. Since we don't have the ability to create allocated strings in weird ways, it is always able to directly compare the values of the contents of a string, since they are always created the same way. No overloading is necessary! The same holds true for all primitive types in Python.
