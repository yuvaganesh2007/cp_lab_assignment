#include <stdio.h>
   #include <stdlib.h>

int main() {
    int *ptr;  
    ptr = (int *)malloc(sizeof(int));

   
    if (ptr == NULL) {
        printf("Memory allocation failed\n");
        return 0; 
    }
      printf("Enter an integer value: ");
      scanf("%d", ptr);

    printf("You entered: %d\n", *ptr);

    free(ptr);

    return 0;
}
