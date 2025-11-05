#include <stdio.h>
  #include <stdlib.h>

int main() {
    int *ptr;  
    int n, i;

    printf("Enter number of integers: ");
    scanf("%d", &n);

    ptr = (int *)calloc(n, sizeof(int));

   if (ptr == NULL) {
        printf("Memory allocation failed\n");
        return 0;
    }

  
    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &ptr[i]);
    }

    printf("Stored integers are:\n");
    for (i = 0; i < n; i++) {
        printf("%d ", ptr[i]);
    }
    
    free(ptr);

    return 0;
}
