Removing spaces from a string.
In this article we will learn how to write a C program to remove spaces from a string. 

Here we will store the string in a character array lets say str and that original string will contain the spaces in between.

Example:- 
Input string: “Prep  insta”

Output string: “Prepinsta”

Remove all character from a string except alphabets in python
Algorithm:
Initialize the variables.
Accept the input.
Initialize while loop and terminate it at the end of string.
Iterate each character through the loop.
Exclude spaces.
Store the string without spaces.
Print result.

While loop in C
C programming code to remove spaces from a string
#include<stdio.h> 
using namespace std;
// Function to remove all spaces from a given string
void removeSpaces(char *str)
{
    // To keep track of non-space character count
    int count = 0;
    // Traverse the provided string. If the current character is not a space,
    //move it to index 'count++'.
    for (int i = 0; str[i]; i++)
        if (str[i] != ' ')
            str[count++] = str[i]; // here count is incremented
    str[count] = '\0';
}
// Driver program to test above function
int main()
{
    char str[] = "P re p i  n  sta ";
    removeSpaces(str);
    printf("%s", str);
    return 0;
}
Output
Prepinsta
