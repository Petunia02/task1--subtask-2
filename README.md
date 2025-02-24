# task1--subtask-2
#include <iostream>
using namespace std;

int main() {
    int temp1, temp2, temp3;

    // Prompt the user to enter the first temperature reading
    cout << "Enter the first temperature reading: ";
    cin >> temp1;

    // Prompt the user to enter the second temperature reading
    cout << "Enter the second temperature reading: ";
    cin >> temp2;

    // Check if the second temperature increase is valid
    if (temp2 - temp1 > 50) {
        cout << "REDUCE FRYER HEAT BEFORE TAKING THE THIRD READING" << endl;
        return 0; // Exit the program if the increase is too high
    }

    // Check if the increase is too low
    if (temp2 - temp1 < 10) {
        cout << "Increase the fryer heat before taking the third reading" << endl;
        return 0; // Exit the program if the increase is too low
    }

    // Prompt the user to enter the third temperature reading
    cout << "Enter the third temperature reading: ";
    cin >> temp3;

    // Check if the third temperature reading is valid
   // if (temp3 - temp2 > 50) {
   //     cout << "REDUCE FRYER HEAT BEFORE TAKING THE THIRD READING" << endl;
  //      return 0; // Exit the program if the increase is too high
   // }

    // Check if the oil temperature is in the correct frying range
    if (temp3 >= 150 && temp3 <= 190) {
        cout << "You may start frying the Mangwinyas" << endl;
    } else {
        cout << "Oil is not ready for frying!" << endl;
    }

    return 0;
}
