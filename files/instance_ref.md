#Instance reference name in data type (class)

## C++
Within a class, it is sometimes necessary to reference a variable owned by the class, that shares the same name as a variable in a subclass or function. To avoid a namespace collision, there is an operator that allows you to reference the containing classes namespace from a subclass or class function (method).
Example:

    class foo {
        int x;
        foo(int x) {
            this.x = x; // Collision avoided!
        }
    }

## Python
In Python, the first object of every function within a class automatically contains a reference to the containing class, usually called 'self'. The interpreter is smart enough to use the self object when a conflict occurs, so the programmer doesn't have to do anything special. Automatically is a running theme with Python.
