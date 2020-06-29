#include <iostream>

using namespace std;

const int ROCK		= 1;

const int PAPER		= 2;

const int SCISSORS	= 3;

const int QUIT      = 4;

// function prototype
int getUserChoice();

int getComputerChoice();

void determineOutcome(int, int);

void displayChoice(int);

//function main

int main( )
{

    int userChoice;
	int computerChoice;

    // comment 1: generate a random number in the range of 1 through 3.
	computerChoice = getComputerChoice();
	// comment 2: ask for user's choice
	userChoice = getUserChoice();

	while (userChoice != QUIT)
	{
        // comment 3: display user's choice
		cout << "\nYou selected: ";
		displayChoice(userChoice);

        // comment 4: display computer's choice
		cout << "\nThe computer selected: ";
		displayChoice(computerChoice);

        // comment 5: determine the outcome
		determineOutcome(userChoice, computerChoice);
		cout<<endl;

        // comment 6: Keep running the program until the user input 4
		computerChoice = getComputerChoice();
		userChoice = getUserChoice();

	}
    return 0;
}

int getUserChoice()
{
    int choice;

    // comment 7: show the choices
    cout << "Game Menu\n";
	cout << "--------\n";
	cout << "1) Rock \n";
	cout << "2) Paper \n";
	cout << "3) Scissors \n";
	cout << "4) Quit \n";

    cout << "\nEnter your choice: ";
    cin >> choice;

    // comment 8: if the input value is invalid, ask for the numebr agian.
    while (choice < 1 || choice > 4)
    {
        cout << "Invalid selection. Enter 1, 2, 3, or 4: ";
        cin >> choice;
    }

    // comment 9: if the input in 1 to 4, then return each constant variable for each choice number.
    switch (choice)
    {
    case 1:
        return ROCK;
        break;
    case 2:
        return PAPER;
        break;
    case 3:
        return SCISSORS;
        break;
    case 4:
        return QUIT;
        break;
    }
}

int getComputerChoice()
{
    int num;

    //comment 10: generate a number between 1, 2, and 3
    num = rand() % 2 + 1;

    //comment 11: if the input in 1 to 3, then return each constant variable
    switch (num)
    {
        case 1:
            return ROCK;
            break;
        case 2:
            return PAPER;
            break;
        case 3:
            return SCISSORS;
            break;
    }
}

void determineOutcome(int user, int computer)
{
    // comment 11: detemine who wins or whethe it is a tie.
    if (user == computer)
    {
        cout << "\nTie. No winner. \n";
    }
    else if (user == 1 && computer == 2)
    {
        cout << "\nComputer wins! Paper wraps rock. \n";
    }
    else if (user == 1 && computer == 3)
    {
        cout << "\nYou wins! Rock smashes scissors. \n";
    }
    else if (user == 2 && computer == 1)
    {
        cout << "\nYou wins! Paper wraps rock. \n";
    }
    else if (user == 2 && computer == 3)
    {
        cout << "\nComputer wins! Scissors cuts paper. \n";
    }
    else if (user == 3 && computer == 1)
    {
        cout << "\nComputer wins! Rock smashes scissors. \n";
    }
    else if (user == 3 && computer == 2)
    {
        cout << "\nYou wins! Scissors cuts paper. \n";
    }
}

void displayChoice(int number){
    // comment 12: display the name of each choice.
    switch (number)
    {
        case 1:
            cout << "Rock";
            break;
        case 2:
            cout << "Paper";
            break;
        case 3:
            cout << "Scissors";
            break;
    }
}

