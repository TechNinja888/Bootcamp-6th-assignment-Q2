#include <iostream>
#include <string>

using namespace std;

int main() {
    // Predefined correct username and password
    string correct_username = "FidelismichealB";
    string correct_password = "TechNinja888";

    string username, password;

    while (true) {
        // Prompt for username
        cout << "Enter username (or 'q' to quit): ";
        getline(cin, username);

        // Check if user wants to quit
        if (username == "q") {
            cout << "Exiting..." << endl;
            break;
        }

        // Prompt for password
        cout << "Enter password (or 'q' to quit): ";
        getline(cin, password);

        // Check if user wants to quit
        if (password == "q") {
            cout << "Exiting..." << endl;
            break;
        }

        // Check if the username and password are correct
        if (username == correct_username && password == correct_password) {
            cout << "Login successful!" << endl;
            break;
        } else {
            cout << "Wrong username or password, please try again." << endl;
        }
    }

    return 0;
}
