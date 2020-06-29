#include <iostream>

using namespace std;

//function main

int main( )
{
    string name1, name2, name3, first_place, second_place, third_place;
    double time1, time2, time3;

    // comment1: explain the instruction
    cout << "Enter the names of three runners and their finishing times.\n";
    cout << "I will tell you who came in first, second, and third.\n\n" << endl;

    // comment2: Prompt the user for the name and finishing of the first runner (type string variable)
    cout << "Name of Runner 1: ";
    getline(cin, name1); // comment3: save the first name into name1
    cout << "Runner 1's finishing time: ";
    cin >> time1 ; // comment4: save the first finishing time into time1
    cin.ignore();
    cout << "\n";

    // comment5: Prompt the user for the name and finishing of the second runner (type string variable)
    cout << "Name of Runner 2: ";
    getline(cin, name2); // comment6: save the second name into name1
    cout << "Runner 2's finishing time: ";
    cin >> time2; // comment7: save the second finishing time into time1
    cin.ignore();
    cout << "\n";

    // comment8: Prompt the user for the name and finishing of the third runner (type string variable)
    cout << "Name of Runner 3: ";
    getline(cin, name3); // comment9: save the third name into name1
    cout << "Runner 3's finishing time: ";
    cin >> time3 ; // comment10: save the third finishing time into time1
    cin.ignore();
    cout << "\n";

    // comment11: determine whether any value is negative, if so, return the error message
    if (time1 <= 0 || time2 <= 0 || time3 <= 0)
    {
        cout << "Enter positive values only for each runner's time.";
    }
    else  //comment12: otherwise, determine who is 1st, 2nd, 3rd.
    {
        if (time1 > time2 && time1 > time3)
        {
            first_place = name1;
            if (time2 > time3)
            {
                second_place = name2;
                third_place = name3;
            }
            else
            {
                second_place = name3;
                third_place = name2;
            }
        }
        else if (time2 > time1 && time2 > time3)
        {
            first_place = name2;
            if (time1 > time3)
            {
                second_place = name1;
                third_place = name3;
            }
            else
            {
                second_place = name3;
                third_place = name1;
            }
        }
        else
        {
            first_place = name3;
            if (time2 > time1)
            {
                second_place = name2;
                third_place = name1;
            }
            else
            {
                second_place = name1;
                third_place = name2;
            }
        }
        //comment12: print out the 1st, 2nd, 3rd places.
        cout << first_place << " came in 1st place.\n";
        cout << second_place << " came in 2nd place.\n";
        cout << third_place << " came in 3rd place.\n";
    }

    return 0;
}

