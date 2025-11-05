#include <stdio.h>
#include <stdlib.h>

int main() {
    float *ptr;   
    int n, i;     
    float sum = 0, average;

    printf("Enter how many numbers: ");
    scanf("%d", &n);

    ptr = (float *)malloc(n * sizeof(float));

    if (ptr == NULL) {
        printf("Memory allocation failed\n");
        return 0;
    }

    printf("Enter %d numbers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%f", &ptr[i]);
        sum += ptr[i];
    }

    average = sum / n;

    printf("Sum = %.2f\n", sum);
    printf("Average = %.2f\n", average);

    free(ptr);

    return 0;
}
