#include <stdio.h>
int main()
 {
    int score = 0;
    char answer;
    // Question 1
    printf("What is the capital of India?\n");
    printf("A) Mumbai\n");
    printf("B) Delhi\n");
    printf("C) Kolkata\n");
    printf("D) Chennai\n");
    printf("Enter your answer (A/B/C/D): ");
    scanf(" %c", &answer);
    if (answer == 'B' || answer == 'b') {
        printf("Correct!\n");
        score++;
    } else {
        printf("Invalid\n");
    }
    // Question 2
    printf("Who is the founder of C programming language?\n");
    printf("A) Dennis Ritchie\n");
    printf("B) Bjarne Stroustrup\n");
    printf("C) Larry Wall\n");
    printf("D) Linus Torvalds\n");
    printf("Enter your answer (A/B/C/D): ");
    scanf(" %c", &answer);
    if (answer == 'A' || answer == 'a') {
        printf("Correct!\n");
        score++;
    } else {
        printf("Invalid\n");
    }
    // Question 3
    printf("What is the chemical symbol for gold?\n");
    printf("A) Ag\n");
    printf("B) Au\n");
    printf("C) Hg\n");
    printf("D) Pb\n");
    printf("Enter your answer (A/B/C/D): ");
    scanf(" %c", &answer);
    if (answer == 'B' || answer == 'b') {
        printf("Correct!\n");
        score++;
    } else {
        printf("Invalid\n");
    }
    printf("Your final score is: %d/3\n", score);
    return 0;
}

#   P R O J E C T  
 