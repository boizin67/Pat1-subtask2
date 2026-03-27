# Pat1-subtask2#include <iostream>
using namespace std;

int main() { 
    int temp1, temp2, temp3;

    // Input temperatures
    cout << "Enter first temperature: ";
    cin >> temp1;

    cout << "Enter second temperature: ";
    cin >> temp2;

    cout << "Enter third temperature: ";
    cin >> temp3;

    // Check second reading
    if (temp2 - temp1 > 50) {
        cout << "Warning: Temperature increased too fast!" << endl;
    }
    else if (temp1 - temp2 > 50) {
        cout << "Warning: Temperature dropped too fast!" << endl;
    }
    else {
        cout << "Second reading is within safe range." << endl;
    }

    // Check third reading
    if ((temp3 - temp1) < 10) {
        cout << "Oil is not heating properly." << endl;
    }
    else {
        cout << "Oil temperature is increasing normally." << endl;
    }

    return 0;
}
