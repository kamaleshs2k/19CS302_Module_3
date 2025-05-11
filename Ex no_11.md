# EX 11 C Program to convert a given decimal value to binary using function without arguments with return type.
## DATE:11/05/2025
## AIM:
To write a C Program to convert a given decimal value to binary using function without arguments with return type.

## Algorithm
1.Start the program and declare a function to return binary.

2.Inside the function, read a decimal number from the user.

3.Convert the decimal number to binary using an array and loop.

4.Return the binary number as an integer array or display from the function.

5.In main(), call the function to trigger conversion.

## Program:
```
/*
Program to C Program to convert a given decimal value to binary using function without arguments with return type.
Developed by: Kamalesh S
RegisterNumber: 212223060108 
*/

#include <stdio.h>

int convertToBinary()
{
    int num, binary[32], i = 0, j;

    printf("Enter a decimal number: ");
    scanf("%d", &num);

    if(num == 0)
    {
        printf("Binary = 0\n");
        return 0;
    }

    while(num > 0)
    {
        binary[i] = num % 2;
        num = num / 2;
        i++;
    }

    printf("Binary = ");
    for(j = i - 1; j >= 0; j--)
    {
        printf("%d", binary[j]);
    }
    printf("\n");

    return 1;
}

int main()
{
    convertToBinary();
    return 0;
}

```

## Output:

![image](https://github.com/user-attachments/assets/572b7254-5fdc-4cbd-9619-a35be338bfef)


## Result:
Thus the program was executed and the output was verified successfully.
