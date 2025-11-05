#include <stdio.h>
#include <stdlib.h>

struct Student {
    char name[50];
    int roll;
    float marks;
};

int main() {
    struct Student student[100], temp;
    FILE *fp;
    int count = 0, i, j;

    fp = fopen("students.dat", "rb");
    if (fp == NULL) {
        printf("File cannot be opened\n");
        return 0;
    }

    while (fread(&student[count], sizeof(struct Student), 1, fp) == 1) {
        count++;
    }

    fclose(fp);

    for (i = 0; i < count - 1; i++) {
        for (j = i + 1; j < count; j++) {
            if (student[i].marks < student[j].marks) {
                temp = student[i];
                student[i] = student[j];
                student[j] = temp;
            }
        }
    }

 
    printf("\nRank-wise Student List:\n");
    for (i = 0; i < count; i++) {
        printf("Rank %d: Name: %s  Roll: %d  Marks: %.2f\n",
               i + 1, student[i].name, student[i].roll, student[i].marks);
    }

    return 0;
}
