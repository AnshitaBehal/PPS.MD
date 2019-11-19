![College  Logo](https://www.gndec.ac.in/logo.png)

# **Programming for Problem Solving**
## **Name:- Anshita Behal**
## **CRN:-1921012**
## **Branch:- IT-A1**
---

### 1) To print name.
```C
      /* Program to print your name */

#include<stdio.h>
int main() {

puts("**************");
puts("anshita behal");
puts("**************");

return 0;
}
```
### 2) To print College address.
```C
        /* College Address */
 
#include<stdio.h>
int main() {

printf("\n\t\t\tGuru Nanak Dev Engineering College,");
printf("\n\t\t\tGill Road,");
printf("\n\t\t\tLudhiana , Punjab");

return 0;
}
```
### 3) Program to add two integers.
```C
     /* To add two integers */

#include <stdio.h>
int main() {
    
int a,b;

printf("\nEnter the numbers....");

printf("\nA:");
scanf("%d",&a);

printf("\nB:");
scanf("%d",&b);

a=a+b;

printf("\n Sum of the number is %d ",a);

return 0;

}
```
### 4) Program to find quotient and remainder.
```C
    /* To find quotient and remainder */

#include <stdio.h>

int main() {
    
int a,b,r,q;

printf("\nEnter the Dividend:");
scanf("%d",&a);

printf("\nEnter the divisor:");
scanf("%d",&b);

r=a%b;
q=a/b;

printf("\nRemainder: %d",r);
printf("\nQuotient: %d",q);

return 0;
}
```

### 5) Program to check even odd number.
```C
/* To find whether number is even or odd */

#include<stdio.h>
int main() { 

  int num,temp;

  printf("Enter the Number:");
  scanf("%d",&num);

  if(num%2==0)
  printf("\nNumber is Even....");

  else
  printf("\nNumber is Odd....");

  printf("\n\n");
  return 0;
}
```
### 6) Finding greteast of two numbers.
```C
     /* Largest one in two */

#include<stdio.h>

int main() {
    int a,b;
    printf("Enter any two number(A and B): ");
    scanf("%d%d", &a, &b);
    
if(a>b)
printf("\nA is largest....");
else
        printf("\nB is largest.....");
    
return 0;
}
```
### 7) Find greatest of three number .
```
/* Largest of three number */

#include<stdio.h>
int main() {
int x, y, z, large;
        
 printf(" Enter any three integer numbers for x, y, z :  ") ;

scanf("%d %d %d", &x, &y, &z) ;

large = (x > y ? ( x > z ? x : z) : (y > z ? y : z)) ;

printf("\n\n Largest  or biggest or greatest or maximum among 3 numbers using Conditional ternary Operator :  %d", large) ;
       
 return 0;
}
```
### 8) Program to assign grade to student according to percentage.
```C
/* To find grade of a student by marks */

#include<stdio.h>
int main() { 
    
  int s1,s2,s3,s4,s5,agg;
  float perc;

  printf("Enter the Marks in 5 Subjects Respectively:\n");

scanf("%d%d%d%d%d",&s1,&s2,&s3,&s4,&s5);

agg=s1+s2+s3+s4+s5; // Aggregate Marks
  
  perc=agg/500.0*100;  // Perc Marks

  if(perc>=90)
  {
      printf("\nA");
      
  }
  
  else if (perc>=80 && perc<90)
  { 
      printf("\nB");
      
  }
  
  else if(perc>=70 && perc<80)
  {
      printf("\nC");
      
  }
  
  else if(perc>=60 && perc<70)
  { 
      printf("\nD");
  }
  else if(perc>=50 && perc<60)
  {
      printf("\nE");
  }
  else 
     {
          printf("\nScope of Improvement....");
    } 
    return 0;
}
```

### 9) Program to check year is leap or not.
```C
/* To find whether year is leap or not */

#include<stdio.h>
int main() { 

  int year,temp;

  printf("Enter the year:");
  scanf("%d",&year);

  temp=year%4;

  if(year%100==0)
  {
     if(year%400==0)
     printf("\nLeap year...");
  }

  else
  {
    if(year%4==0)
    printf("\nLeap year...");

else
    printf("\nNot a Leap year...");
   }
  
  return 0;
}
```
### 10) Program to print table of 5.
```C
/* Table of 5 */

#include<stdio.h>

int main() { int res;

for(int i=1;i<=10;i++) {

res=5*i;
    
   printf("\n5*%d=%d",i,res);
   }

   return 0;
}
```
### 11) To make simple calculator using switch case.
```C
/* C Program to Create Simple Calculator using Switch Case */
 
#include <stdio.h>
 
int main() {
	char Operator;
	float num1, num2, result = 0;
	
printf("\n Please Enter an Operator (+, -, *, /)  :  ");
scanf("%c", &Operator);
  	
printf("\n Please Enter the Values for two Operands: num1 and num2  :  ");
scanf("%f%f", &num1, &num2);
  	
switch(Operator)
  	{
  		case '+':
  			result = num1 + num2;
  			break;
  		case '-':
  			result = num1 - num2;
  			break;
  		case '*':
  			result = num1 * num2;
  			break;
  		case '/':
  			result = num1 / num2;
  			break;
		default:
			printf("\n You have enetered an Invalid Operator ");				    			
	}
  
printf("\n The result of %.2f %c %.2f  = %.2f", num1, Operator, num2, result);
	
return 0;
}
```
### 12) To calculate reverse of a number.
```C
/* To find reverse of a Number*/

#include<stdio.h>
int main() { 

  int num,rev=0;

  printf("\nEnter the Number:");
  scanf("%ld",&num);

while(num!=0)
{ 
    rev = rev * 10;
    rev = rev + num%10;
    num = num/10;
  }
  

  printf("\nReversed number:%d",rev);

  printf("\n\n");
  return 0;
}
```

### 13) To check whether number is palindrome or not.
```C
 /* Palindrome of a number */

#include <stdio.h>
int main() {
    
     int n, reversedInteger = 0, remainder, originalInteger;
    printf("Enter an integer: ");
    scanf("%d", &n);
    originalInteger = n;
    // reversed integer is stored in variable 
    while( n!=0 )
    {
        remainder = n%10;
        reversedInteger = reversedInteger*10 + remainder;
        n /= 10;
    }
    // palindrome if orignalInteger and reversedInteger are equal
    if (originalInteger == reversedInteger)
        printf("%d is a palindrome.", originalInteger);
    else
        printf("%d is not a palindrome.", originalInteger);
    
    return 0;
}
```
### 14) To check whether a number is prime or not.
```C
/* Program to check prime no. */

#include <stdio.h>
#include <stdlib.h>
 
int main() {
    
   int num, j, flag;
  
  printf("Enter a number \n");
   scanf("%d", &num);
 
  if (num <= 1)
    {
        printf("%d is not a prime numbers \n", num);
        exit(1);
    }
    flag = 0;
    for (j = 2; j <= num / 2; j++)
    {
        if ((num % j) == 0)
        {
            flag = 1;
            break;
        }
    }
    if (flag == 0)
        printf("%d is a prime number \n", num);
     else
        printf("%d is not a prime number \n", num);

return 0;
    
}
```
### 15) Program to print prime number to 100.
```C
/* Prime number from 1 to 100 */
 
 #include<stdio.h>

   int main(){

int numbr,k,remark;

printf(" The prime numbers between 1 and 100 : \n");

   for(numbr=2;numbr<=100;++numbr)

  {

   remark=0;

  for(k=2;k<=numbr/2;k++){

  if((numbr % k) == 0){

 remark++;

  break;
     }

   }

   if(remark==0)
    printf("\n    %d ",numbr);

 }

  return 0;

   } 
 ``` 
### 16) Program to check whether a number is armstrong or not.
```C
/* To check armstrong number */

#include <stdio.h>
int main()
{
    int number, originalNumber, remainder, result = 0;

printf("Enter a three digit integer: ");
    scanf("%d", &number);

originalNumber = number;

while (originalNumber != 0)
    {
        remainder = originalNumber%10;
        result += remainder*remainder*remainder;
        originalNumber /= 10;

}

if(result == number)
        printf("%d is an Armstrong number.",number);
    else
        printf("%d is not an Armstrong number.",number);

return 0;
}

```
### 16) Print Different Patterns.
i) Pattern 1.
```C
#include <stdio.h>
int main() {
    
   int i,j,r;
    
   printf("Enter number of rows: ");
    scanf("%d",&r);
    
for(i=1; i<=r; ++i)
    {
        for(j=1; j<=i; ++j)
        {
            printf("%d ",j);
        }
        printf("\n");
    }
    return 0;
}

```
### ii) Pattern 2. 
```C
#include <stdio.h>
int main() {
    
   int r,i,j,num= 1;
   printf("Enter number of rows: ");
    scanf("%d",&r);
    for(i=1;i<=r;i++)
    {
        for(j=1;j<=i;++j)
        {
            printf("%d",num);
            ++num;
        }
        printf("\n");
    }
    return 0;
}
```
### 17) To find sum of the N natural numbers in an array.
```C
/* Sum of N no.s in array */
     
#include<stdio.h>

int main() {
    printf("\n\n\t\tStudytonight - Best place to learn\n\n\n");
    int n, sum = 0, c, array[100];

printf("Enter the number of integers you want to add: ");
    scanf("%d", &n);

 printf("\n\nEnter %d integers \n\n", n);

for(c = 0; c < n; c++)
   {
        scanf("%d", &array[c]);
        sum += array[c];    // same as sum = sum + array[c]
    }

  printf("\n\nSum = %d\n\n", sum);
    return 0;
}
```
### 18) Program to add two matrices .
```C
/*  Addition of matrix */
    
#include <stdio.h>
 
int main() {
   
   int m, n, c, d, first[10][10], second[10][10], sum[10][10];
 
   printf("Enter the number of rows and columns of matrix\n");
   scanf("%d%d", &m, &n);
   
   printf("Enter the elements of first matrix\n");
 
   for (c = 0; c < m; c++)
      for (d = 0; d < n; d++)
         scanf("%d", &first[c][d]);
 
   printf("Enter the elements of second matrix\n");
 
   for (c = 0; c < m; c++)
      for (d = 0 ; d < n; d++)
         scanf("%d", &second[c][d]);
   
   printf("Sum of entered matrices:-\n");
   
   for (c = 0; c < m; c++) {
      for (d = 0 ; d < n; d++) {
         sum[c][d] = first[c][d] + second[c][d];
         printf("%d\t", sum[c][d]);
      }
      printf("\n");
   }
 
   return 0;
}
```
### 19) Program to multiply two matrices .
```C
/* Multiplation of matrices */

#include <stdio.h>
int main()
     {
      int m, n, p, q, c, d, k, sum = 0;
      int first[10][10], second[10][10],   multiply[10][10];
 
  printf("Enter number of rows and columns of first matrix\n");
  scanf("%d%d", &m, &n);
  
  printf("Enter elements of first matrix\n");
 
  for (c = 0; c < m; c++)
    for (d = 0; d < n; d++)
      scanf("%d", &first[c][d]);
 
  printf("Enter number of rows and columns of second matrix\n");
  scanf("%d%d", &p, &q);
 
  if (n != p)
    printf("The matrices can't be multiplied with each other.\n");
  
  else
  {
    printf("Enter elements of second matrix\n");
 
for (c=0;c<p;c++)
      for (d = 0; d < q; d++)
        scanf("%d", &second[c][d]);
 
  for (c = 0; c < m; c++) {
      for (d = 0; d < q; d++) {
        for (k = 0; k < p; k++) {
          sum = sum + first[c][k]*second[k][d];
        }
 
   multiply[c][d] = sum;
        sum = 0;
      }
    }
 
   printf("Product of the matrices:\n");
 
   for (c = 0; c < m; c++) {
      for (d = 0; d < q; d++)
        printf("%d\t", multiply[c][d]);
 
   printf("\n");
    }
  }
 
  return 0;
}
```
   
