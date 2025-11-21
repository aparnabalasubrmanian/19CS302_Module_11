
# EX 55 C program to find a square of number using function with arguments without return type.
## DATE: 13.11.25
## AIM:
To write a C program to find a square of number using function with arguments without return type.

## Algorithm

1. **Start**  
2. Define a function `findSquare(num)` that takes an integer argument.  
3. Inside the function, compute `num * num` and display the result.  
4. In the `main()` function:  
   - Accept an integer input from the user.  
   - Call `findSquare(number)` with the input value.  
5. **End**  


## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/
#include <stdio.h>

void findSquare(int num) {
    printf("Square of %d is: %d\n", num, num * num);
}

int main() {
    int number;
    printf("Enter a number: ");
    scanf("%d", &number);
    
    findSquare(number);
    
    return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/417382e7-5233-4f85-af71-e0b854b57f79)



## Result:
Thus the program was executed and the output was verified successfully.
