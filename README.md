# Escape-The-Gungeon-cpp
//Author- Jordan Garcia
//Assignment- Escape the Dungeon Adventure
//Description- Creating a code in C++ making a text based adventure in the way to escape the dungeon

#include <iostream>
#include <string>

using namespace std;

int main() {
    // Game Introduction
    cout << "Welcome to Escape the Dungeon!" << endl;
    cout << "You find yourself trapped in a dark dungeon."<< endl;
     cout << "Your mission is to find a way out."<<endl;
    cout << "What do you do?" << endl;

  
    cout << "1. Search the room" << endl;
    cout << "2. Try the door" << endl;

    int choice;
    cin >> choice;

    if (choice == 1) {
        cout << "You search the room and find a rusty key." << endl;
        cout << "Now what?" << endl;
        cout << "1. Take the key" << endl;
        cout << "2. Leave the key" << endl;
        cin >> choice;
        if (choice == 1){
            cout << "You take the key and continue" << endl;
        }
        else{
            cout << "You leave the key and continue" << endl;
        }
    } else if (choice == 2) {
        cout << "You try the door, but it's locked." << endl;
        cout << "You must find a way to open it." << endl;
        cout << "What do you do?" << endl;
        cout << "1. Search the room" << endl;
        cin >> choice;
        if (choice == 1){
            cout << "You search the room and find a rusty key." << endl;
            cout << "Now what?" << endl;
            cout << "1. Take the key" << endl;
            cout << "2. Leave the key" << endl;
            cin >> choice;
            if (choice == 1){
                cout << "You take the key and continue" << endl;
            }
            else{
                cout << "You leave the key and continue" << endl;
            }
        }
    } else {
        cout << "Invalid choice. Game Over." << endl;
        return 0;
    }

    return 0;
}
