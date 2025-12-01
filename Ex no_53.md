
# EX 53 C program to remove duplicates in an array.
## DATE: 13.11.25
## AIM:
To write a C program to remove duplicates in an array.

## Algorithm
1. **Start**  
2. Input the number of elements `n`.  
3. Input `n` elements into the array.  
4. Create an empty temporary array `temp` to store unique elements.  
5. Initialize an index variable `index = 0`.  
6. Loop through each element in the original array:  
   - Check if the element already exists in `temp`.  
   - If the element is not a duplicate, add it to `temp` and increment `index`.  
7. Copy the elements from `temp` back to the original array.  
8. Update `n` to the new size of the array.  
9. Print the modified array without duplicates.  
10. **End**  

This step-by-step method ensures that duplicates are effectively removed while maintaining the order of unique elements. Let me know if you need optimizations! 🚀
 

## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/
#include <stdio.h>

int main()
{
    int n, i, j, k;
    int a[100];

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter the elements: ");
    for (i = 0; i < n; i++)
        scanf("%d", &a[i]);

    for (i = 0; i < n; i++)
    {
        for (j = i + 1; j < n; j++)
        {
            if (a[i] == a[j])
            {
                for (k = j; k < n - 1; k++)
                    a[k] = a[k + 1];

                n--;
                j--;
            }
        }
    }

    printf("Array after removing duplicates: ");
    for (i = 0; i < n; i++)
        printf("%d ", a[i]);

    return 0;
}

```

## Output:

![image](https://github.com/user-attachments/assets/56f5c64c-b809-461f-8156-695f95722459)


## Result:
Thus the program was executed and the output was verified successfully.
