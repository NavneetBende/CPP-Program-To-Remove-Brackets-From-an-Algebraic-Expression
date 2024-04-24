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
