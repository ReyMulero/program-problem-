# program-problem-
need help getting the first letteer capitalized it not working right

#include <stdio.h>
#include <stdlib.h>
#include <string.h>
void uppername( char upperName[])
{
    int len = strlen( upperName);
    int i;
    for(i=0; i<len;i++)
    {
        upperName[i]= toupper(upperName[i]);
    }
    printf("upper case name is %s \n", upperName);

}

void makeMeLower( char lowerName[])
{
    int len = strlen( lowerName);
    int i;
    for(i=0; i<len;i++)
    {
        lowerName[i]= tolower(lowerName[i]);
    }
    printf("lower name is:%s\n",lowerName);
}

void original(char name[])
{
    printf("original name is:%s\n",name);
}
void firstLetter(char initialCappedName[])
{
    initialCappedName[0]=toupper(initialCappedName[0]);
    printf("initial caped name %s \n",initialCappedName);
}


int main()
{
    char f[20];
    printf("please enter your first name: ");
    scanf("%s", f );

    original(f);
    makeMeLower(f);
    uppername(f);
    firstLetter(f);


     return 0;
}
