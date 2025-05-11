# EX 12 C program to check whether the given number is prime or not using function without return type and with arguments.
## DATE: 11/05/2025
## AIM:
To write a C program to check whether the given number is prime or not using function without return type and with arguments.

## Algorithm
1.Start the program and define a function with arguments and no return type.

2.Read a number from the user in main().

3.Pass the number as an argument to the function.

4.In the function, check if the number is divisible by any number from 2 to n/2.

5.Print whether the number is prime or not from the function.  

## Program:
```
/*
C program to check whether the given number is prime or not using function without return type and with arguments.
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/

#include <stdio.h>

void checkPrime(int num)
{
    int i, isPrime = 1;

    if(num <= 1)
    {
        printf("%d is not a prime number.\n", num);
        return;
    }

    for(i = 2; i <= num / 2; i++)
    {
        if(num % i == 0)
        {
            isPrime = 0;
            break;
        }
    }

    if(isPrime)
    {
        printf("%d is a prime number.\n", num);
    }
    else
    {
        printf("%d is not a prime number.\n", num);
    }
}

int main()
{
    int number;

    printf("Enter a number: ");
    scanf("%d", &number);

    checkPrime(number);

    return 0;
}

```

## Output:
![image](https://github.com/user-attachments/assets/957a57bf-913d-499f-bde4-c30b84bcb631)



## Result:
Thus the program was executed and the output was verified successfully.
