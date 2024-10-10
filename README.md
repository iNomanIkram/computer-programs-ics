# ICS-ComputerPrograms
List of questions provided along with the solution code for students of I.C.S Federal Board Specifically


Q6.Write a program that will print this message (chap2)
I Love Computers
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
printf("I Love Computers");
getch();
}
```
Q6.What will be printed by the following program?(chap3)
getch();
}
count=0;total=0
count=1;total=1
count=2;total=3
count=3;total=6
count=4;total=10
count=5;total=15
count=6;total=21
count=7;total=28
Q7.Write the above program using while loop?(chap 3)
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int count=0;
int total=0;
while(count<8)
{
total=total+count;
printf("\n count=%d,total=%d",count,total);
count++;
}
getch();
}
```
Q9.Write a program to find the sum of positive odd numbers and and the product of positive numbers less than or equal to 30?(chap 3)
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int sum,i,j;
long int prod;
prod=1;
for(i=0;i<30;i=i+2)
prod=prod * i;
sum=0;
for(j=1;j<30;j=j+2)
sum=sum+j;
printf("\nThe sum of odd number less than 30 is %d",sum);
printf("\nThe prod of even number less than 30 is %d",prod);
getch();
}
```
Q11.Write a program that prints the square of all the numbers from 1 to 10.(chap 3)
    Number                Square
     ---------                    ---------
         1                               1
         2                               4
         3                               9
         -                                -
       10                           100
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int n;
printf("\n\tNumber\tSquare");

for(n=1;n<10;n++)
printf("\n\t%d\t%d",n,n*n);
getch();
}
```
Q10.Write two programs that read an integer and print its table in descending order using using for loop and while loop?(chap 3)
FOR LOOP
```
# include<stdio.h>
# include<conio.h>
void main(void)
{
int i,n;
printf("Enter the number whose table is required\n");
scanf("%d",&n);
for(i=10;i>=1;i--)
printf("\n%2d x %2d = %3d",n,i,n*i);
getch();
}
```
WHILE LOOP
```
# include<stdio.h>
# include<conio.h>
void main(void)
{
int i,n;
i=10;
printf("Enter the number whose table is required\n");
scanf("%d",&n);
while(i>=1)
{
printf("\n%2d x %2d = %3d",n,i,n*i);
i--;
}
getch();
}
```
Q2.Write a program that reads temperature and prints a message as given below.(chap4)
                  Tempeature         Message
                     t>35                       it is hot!
                t>=20,t<=35             nice day!
                     t<20                      it is cold!
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int temp;
printf("enter temperature");
scanf("%d",&temp);
if(temp>35)
printf("its hot!");
else if(temp>=20 && temp <=35)
printf("its nice!");
else if(temp<20)
printf("its cold!");
else
printf("\n invalid temp");
getch();
}
```
Q4.Write a program that reads three numbers and prints the largest?(chap 4)
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int x,y,z;
printf("Enter three numbers\n");
scanf("%d %d %d",&x,&y,&z);
if(x>y&&x>z)
printf("x is largest \n",x);
else if (y>x && y>z)
printf("y is largest %d\n",y);
else
printf("z is largest %d \n",z);
getch();
}
```
Q5.A class of 35 students takes examination in which marks range from 0 to 100.Write a program which finds.
a)the average marks
b)the number of students failed(marks below 50)
c)the number of students who scored 100 marks
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int marks,i,fail,fullmarks,sum,avg;
sum=0;
fail=0;
fullmarks=0;
for(i=0;i<35;i++)
{
printf("ENTER MARKS=");
scanf("%d",&marks);
if(marks<50)
fail++;
else if(marks==100)
fullmarks++;
sum=sum+marks;
}
avg=sum/35;
printf("\navg is = %d",avg);
printf("\n no. of fail students are  =%d",fail);
printf("\nthe students who got full marks  =%d",fullmarks);
getch();
}
```
Q6.Write a program that prints all odd positive integer less than 100 skipping those that are exactly divisble by 7?(chap 4)
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int i;
for(i=1;i<100;i=i+2)
{
if(i%7!=0)
printf("\n%d",i);
}
getch();
}
```
Q5.Write a program thats reads n integer and prints the smallest along its subscript value in the list?(chap 5)
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int marks[10],i,min;
printf("enter the marks\n");
for(i=0;i<10;i++)
scanf("%d",&marks[i]);
min=marks[0];
for(i=0;i<10;i++)
if(min>marks[i])
min=marks[i];
printf("the min marks in array is %d",min);
for(i=0;i<10;i++)
printf("\nvalue in index[%d] is %d",i,marks[i]);
getch();
}
```
Q6.Write a program that read two integer arrays a and b having 5 elements each and prints the sum of the products as given below.(chap 5)
sum=a[0]*b[0] + a[1]*b[1] + .....+ a[4]*[4]
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int a[5],b[5],i;
int sum,prod;
printf("enter the values in 1st array\n");
for(i=0;i<5;i++)
scanf("%d",&a[i]);
printf("enter the values in 2nd array\n");
for(i=0;i<5;i++)
scanf("%d",&b[i]);
sum=0;
prod=1;
for(i=0;i<5;i++)
prod=a[i]*b[i];
sum=sum+prod;
printf("sum of product is %d",sum);
getch();
}
```
Q7.Write a program that read n floating point numbers and prints the sum of positive numbers.(chap 5)
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int j,sum,n;
float a[50];
printf("enter the number of integer\n");
scanf("%d",&n);
printf("enter value in array\n");
for(j=0;j<n;j++)
scanf("%f",&a[j]);
sum=0;
for(j=0;j<n;j++)
if(a[j]>0)
sum=sum+a[j];
printf("the sum of positive numbers is %d",sum);
getch();
}
```
Q9.Write codes that will print the following patterns.
a) 1
     1 2
     1 2 3
     1 2 3 4
     1 2 3 4 5
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int i,j;
for(i=1;i<=5;i++)
{
for(j=1;j<=i;j++)
printf("%d",j);
printf("\n");
}
getch();
}
```
b) 1 2 3 4 5
     1 2 3 4 
     1 2 3 
     1 2 
     1 
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int i,j;
for(i=5;i>=1;i--)
{
for(j=1;j<=i;j++)
printf("%d",j);
printf("\n");
}
getch();
}
```
c)  1 2 3 4 5
     2 3 4 5
     3 4 5
     4 5
     5 
```
# include<stdio.h>
# include<conio.h>
void main(void)
{
int i,j;
for(i=0;i<5;i++)
{
for(j=1+i;j<=5;j++)
printf("%d",j);
printf("\n");
}
getch();
}
```
d) * 
     * *
     * * * 
     * * * *
     * * * * *
```
# include <stdio.h>
# include <conio.h>
void main(void)
{
int i,j;
for(i=1;i<=5;i++)
{
for(j=1;j<=i;j++)
printf("* ",j);
printf("\n");
}
getch();
}
```
Q10.for two dimeentional array x that has r rows and c columnsn.print the sum and average of each row.(chap5)
```
# include<stdio.h>
# include<conio.h>
void main(void)
{
int x[50][50],sum,avg,i,j;
int r,c;
printf("enter total no of rows\n");
scanf("%d",&r);
printf("enter total no of column\n");
scanf("%d",&c);
for(i=0;i<r;i++)
for(j=0;j<c;j++)
scanf("%d",&x[i][j]);
for(i=0;i<r;i++)
{
sum=0;
for(j=0;j<c;j++)
sum=sum+x[i][j];
avg=sum/c;
printf("\nthe sum of %d row is %d and average is %d",i+1,sum,avg);
}
getch();
}
```
Q.For a floating-point array x whose size is n,find geeometric mean.
```
# include<stdio.h>
# include<conio.h>
# include<math.h>
void main(void)
{
int i,n;
float a[50],prod,gm;
printf("enter number");
scanf("%d",&n);
printf("enter the value in array");
for(i=0;i<n;i++)
scanf("%f",&a[i]);
{
prod=1;
for(i=0;i<n;i++)
prod=prod*a[i];
gm=pow((prod),1/n);
printf("%f",gm);
}
getch();
}
```
Q2.Write a program that prints the larger of two numbers entered from the keyboard.use a function to do the actual comparison of the two numbers .Pass the two numbers to the function as arguments and have the function return with return().  Chap 6
```
# include<stdio.h>
# include<conio.h>
void answer(int x,int y);
void main(void)
{
int i,j;
printf("enter the first value\n");
scanf("%d",&i);
printf("enter the second value\n");
scanf("%d",&j);
answer(i,j);
getch();
}
void answer(int x,int y)
{
if(x>y)
printf("x is largest");
else
printf("y is largest");
}
```
Q.Write a program using a function to calculate the area of rectangle. (chapter 6)
# include<stdio.h>
# include<conio.h>
```
int Area(int x,int y);
void main(void)
{
int i,j;
printf("enter the length\n");
scanf("%d",&i);
printf("enter the width\n");
scanf("%d",&j);
printf("the area of rectangle is %d",Area(i,j));
getch();
}
int Area(int x,int y)
{
int a;
a=x*y;
return a;
}
```
Q4.write a program that produces the following table of temperature in centigrade and fahrenheit from 0 degree to 50 degree centigrade .Use a function for Conversion.(chapter 6)
------------------------------------------------
 Centigrade               fahrenheit
------------------------------------------------
  0                                           32
  5
  10
  .
  .
  .
  50
```
# include<stdio.h>
# include<conio.h>
int fact(int x);
void main(void)
{
int i;
printf("\n----------------------------");
printf("\n Centigrade     Fahrenheit");
printf("\n----------------------------");
for(i=0;i<=50;i=i+5)
printf("\n %2d              %3d",i,fact(i));
getch();
}
int fact(int x)
{
int j,F;
F=1;
for(j=0;j<10;j++)
F=9/5*x+32;
return F;
}
```
Q6.Write a program that reads n floating point numbers in an array and prints their product using a function. ( chapter 6)
```
# include <stdio.h>
# include <conio.h>
void prod(float a[],int m);
void main(void)
{
float b[50];
int i,n;
printf("enter total no. of elements=\n");
scanf("%d",&n);
printf("enter values in array\n");
for(i=0;i<n;i++)
scanf("%f",&b[i]);
prod(b,n);
getch();
}
void prod(float a[],int m)
{
int i;
float product;
product=1;
for(i=0;i<m;i++)
product=product*a[i];
printf("the prod is=%f",product);
}
```
Q7.write a program that reads numbers in two integer array x and y or size m and n and prints them in ascending order using function.(chapter 6)
```
# include <stdio.h>
# include <conio.h>
void fn1(int a[],int c);
void fn2(int b[],int d);
void main(void)
{
int x[50],y[50],m,n,i;
printf(" enter no. of elements for first array ");
scanf("%d",&m);
printf(" enter no. of elements for 2nd array ");
scanf("%d",&n);
printf("enter values in first array=");
for(i=0;i<m;i++)
scanf("%d",&x[i]);
printf("enter values in 2nd array=");
for(i=0;i<n;i++)
scanf("%d",&y[i]);
fn1(x,m);
fn2(y,n);
getch();
}
void fn1(int a[],int c)
{
int i,j,holder;
for(i=0;i<c-1;i++)
for(j=0;j<c-1;j++)
if(a[j]>a[j+1])
{
holder=a[j];
a[j]=a[j+1];
a[j+1]=holder;
}
for(j=0;j<c;j++)
printf("\n first array sorted value is %d",a[j]);

}
void fn2(int b[],int d)
{
int i,j,holder;
for(i=0;i<d-1;i++)
for(j=0;j<d-1;j++)
if(b[j]>b[j+1])
{
holder=b[j];
b[j]=b[j+1];
b[j+1]=holder;
}
for(j=0;j<d;j++)
printf(" \n 2nd sorted array is %d",b[j]);
}
```
