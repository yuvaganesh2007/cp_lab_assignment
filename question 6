#include <stdio.h>
#include <stdlib.h>

int main() {
    FILE *fp;        
    char text[200];  

    fp = fopen("filename.txt", "a");

    if (fp == NULL) {
        printf("Unable to open file\n");
        return 0; 
    }

    printf("Enter text to append:\n");
    fgets(text, sizeof(text), stdin);  

    fputs(text, fp); 
    fclose(fp);

    printf("Text appended successfully\n");

    return 0;
}
