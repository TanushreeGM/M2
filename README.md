# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int M,N;
    printf("Enter the starting value: ");
    scanf("%d",&M);
    printf("\nEnter the ending value: ");
    scanf("%d",&N);
    for(int num=M;num<=N;num++){
        printf("%d ",num);
    }
    return 0;
}
```
## OUTPUT:
<img width="399" height="238" alt="Screenshot 2025-12-26 185642" src="https://github.com/user-attachments/assets/e67448fb-5f83-402a-832a-55ac33ce1094" />










## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int n,row,col;
    printf("Enter the number of rows: ");
    scanf("%d",&n);
    for(row=1;row<=n;row++){
        for(col=1;col<=n-row;col++){
            printf(" ");
        }
        for(col=1;col<=row;col++){
            printf("* ");
        }
        printf("\n");
    }
    return 0;
}
```

## OUTPUT:
<img width="392" height="337" alt="Screenshot 2025-12-26 190152" src="https://github.com/user-attachments/assets/10996be9-fddd-444c-9215-9d655d82a005" />






## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include<stdio.h>
void add(int, int);
void sub(int,int);
int main()
{
    int n1,n2;
    printf("Enter 2 numbers:");
    scanf("%d%d",&n1,&n2);
    add(n1,n2);
    sub(n1,n2);
    return 0;
}
void add(int n1,int n2)
{
    int sum=n1+n2;
    printf("The sum of the two numbers is= %d",sum);
}
void sub(int n1,int n2)
{
    int sub=n1-n2;
    printf("\nThe subtracted value is= %d",sub);
}
```

## OUTPUT:
<img width="400" height="216" alt="image" src="https://github.com/user-attachments/assets/12a68241-3305-4418-a0c0-5f98f352384b" />






## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int num,sum=0,digit;
    scanf("%d",&num);
    for(int n=num;n>0;n/=10)
    {
        digit=n%10;
        if(digit%2!=0){
            sum+=digit;
        }
    }
    printf("Sum of odd digits = %d",sum);
    return 0;
    
}
```

## OUTPUT:
<img width="403" height="189" alt="image" src="https://github.com/user-attachments/assets/bbfbabb4-696c-4865-8486-03aff32a969f" />




## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include<stdio.h>
long fact(int n)
{
    int i,fact=1;
    for(i=1;i<=n;i++)
    {
        fact*=i;
    }
    return fact;
}
int main()
{
    int n;
    long result;
    scanf("%d",&n);
    result=fact(n);
    printf("The factorial is %ld",result);
    return 0;
    
}
```

## OUTPUT:
<img width="388" height="181" alt="image" src="https://github.com/user-attachments/assets/5918c284-028c-4e63-bef1-4dc006fedd93" />

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
