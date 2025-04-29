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
void calculateEMI(float principal, float rate, int year) {
    float monthlyRate = rate / (12 * 100);
    int months = year * 12;
    float emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / 
                (pow(1 + monthlyRate, months) - 1);
    printf("Monthly EMI is= %.3f\n", emi);
}

int main() {
    float principal = 345000.80;
    float rate = 9.25;
    int year= 4;
    calculateEMI(principal, rate, year);
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/45b5536c-bb0f-4354-aef4-6c0dbdc58fe8)





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 10.

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

int main() {
    int n = 10;
    int first = 0, second = 1, next;
    for (int i = 0; i < n; i++) {
        if (i <= 1) {
            next = i; 
        } else {
            next = first + second; 
            first = second;        
            second = next;  
        }
        printf("%d ", next);
    }

    printf("\n");
    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/f8f9b719-071b-4e31-ba67-19089eced125)








## RESULT
Thus the program to generate the Fibonacci series for the value 10 has been executed successfully.
 
 


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

int main() {
    int n;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("%d\n", arr[n - 1]);
    
    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/a1257554-d92d-450a-9f7f-cddd0fdfb1a2)









## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-AND-NEGATIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements and negative elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1 for positive.
5.	else increment count by 1 for negative.
6.	Display result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
    int m,p=0,n=0;
    scanf("%d",&m);
    int arr[m];
    for(int i=0;i<m;i++)
    {
        scanf("%d",&arr[i]);
    }
    for(int i=0;i<m;i++)
    {
        if(arr[i]>0)
        {
            p++;
        }
        else if(arr[i]<0)
        {
            n++;
        }
    }
    printf("count  of positive numbers  in array: %d\n",p);
    printf("count  of negative numbers  in array: %d\n",n);
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/711f1aed-e41b-4edf-ae34-e584f1316e5e)




## RESULT
Thus the program to count total number of positive elements and negative elements in an array has been executed successfully.





 
 


# EX -15 - Replace All odd Elements With 1 In One Dimensional Array

## Aim:
To write a C program to replace all odd elements with 1 in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is odd (i.e., if the element modulo 2 equals 1).
3.	Replace even elements with 1:
     If an element is even, replace that element with the character 1.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int arr[100], n, i;
    scanf("%d", &n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 != 0) {  
            arr[i] = 1;
        }
    }
    for(i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");

    return 0;
}
```
## Output:
 ![image](https://github.com/user-attachments/assets/e9c4b1eb-63cc-40f4-b5cb-d80ca27f388f)



## Result:

Thus, the program to replace all odd elements with 1 in one dimensional array was verified successfully.



