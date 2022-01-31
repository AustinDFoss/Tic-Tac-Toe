# Tic-Tac-Toe
Loom Video Explanation: https://www.loom.com/share/742753c3815b4d99a662a65f94bb2e6d
For educational purposes

#include <stdio.h>
#define X 3
#define Y 3

// Prints array
void printArray(char row[][Y], size_t one, size_t two)
{
    // Column Headers
    printf("%s", "       [0]  [1]  [2]");
    for (size_t i = 0; i < one; ++i) {
        // Labels Rows
        printf("\nrow[%lu] ", i);
        for (size_t j = 0; j < two; ++j) {
            printf("%-5c", row[i][j]);
        }
    }
}

int main(void)
{
    char row[X][Y] =
    { { '-', '-', '-'},
      { '-', '-', '-'},
      { '-', '-', '-'}};
    // Prints rows and font
    puts("Enter Grid Number: ");
    printArray(row, X, Y);
}
