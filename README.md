PRINTING PATTERN:
 

****

  ****

    ****

      ****

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM
Take the number of rows as input from the user (length of side of rhombus) and store it in any variable.(‘l‘ in this case).
Run a loop ‘l’ number of times to iterate through each of the rows. From i=0 to i<l. The loop should be structured as for( i=0 ; i<l : i++).
 Run a nested loop inside the main loop to print the spaces before the rhombus. From j=0 to j<i. The loop should be structured as for( j=0; j<i ; j++).
Run another nested loop inside the main loop after the previous loop to print the stars in each column of a row. From j=0 to j<l. The loop should be structured as for( j=0 ; j<l ; j++).
Move to the next line by printing a new line . printf(“/n”).
Code in C:
#include<stdio.h>
int main()
{
int i,j,l; //declaring integer variables i,j for loops and l for number of rows/columns
printf("enter number of rows/columns\n"); //asking the user for input
scanf("%d",&l); //taking input from the user
for(i=0;i<l;i++) //loop controlling number of rows
   {
      for(j=0;j<i;j++) //inner loop for spaces
         {
            printf(" ");
         }
      for(j=0;j<l;j++) //inner loop for printing the stars in each column of a row
         {
            printf("*");
         }
      printf("\n"); // printing a new line after each row
   }
}
TAKING INPUT:
 DISPLAYING OUTPUT:
