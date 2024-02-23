/*		CODE NUMBER 2
        Full Name	:	Deepthi Jibu Valachery
		Student ID	:	[redacted]
		Class		:	[redacted]
		Programme	:	Assignment 2
*/

#include <iostream>
#include <iomanip>
#include <cmath>
#include <climits>

using namespace std;

void printStars (int n) {
	int count;
	
	for (count=1; count<=n; count=count+1)
		cout << "*";
}


int main () {
	
	int year1, year2, tempYr, years;
	int sumTotal, sumC1, sumC2, sumC3, sumC4;
	int n; 
	int min = INT_MAX, max = INT_MIN, minYear, maxYear;
	
	float graph30, graph50, graph50G, graph90;
	float avgTotal, avg30, avg50, avg50G, avg90;
	
	double totalStudent, c1, c2, c3, c4;
	double percent30, percent50, percentG50, percent90;
	double avgPercent30, avgPercent50, avgPercent50G, avgPercent90;
																								// Declarations
	
	cout << "Course Code - Assignment 2" << endl;
	cout << "========================" << endl;
	cout << endl;
	
	cout << "Starting year: ";
	cin >> year1;
	
	cout << "Ending year: ";
	cin >> year2;																				// User input years
	cout << endl;
	
	if (year1 < 2010 || year1 > 2018) {
		cout << "The starting year is out of range [2010..2018]. Aborting.....";
		exit (1) ;
	} 
	else if (year2 > 2018 || year2 < 2010) {
		cout << "The ending year is out of range [2010..2018]. Aborting.....";
		exit (1) ;																				// Checking if years are valid
	}
	if (year1 > year2) {
		tempYr = year1;
		year1 = year2;
		year2 = tempYr;
	}																							// Swapping the years
	
	cout << "Analysing from year " << year1 << " to " << year2 << "...." << endl << endl;
	
	years = (year2 - year1) + 1;
	
	sumC1 = 0;
	sumC2 = 0;
	sumC3 = 0;
	sumC4 = 0;
	
	for (n = year1; n <= year2; n = n + 1) {
		cout << "Please enter data for " << n << " [Total students, Category 1, Category 3, Category 4] " << endl;
		cout << "(Please click the enter button after each data) : " << endl;
		cin >> totalStudent >> c1 >> c3 >> c4;													// User inputs data for each year
		cout << endl;							
		
		
		cout << "Year of exam: " << n;
		cout << endl;
		
		percent30 = (c1/totalStudent) * 100;
		c2 = totalStudent - c3;																	// Calculate category 2
		percent50 = (c2/totalStudent) * 100;
		percentG50 = (c3/totalStudent) * 100;
		percent90 = (c4/totalStudent) * 100;
		
		cout << fixed << setprecision(2);
		
		cout << "Percentage getting <= 30% : " << percent30 << endl;
		cout << "Percentage getting < 50% : " << percent50 << endl;
		cout << "Percentage getting >= 50% : " << percentG50 << endl;
		cout << "Percentage getting >= 90% : " << percent90 << endl;							// Percentages in each category 
		
		cout << endl;
		
		sumTotal = sumTotal + totalStudent;
		sumC1 = sumC1 + c1;
		sumC2 = sumC2 + c2;
		sumC3 = sumC3 + c3;
		sumC4 = sumC4 + c4;																		// Total students in each category
		
		if (c4 > max){
			max = c4;
			maxYear = n;
		}
		if (c2 < min) {
			min = c2;
			minYear = n;
		}																						// Max and min with the year it occured
		
	}
	
	avgTotal = floor (sumTotal/years);
	avg30 = floor (sumC1/years);
	avg50 = floor (sumC2/years);
	avg50G = floor (sumC3/years);
	avg90 = floor (sumC4/years);																// Average number of students 
	
	avgPercent30 = (avg30/avgTotal) * 100; 
	avgPercent50 = (avg50/avgTotal) * 100; 
	avgPercent50G = (avg50G/avgTotal) * 100;
	avgPercent90 = (avg90/avgTotal) * 100; 														// Average percentage of students
	
	cout << "Period of analysis: " << year1 << " to " << year2 << endl;
	cout << "Number of years analysed: " << years << endl;
	cout << endl;
	
	cout << "Average number of students getting <= 30%: " << avg30 << " (" << avgPercent30 << "%)" << endl;
	cout << "Average number of students getting < 50%: " << avg50 << " (" << avgPercent50 << "%)" << endl;
	cout << "Average number of students getting >= 50%: " << avg50G << " (" << avgPercent50G << "%)" << endl;
	cout << "Average number of students getting >= 90%: " << avg90 << " (" << avgPercent90 << "%)" << endl;
	
	cout << endl;																				// Displaying the averages
	
	cout << "The highest number of students getting >= 90% was " << max << endl;
	cout << "It occurred in " << maxYear << endl;
	cout << endl;
	
	cout << "The lowest number of students getting < 50% was " << min << endl;
	cout << "It occurred in " << minYear << endl;
	cout << endl;																				// Displaying the max and min
	
	cout << "Graphical display of averages for period " << year1 << " to " << year2 << ":" << endl;
	
	graph30 = ceil (avg30/500) ;
	graph50 = ceil (avg50/500) ;
	graph50G = ceil (avg50G/500) ;
	graph90 = ceil (avg90/500) ;
	
	cout << "Students that got <= 30% : " ; printStars (graph30);
	cout << endl;
	cout << "Students that got <  50% : " ; printStars (graph50);
	cout << endl;
	cout << "Students that got >= 50% : " ; printStars (graph50G);
	cout << endl;
	cout << "Students that got >= 90% : " ; printStars (graph90);								// Displaying graph
    
    
	return 0;
}
