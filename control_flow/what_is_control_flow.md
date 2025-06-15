When a program is run, the CPU begins execution at the top of main(), executes some number of statements
(in sequential order by default), and then the program terminates at the end of main(). 
The specific sequence of statements that the CPU executes is called the program’s execution path (or path, for short).


//example code
#include <iostream>

int main()
{
    std::cout << "Enter an integer: ";

    int x {};
    std::cin >> x;

    std::cout << "You entered " << x << '\n';

    return 0;
};

The execution path of this program includes lines 5, 7, 8, 10, and 12, in that order. 
This is an example of a straight-line program. Straight-line programs take the same path 
(execute the same statements in the same order) every time they are run.

However, often this is not what we desire. For example, if we ask the user for input, 
and the user enters something invalid, ideally we’d like to ask the user to make another choice. 
This is not possible in a straight-line program. In fact, the user may repeatedly enter invalid input, 
so the number of times we might need to ask them to make another selection isn’t knowable until runtime.
