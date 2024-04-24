Removing brackets from an algebraic expression
To remove brackets first we need to find them, so we will iterate the input string through a while loop and store it in the new character array if brackets are found we will not store them in the new array in this way as the end of the string is reached we have a new algebraic expression without brackets.

Remove Brackets From an Algebraic Expression Cpp program
Algorithm:
Initialize the variables and accept the input.
Initialize a while loop and terminate it at the end of string. 
Iterate each character of the string through that loop.
Store these characters into an new array skip brackets , if found.
Print result.
C++ programming code to remove brackets from an algebraic expression
Run
#include <iostream>
using namespace std;

int main()
{
//Initializing variables.
char str[100]="Prepins))ta", str_without_brackets[100];
int i=0, j=0 ;

//Iterating each character of string.
while(str[i] != '\0')
{
if(str[i] != '(' && str[i] != ')')//Removing brackets.
{
str_without_brackets[j++] = str[i];
}
i++;
}
str_without_brackets[j] = '\0';

//Printing result.
cout<<"The string after removing all the brackets is:\n"<<str_without_brackets;
return 0;
}
Output
The string after removing all the brackets is:
Prepinsta
Method 2
Here we are using the same concept as above but this is implemented using for loop.

Run
#include <iostream>
using namespace std;

int main()
{
//Initializing variables.
char str[100]="P(repi((nsta)", str_without_brackets[100];
int i=0, j=0 ;

//Iterating each character of string.
for(int i=0;str[i] != '\0';i++)
{
if(str[i] != '(' && str[i] != ')')//Removing brackets.
{
str_without_brackets[j++] = str[i];
}
}
str_without_brackets[j] = '\0';
//Printing result.
cout<<"The string after removing all the brackets is:\n"<<str_without_brackets;
return 0;
}
Output
The string after removing all the brackets is:
Prepinsta
