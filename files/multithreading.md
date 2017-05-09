# Multithreading

## C++
This is perhaps the holy grail of C++ topics. C++ can be used for parallel code in pretty much any way which can be imagined. Want to spawn a bunch of processes handled by the OS scheduler and communicating via shared objects? Check. Want to create a massive thread pool of divided chunks of work and have each processor core work on as many of them as it can? Check. Want to setup several separate machines to process the same data and communicate over a network? Check. There is essentially no limit to the multithread capabilities of C++. None of them are particularly easy to write an example for, however. 

## Python
Multithreading in Python is very easy to do, with one big limitation in comparison to C++, threads created in a Python program all share the same memory space. In C++ you can accomplish anything you desire, where Python threads are comparable only to the C++ standard library threads, which spawn light-weight side jobs that can be used for parallel processing a small in-program task, while not actually being a separate process at the OS level. This works well enough for most tasks, but for very large workloads C++ is the better choice.

