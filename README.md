
## Name:Raha Priya Dharshini M
## Reg no.:212224240124
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

void calculateEMI(float principal, float rate, int time) {
    float emi;
    rate = rate / (12 * 100); 
    int months = time * 12;   
    emi = (principal * rate * (1 + rate) * months) / 2;
    printf("Estimated EMI: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int time;
    printf("Enter loan amount: ");
    scanf("%f", &principal);
    printf("Enter annual interest rate (in %%): ");
    scanf("%f", &rate);
    printf("Enter loan period (in years): ");
    scanf("%d", &time);
    calculateEMI(principal, rate, time);
    return 0;
}
```


## OUTPUT
![Screenshot 2025-05-12 221753](https://github.com/user-attachments/assets/b5272102-854d-4c4f-93a7-5e128e9ec16d)


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

int main() {
    int n = 6; // Number of terms
    int first = 0, second = 1, next, i;

    printf("Fibonacci series for %d terms:\n", n);

    for(i = 0; i < n; i++) {
        if(i == 0)
            next = first;
        else if(i == 1)
            next = second;
        else {
            next = first + second;
            first = second;
            second = next;
        }

        printf("%d ", next);
    }

    return 0;
}
```


## OUTPUT
![Screenshot 2025-05-12 222552](https://github.com/user-attachments/assets/1dcb0d5d-6fa4-4ca4-9635-f0f3adedee09)


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

int main() {
    int n, i;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n]; 

    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("The last element is: %d\n", arr[n - 1]);

    return 0;
}
```

## OUTPUT
![Screenshot 2025-05-12 223514](https://github.com/user-attachments/assets/ba9daa15-55e2-4303-8831-72ea832c10f6)

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

int main() {
    int n, i, count = 0;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    if(arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements: %d\n", count);
    return 0;
}
```


## OUTPUT
![Screenshot 2025-05-12 224219](https://github.com/user-attachments/assets/e9e6c2a2-880c-4d3f-8b3d-77f3ba261fa3)
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
int main() {
    int n, i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d integers:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Modified array:\n");
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }
    return 0;
}
```


## Output:
![image](https://github.com/user-attachments/assets/30b6a08e-31c3-4178-9836-4c6539f00729)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



