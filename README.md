# Lab-12.20-
#include <iostream>
using namespace std;

int main() {
  int value1;
  int value2;		// value is some positive number n
	double total = 0;	// total holds the sum of the first n positive numbers 
	int number;		// the amount of numbers
	double mean;		// the average of the first n positive numbers

	cout << "Please enter a positive integer" << endl;
	cin >> value1;
  cout << "Please enter a positive integer" << endl;
	cin >> value2;
  
	if (value1 > 0) 
	{
		for (number = value1; number <= value2; number++)
		{
			total = total + number;
      
		}	// curly braces are optional since there is only one statement

		mean = total / (value2 - value1 + 1);	// note the use of the typecast
													// operator here 
		cout << "The mean average of the first " << number
			 << " positive integers is " << mean << endl;
	}
	else
		cout << "Invalid input - integer must be positive" << endl;

}
