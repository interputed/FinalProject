# Null/Nil References

## C++
Having a way to assign a pointer variable to point at nothing is often useful in C++. To do so, we use the pre-defined constant 'nullptr'. This points to a memory address pre-defined as nothing. This should almost always be memory address 0x00000000. The value stored at this pointer should always be 0, or NULL. So, you can initialize objects to NULL, and object pointers to nullptr.

## Python
As if it comes as any surprise, Python handles this in an easier way. Rather than have '0', and 'NULL', and 'nullptr' there is just a single value that works for all types that have not been set to any value, and that is 'None'. For example:

    if yourVar is None:
        ... # do stuff

This assignment is making me like Python more than I did!