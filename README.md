# Functions-Lecture
// MATH LIBRARY.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

    #include <iostream>
    using namespace std;

    void welcome();
    void  goodbye();



    int main()
  	{

	welcome();
	goodbye();


	}

	void welcome() {
	cout << "Welcome to my program" << endl;

	}


	void goodbye() {
	cout << "End of the program. Goodbye! " << endl;

  	}

## Exercises

	#include <iostream>
	#include <string>
	#include <math.h>
	#include <cmath>
	using namespace std;

	string message(double num)
	{

	cout << "\n\nThe exponent from 1-10 is: " << endl;
	double y = 1;
	do
	{
		cout << y << " exponent value for " << num << " is: ";
		
		cout << pow(num, y) << endl;
		y++;
	} while (y != 11);

	return "/////////////////////";
	}

	int main()
	{

	int num, fact = 1;

	cout << "Enter number: " << endl;
	cin >> num;

	while (cin.fail())
	{
		cout << "Invalid " << endl;
		cin.clear();
		cin.ignore(1000, '\n');
		cin >> num;
	}


	cout << message(num) << endl;

	return 0;

	}

## Root Exercise
	#include <iostream>
	#include <string>
	#include <math.h>
	#include <cmath>
	using namespace std;

	string message(double num)
	{

	cout << "\n\nThe rooth from 1-10 is: " << endl;
	double y = 1;
	do
	{
		cout << y << " root value for " << num << " is: ";
		double x = 1 / y;
		double r = pow(num, x);
		cout << r << endl;
		y++;
	} while (y != 11);

	return "//////////////////////";
	}

	int main()
	{

	int num, fact = 1;
	
	cout << "Enter a number you want the root value from 1-10: " << endl;
	cin >> num;

	while (cin.fail())
	{
		cout << "Invalid input. " << endl;
		cin.clear();
		cin.ignore(1000, '\n');
		cin >> num;
	}


	cout << message(num) << endl;

	return 0;

	}
	
	
##

	#include <iostream>
	using namespace std;

	void myCalculation(int num) {
    num *= 2;
    num += 8;
    cout << num << endl;

	}

	int main()
	{
    int userNum;
    cout << "Enter a number : ";
    cin >> userNum;
    myCalculation(userNum);
	}
	
	
	
##
	
	
	#include <iostream>
	using namespace std;
	int myCalculation(int num) {
    num *= 2;
    num += 8;
    return num;
	}

	int main()
	{
    int userNum;
    cout << "Enter a number : ";
    cin >> userNum;
    userNum = myCalculation(userNum);
    cout << userNum << endl;
    return 0;
	}
	
	
##	
	
	
	#include <iostream>
	using namespace std;
	double sumItems(double item1 ,double item2) {
    double total = item1 + item2;
    return total;
	}

	int main()
	{
    double myMoney = 40.00;
    double shoes = 25.99;
    double tshirt = 11.50;

    if (sumItems(shoes, tshirt) <= myMoney) {
        cout << "YOU CAN AFFORD THESE ITEMS YAY" << endl;

    }
    else {
        cout << "Save up amigo" << endl;
    }

	}
	
	
##
	
	#include <iostream>
	using namespace std;
	string greetings(int time) {
	if (time < 12) {
		return "Good Morning!";
	}
	else {
		return "Good Afternoon";
	}

	}

	int main() {
	cout << "What time is it?" << endl;
	int userInput;
	cin >> userInput;

	cout << greetings(userInput) << endl;
	}
	
	
	
	
	#include <iostream>
	using namespace std;
	double sumItems(double item1, double item2) {
    double total = item1 + item2;
    return total;
	}

	int main()
	{
    double myMoney;
    double shoes;
    double tshirt;

    cout << "How much money do you have on your wallet right now?" << endl;
    cin >> myMoney;

    cout << "Okay, how much is the band shirt you always wanted?"<< endl;
    cin >> tshirt;
    cout << "Coolio, how are the shoes then?" << endl;
    cin >> shoes;


    if (sumItems(shoes, tshirt) <= myMoney) {
        cout << "YOU CAN AFFORD THESE ITEMS YAY" << endl;

    }
    else {
        cout << "Save up amigo" << endl;
    }

	}
	
	
	
##
	#include <iostream>
	using namespace std;
	string greetings(int time) {
	
	if (time < 12) {
		return "Good Morning";
	}
	else if (time >= 12 && time <= 17) {
		return "Good Afternoon";
	}
	else if (time >= 18 && time <= 21) {
		return "Good Evening";

	}
	else if (time >= 22 && time <= 24) {
		return "Good Night";
	}

	}
	int main() {
	cout << "What time is it? (24 HOUR FORMAT)" << endl;  
	int userInput; 
	cin >> userInput; 

	cout << greetings(userInput) << endl;
	return 0;
	}

