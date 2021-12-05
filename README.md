# primitive_operations_on_array
It includes insertion, deletion and traversal of an array

#include<stdio.h>

void main()

{

int i,A[10],n,j,pos,c;

printf("Enter the size of array : ");

scanf("%d",&n);

printf("Insertion");

printf("\nEnter the elements of array : \n");

for(i=0;i<n;i++)

scanf("%d",&A[i]);

printf("\nTraversing\n");

for(i=0;i<n;i++)

printf("%d ",A[i]);

printf("\nDo you want to delete any element ? (1 for yes and 2 for no) : ");

scanf("%d",&c);

switch(c)

{

case 1 : printf("Enter the position from where u want to delete : ");

scanf("%d",&pos);

if (pos >= n+1)

printf("Deletion not possible.\n");

else

{

for (j=pos-1;j<n-1;j++)

A[j] = A[j+1];

printf("Updated array : ");

for (j=0;j<n-1;j++)

printf("%d ", A[j]);

}

break;

case '2' : break;

default : printf("You entered a wrong choice");

}

}
