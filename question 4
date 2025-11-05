#include <stdio.h>
#include <stdlib.h>

int main() {
    int *stack;       
    int n, top = -1;  
    int choice, value;
    int i;
    printf("Enter size of stack: ");
    scanf("%d", &n);
    stack = (int *)malloc(n * sizeof(int));
    if (stack == NULL) {
        printf("Memory allocation failed\n");
        return 0; 
    }

    do {
        printf("\n--- Stack Menu ---\n");
        printf("1. Push\n");
        printf("2. Pop\n");
        printf("3. Display\n");
        printf("4. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);

        switch (choice) {
            case 1: 
                if (top == n - 1) {
                    printf("Stack Overflow\n");
                } else {
                    printf("Enter value to push: ");
                    scanf("%d", &value);
                    top++;
                    stack[top] = value;
                    printf("%d pushed onto stack\n", value);
                }
                break;

            case 2: 
                if (top == -1) {
                    printf("Stack Underflow\n");
                } else {
                    printf("Popped element: %d\n", stack[top]);
                    top--;
                }
                break;

            case 3: 
                if (top == -1) {
                    printf("Stack is Empty\n");
                } else {
                    printf("Stack elements:\n");
                    for (i = top; i >= 0; i--) {
                        printf("%d\n", stack[i]);
                    }
                }
                break;

            case 4: 
                printf("Exiting program\n");
                break;

            default:
                printf("Invalid choice\n");
        }

    } while (choice != 4);

    free(stack);

return 0;
}

    return 0;
}