### 20) Program to calculate factorial of a number with recursion.
```C
/* Recursion */

#include<stdio.h>
long int multiplyNumbers(int n);
int main() {
    
int n;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    printf("Factorial of %d = %ld", n, multiplyNumbers(n));
    return 0;
}
long int multiplyNumbers(int n)
{
    if (n >= 1)
        return n*multiplyNumbers(n-1);
    else
        return 1;
}
```

### 21) Program to calculate average of 5 numbers using function.
```C
 /* program to find average of 5 numbers  */
 
#include<stdio.h>
int avg(int,int,int,int,int);      // prototype
 
int main() { int a1,a2,a3,a4,a5,res;
   
   printf("\nEnter the numbers respectiively....");
   scanf("%d%d%d%d%d",&a1,&a2,&a3,&a4,&a5);
   
   res=avg(a1,a2,a3,a4,a5);     // function call
   printf("Average of the numbers %d",res);
   
   return 0; 
 }
 
 int avg(int a1,int a2,int a3,int a4,int a5)      // definition
 
 { int p; 
   p=(a1+a2+a3+a4+a5)/5;
   return p;
 }
 ```

### 22) Program to implement bubble sort.
```C
   /* Bubble sort implementation  */
 
#include <stdio.h>
 
int main()
{
  int array[100], n, c, d, swap;
 
  printf("Enter number of elements\n");
  scanf("%d", &n);
 
  printf("Enter %d integers\n", n);
 
  for (c = 0; c < n; c++)
    scanf("%d", &array[c]);
 
  for (c = 0 ; c < n - 1; c++)
  {
    for (d = 0 ; d < n - c - 1; d++)
    {
      if (array[d] > array[d+1]) /* For decreasing order use < */
      {
        swap       = array[d];
        array[d]   = array[d+1];
        array[d+1] = swap;
      }
    }
  }
 
  printf("Sorted list in ascending order:\n");
 
  for (c = 0; c < n; c++)
     printf("%d\n", array[c]);
 
  return 0;
}
```
### 23) Program to store information of 10 students using array of structures.
```C
/* Structures for student */

#include<stdio.h>
struct student
{
  char name[20],address[30];
  int grade,roll,dob;
};

int main()
{
  struct student s[10];
  int i;
  for(i=0;i<10;i++)
  {
    printf("\nEnter records for student[%d]\n",i+1);
    printf("Enter name: ");
    gets(s[i].name);
    printf("Enter address: ");
    gets(s[i].address);
    printf("Enter class, roll number and date of birth(year): ");
    scanf("%d%d%d",&s[i].grade,&s[i].roll,&s[i].dob);
  }
  printf("Records of the 10 students are here");
  for(i=0;i<10;i++)
  {
    printf("\nStudent %d",i+1);
    printf("\nName: %s",s[i].name);
    printf("\nAddress: %s",s[i].address);
    printf("\nClass: %d",s[i].grade);
    printf("\nRoll No.: %d",s[i].roll);
    printf("\nDOB: %d",s[i].dob);
    printf("\n");
  }
  return 0;
}
```
### 24) Program to print the address of variable using pointer.
```C
#include <stdio.h>
int main() {
  int a;
  int *pt;

  a = 10;
  pt = &a;

  printf("\n[&a ]:Address of A = %p", &a);


  return 0;
}
```
