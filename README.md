# Cube
Points
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main() {
    srand(time(0)); // seed random number generator with current time
    int roll = rand() % 6 + 1; // roll the cube
    int score = 0; // initialize score to 0
    cout << "Rolling the cube...\n";
    cout << "You rolled a " << roll << endl;
    if (roll == 1) {
        score += 10; // add 10 points for landing on side 1
        cout << "You landed on side 1! +10 points\n";
    } else if (roll == 2) {
        score += 5; // add 5 points for landing on side 2
        cout << "You landed on side 2! +5 points\n";
    } else if (roll == 3) {
        score += 7; // add 7 points for landing on side 3
        cout << "You landed on side 3! +7 points\n";
    } else if (roll == 4) {
        score += 2; // add 2 points for landing on side 4
        cout << "You landed on side 4! +2 points\n";
    } else if (roll == 5) {
        score += 8; // add 8 points for landing on side 5
        cout << "You landed on side 5! +8 points\n";
    } else {
        score += 1; // add 1 point for landing on side 6
        cout << "You landed on side 6! +1 point\n";
    }
    cout << "Your final score is " << score << endl; // display final score
    return 0;
}
