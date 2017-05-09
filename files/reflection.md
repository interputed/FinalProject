# Reflection

## C++
C++ does not support any reflection abilities.

## Python
Python has many reflection-enabling functions, such as, type(), isinstance(), callable(), dir(), and getattr().
Reflection Example:

    # without reflection
    obj = Foo()
    obj.hello()

    # with reflection
    class_name = "Foo"
    method = "hello"
    obj = globals()[class_name]()
    getattr(obj, method)()

    # with eval
    eval("Foo().hello()")

(Credit: https://en.wikipedia.org/wiki/Reflection_%28computer_programming%29)
































(I don't know anything about reflection)
