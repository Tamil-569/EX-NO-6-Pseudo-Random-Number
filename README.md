
# EX-NO-6-Pseudo-Random-Number
## Date : 28-10-2026
# AIM: 

Implementation of Pseudorandom Number Generation Using Standard library


# ALGORITHM:

1) Start the program and import the required libraries.
2) Seed the random number generator using the current time(i.e)
rand(time(0));
3) Get the number of randon number to generate.
4) Pass the value for number of iterations and print the numbers.
5) End the program.


# PROGRAM:
```

#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    printf("Enter the minimum value: ");
    
    scanf("%d", &min);
    printf("Enter the maximum value: ");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }
    return 0;
}
```


# OUTPUT:
<img width="1644" height="758" alt="{AE652CB9-0245-4961-A5DE-10CCD3D4D6D2}" src="https://github.com/user-attachments/assets/74d4ab88-8dae-4adc-b4d2-edf0c1c5aa7b" />



# RESULT:
The implementation of Pseudorandom Number Generation using Standard library is successful.
