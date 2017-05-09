# Memory Management

## C++
### How is it handled?
C++ gives you the freedom to manage memory automatically or manually. Since C++ supports passing objects by reference, unlike C, it's possible to write entire programs without ever needing to manually allocate and de-allocate memory.

### How does it work?
When creating a variable, array, class instance, etc., they are automatically accumulated and set to be free'd on program exit, or when no longer needed.
Alternatively, you can manually allocate space in memory for any type being used in C++. This will force an object to stay in memory until it is explicitly de-allocated by the programmer. Failure to de-allocate before the program exits results in a memory leak. The nice thing about classes in C++, is it allows you to use manual allocation, and write de-allocation code in a destructor method, which is automatically called on program exit. So, in a way, there is a blend of auto and manual memory management. Some would say this is the perfect balance, and the main reason I prefer C++ over more modern languages such as C# and Swift.


## Python
### How is it handled?
Python on the other hand, does not believe in manual memory management at all. Absolutely every object used in a Python program is subject to garbage collection when it is no longer needed. Since python programs are typically much more simple than their C++ counterparts this works, most of the time.

### How does it work?
I honestly have no idea, it just does. :)

