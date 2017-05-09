# Lambda Expressions

## C++
C++ has lambda support, which is better thought of as an unnamed, inline function. I guess it's easier to say "lambda", though I always found the name a bit ridiculous. Basically, anywhere where a value needs to be computed for assignment to something, you can use a lambda to do something more advanced, without having to write a separate function. This can be useful for small cases such as comparison operators in custom classes.
Example: 

    std::sort(x, x + n, /* 2nd Parameter is the lambda below */
        [](float a, float b) {  // Lambda expression begins  
            return (std::abs(a) < std::abs(b));  
        } 
    );  // end of std::sort parameter list

The first line of this example is calling the std::sort() function, which takes 3 parameters, the 3rd parameter is a custom comparator function. Rather than write a function for something so simple, we can simply write a lambda inline, which functions the same.
The 2nd line starts the lambda, sets up its parameter list which can be empty, and the 3rd line returns the result of a comparison between the 2 parameters. It takes some getting use to, but once you see what it's doing the syntax is a little more friendly.


## Python
If nothing has sold you on Python being easier so far, prepare for it to happen with lambda's! Creating a lambda in Python makes the C++ version look like a troll job.
Example:

foo = lambda x, y : x < y

That's it! We are creating a variable named foo and assigning to it the value of true or false depending on if x < y. It should be immediately clear to everyone that the comma separated x and y values are the parameter list, and after the semi-colon is the function logic to be returned. Someone could probably figure this out without even knowing what a lambda is. Another win for Python!
