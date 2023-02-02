Lecture One

unary uses a single input to solve a problem, base 1
bit - binary digit is the origin of the term bit
bit is a zero and one - base 2
bit is similar to a lightbulb being off as 0 and on as 1
transistors represent this binary switch
byte is 8 bits - maximum is 255 - 256 including 0 - 3bytes - 24bits
this is why rgb values go up to 255- maximum amount of numbers in a byte

BASE - 128 64 32 16 8 4 2 1  
BYTE - 0 0 0 0 0 0 0 0

using 8 bits you represent the letter A as 65
this is represented as

01000001

ASCII - American standard code for information interchange, a method of using bytes to represent the alphabet
UNICODE - numbers to letters to capture all different types of languages using binary, non-english letters emojis etc
emojis use the same binary numbers to unicode, but different fonts analagous to representing the different images
base2 - binary
base10 - decimal
unicode is the solution to ascii, add more bits
32 bits is over a billion characters
python and other languages use C under the hood
computational thinking relates to other fields such as the arts

Lecture Two

make also compiles
clang is a comiler
clang creates files in c -- clang -o hello hello.c
compiles a file called hello from the hello.c file
make compiles without needing arguments (is used globally throughout other C languages)
the -o flag

when you compile code multiple steps happen

preprocessing - copy pastes anything with a hash (imports) even code from imports that arent used
compiling - code to assembly
assembling - converts assembly to binary
linking - takes binary from local code and links it with binary from imports

THESE ARE IMPORTS, NECESSARY FOR THE LINKING STAGE IN COMPILING, initialized before anything else happens
#include <cs50.h>
#incldue <stdio.h>

string get_string(string prompt); FUNCTION DEF FROM CS50
^^ THIS IS CALLED A FUNCTION PROTOTYPE

int printf(string )

int main(void)
{
string name = get_string("What's your name? ");
printf("hello, %s\n", name)git
}

%s references the variable name

clang -o hello hello.c -lcs50 '-'-L FLAG INCLUDES THE LIBRARY DURING COMPILATION

Python compiles to C

decompiling goes from binary backwards.
DOWNSIDES - variable names are not contained, the logic is but the computer only needs to understand things in binary
DOWNSIDES - a while loop and a for loop could look exactly the same
clicking the red dot on the left side of vscode tells the compiler to step through the code line by line until you get to the debugger (red dot)
it pauses execution
