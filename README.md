#include <stdio.h>

int main() {
    int c;
    int number1, number2;

    printf("Enter the first number: ");
    scanf("%d", &number1);

    printf("Enter the second number: ");
    scanf("%d", &number2);

    printf("1. Addition\n");
    printf("2. Subtraction\n");
    printf("3. Division\n");
    printf("4. Multiplication\n");
    
    printf("Choose an operation: ");
    scanf("%d", &c);
    
    switch(c){
        case 1:
            printf("The result of the addition is: %d\n", number1 + number2);
            break;
        case 2:
            printf("The result of the subtraction is: %d\n", number1 - number2);
            break;
        case 3:
            if(number2 != 0) {
                printf("The result of the division is: %f\n", (float) number1 / number2);
            } else {
                printf("Division by zero is not allowed.\n");
            }
            break;
        case 4:
            printf("The result of the multiplication is: %d\n", number1 * number2);
            break;
        default:
            printf("Please enter a valid number.\n");
            break;
    }
    return 0;
}
