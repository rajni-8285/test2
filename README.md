#include <stdio.h>

Int print Board(char board[3][3]) {
    printf(" %c | %c | %c \n", board[0][0], board[0][1], board[0][2]);
    printf("---+---+---\n");
    printf(" %c | %c | %c \n", board[1][0], board[1][1], board[1][2]);
    printf("---+---+---\n");
    printf(" %c | %c | %c \n", board[2][0], board[2][1], board[2][2]);}
int check Win(char board[3][3], char player) {
    int i;
    // Check rows
    for (i = 0; i < 3; i++) {
        if (board[i][0] == player && board[i][1] == player && board[i][2] == player)
            return 1
}
    // Check columns
    for (i = 0; i < 3; i++) {
        if (board[0][i] == player && board[1][i] == player && board[2][i] == player)
            return 1;
    }
    // Check diagonals
    if ((board[0][0] == player && board[1][1] == player && board[2][2] == player) ||
        (board[0][2] == player && board[1][1] == player && board[2][0] == player))
        return 1;
    return 0;
}

int main() {
 char board[3][3] = {{'1', '2', '3'}, {'4', '5', '6'}, {'7', '8', '9'}};
    char player = 'X';
    int move, row, col;
    int win = 0;
        while (!win) {
        printBoard(board);
        printf("Player %c, enter your move (1-9): ", player);
        scanf("%d", &move);
        row = (move - 1) / 3;
        col = (move - 1) % 3;
        if (board[row][col] != 'X' && board[row][col] != 'O') {
            board[row][col] = player;
            win = checkWin(board, player);
            player = (player == 'X') ? 'O' : 'X';
        } else {
            printf("Invalid move, try again.\n")
        }
    }

    printBoard(board);
    printf("Player %c wins!\n", (player == 'X') ? 'O' : 'X');

    return 0;
}









# PROJECT
