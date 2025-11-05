#include <stdio.h>
#include <stdlib.h>

int main() {
    FILE *fp;     
    char ch;    

    fp = fopen("filename.txt", "r");

    if (fp == NULL) {
        printf("File cannot be opened\n");
        return 0; 
    }

    printf("File contents:\n");

    ch = fgetc(fp); 
    while (ch != EOF) {
        putchar(ch);
        ch = fgetc(fp); 
    }

    fclose(fp);

    return 0;
}
