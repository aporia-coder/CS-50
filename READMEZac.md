Lecture One

bit - binary digit is the origin of the term bit
bit is a zero and one
bit is similary to a lightbulb being off as 0 and on as 1
byte is 8 bits - maximum is 265 - 3byes - 24bits
transistors represent this binarary switch
base2 - binary
base10 - decimal
unicode is the solution to ascii, add more bits 
32 bits is over a billion characters

Lecture Two
make also compiles
clang is a comiler
clang creates files in c -- clang -o hello hello.c
compiles a file called hello from the hello.c file
make compiles without needing arguments (is used globally throughout other C languages)
the -o flag

when you compile code multiple steps happen

preprocessing - copy pastes anything with a hash (imports)
compiling 
assembling - converts code to assembly language
linking

THESE ARE IMPORTS, NECESSARY FOR THE LINKING STAGE IN COMPILING, initialized before anything else happens
#include <cs50.h>
#incldue <stdio.h>

string get_string(string prompt); FUNCTION DEF FROM CS50
^^ THIS IS CALLED A FUNCTION PROTOTYPE

int printf(string )

int main(void)
{
    string name = get_string("What's your name? ");
    printf("hello, %s\n", name)
}

%s references the variable name

clang -0 hello hello.c -lcs50 '-'-L FLAG INCLUDES THE LIBRARY DURING COMPILATION

