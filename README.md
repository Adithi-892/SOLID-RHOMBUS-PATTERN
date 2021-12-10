# SOLID-RHOMBUS-PATTERN
Write a program to display the following pattern

#include<stdio.h>
int main()
{
 int num,r,c,sp;
 printf("Enter number of rows : ");
 scanf("%d",&num);
 for(r=1; r<=num; r++)
 {
   for(sp=num-r; sp>=1; sp--)
       printf(" ");
   for(c=1; c<=r; c++)
       printf("%d",c);
   for(c=r-1; c>=1; c--)
       printf("%d",c);
   printf("\n");
 }
 for(r=1; r<=num; r++)
 {
   for(sp=r; sp>=1; sp--)
       printf(" ");
   for(c=1; c<=(num-r); c++)
       printf("%d",c);
   for(c=num-r-1; c>=1; c--)
       printf("%d",c);
   printf("\n");
 }
 return 0;
}

======================================================================

OUTPUT

-----------------------

Enter number of rows : 4
   1
  121
 12321
1234321
 12321
  121
   1
