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

