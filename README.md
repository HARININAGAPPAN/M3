# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>
void calculateEMI(float principal, float rate, int months)
{
    float r, emi;
    r = rate / (12 * 100); // Monthly interest rate
    emi = (principal * r * pow(1 + r, months)) / (pow(1 + r, months) - 1);
    printf("The EMI is: %.2f\n", emi);
}
int main()
{
    float principal, rate;
    int months;
    printf("Enter the principal amount: ");
    scanf("%f", &principal);
    printf("Enter the annual rate of interest (in %%): ");
    scanf("%f", &rate);
    printf("Enter the number of months: ");
    scanf("%d", &months);
    calculateEMI(principal, rate, months);
    return 0;
}

```


## OUTPUT


![438661447-7c49b6d8-f7e8-4c39-b69b-130bd7474f6c](https://github.com/user-attachments/assets/c1beb22b-9196-4b12-81e3-926feebbd9b1)



## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() 
{
    int n = 6; 
    int first = 0, second = 1, next, i;
    printf("Fibonacci Series for %d terms:\n", n);
    printf("%d %d ", first, second);
    for(i = 2; i < n; i++) 
    {
        next = first + second;
        printf("%d ", next);
        first = second;
        second = next;
    }
    return 0;
}


```

## OUTPUT


![438661623-11632bf5-f9fe-4713-9ed0-ea76d1b79577](https://github.com/user-attachments/assets/4f1d362b-9413-4605-92d4-2d7d4783e6de)






## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
void main() 
{
    int n, i, arr[100];
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }
    printf("The last element is: %d\n", arr[n-1]);
}


```

## OUTPUT






![438661862-e2d6f41b-c13f-4c3a-923b-98d023ddf064](https://github.com/user-attachments/assets/2431d52f-ae4b-4750-b1ad-7ef4d5df247b)



## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
void main() 
{
    int n, i, count = 0, arr[100];
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }
    for(i = 0; i < n; i++)
    {
        if(arr[i] > 0)
        {
            count++;
        }
    }
    printf("Total number of positive elements = %d\n", count);
}


```


## OUTPUT

![438662072-9270185d-86f5-40e7-af37-3db6a0442c93](https://github.com/user-attachments/assets/6c4dfc23-ac33-43f9-a196-73ef0f8a0e02)




## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>
void main() 
{
    int n, i, arr[100];
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }
    printf("Updated array:\n");
    for(i = 0; i < n; i++)
    {
        if(arr[i] % 2 == 0) 
        {
            printf("E ");
        }
        else
        {
            printf("%d ", arr[i]);
        }
    }
}

```

## Output:
 
![438662211-025a24c3-a684-4c5a-af3a-aa209d73127f](https://github.com/user-attachments/assets/805be7a1-6cca-402f-b87b-f6ff12c7f049)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



