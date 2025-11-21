
# EX 51 C program to reverse a string.
## DATE: 13.11.25
## AIM:
To write a C program to reverse a string.

## Algorithm
- Start
- Accept a string from the user.
- Determine the length of the string.
- Initialize two pointers:- One at the beginning (i = 0).
- One at the end (j = length - 1).

- Swap the characters at positions i and j.
- Increment i and decrement j.
- Repeat steps 5 and 6 until i is greater than or equal to j.



## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/
#include <stdio.h>
#include <string.h>

int main() {
    char str[100], reversed[100];
    int length, i;

    printf("Enter a string: ");
    scanf("%s", str);  // Reads a single word

    length = strlen(str);

    // Reverse manually
    for (i = 0; i < length; i++) {
        reversed[i] = str[length - i - 1];
    }
    reversed[length] = '\0'; // Null-terminate the reversed string

    printf("Reversed string: %s\n", reversed);
    
    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/a5f48a4c-97a5-4f48-818c-9235da71bb17)


## Result:
Thus the program was executed and the output was verified successfully.
