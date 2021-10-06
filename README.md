# First-C-Lab
Displays the use of C++ to write functions. One finds the mean of two numbers. The next one will find the sum of the series 0,1,2..n where n is user input

#include <iostream>
using namespace std;

//define the function 
int factorial (int a)
{
    int ans=1; 
    for (int i=a; i > 0; i --)
    {
        ans= ans * i; 
    }

    return ans; 
}

int main()
{
    //Q #1: Write a C++ Program to print "Hello, World!"
    printf ("Hello, World!\n");

    //Q #2: Take two numeric user inputs and calculate and print the average of those two numbers 
    int x, y;
    
    cout << endl << endl << "Enter two numbers, then the average of those two numbers will print." << endl;

     //user input 
    cout << "enter the first value:: ";
    cin >> x;
    cout << endl << "enter the second value:: ";
    cin >> y; 

    //calculations 
    int avg; 
    avg= (x+y)/2;

    //print result 
    cout << endl << "The average of the two numbers you entered is:: " << avg << endl; 

    //Q #3: Find the sum of the series 0,1,2..n where n is user input 
    int n;
    cout  << endl << endl << "Enter a number to determine the length of the series." << endl;
    //user input 
    cout << "enter a number:: " << endl;
    cin >> n; 

    int sum= 0;
    //calculations
    for (int i= 0; i <= n; i++)
    {
        sum= sum+ i;
    }

    //print result 
    cout << "the sum of a series going to " << n << " is " << sum << endl; 

    //Q #4: calculate the factorial of user input using a fraction 
    int a, ansFact; 
    
    cout << endl << endl << "Enter to find what the factorial of that number is." << endl;

    //user input 
    cout << "enter a number: ";
    cin >> a; 

    //calling the function 
    ansFact= factorial (a); 

    //print result 
    cout << endl << "the factorial of " << a << " is " << ansFact; 

    //Q #5: Ask for 5 user input and store in an array and print the sum of array elements 
    int array [5];
    int sumARR=0; 
    int num;
    
    cout << endl << endl << "Input an array. The sum of the array elememts will be printed." << endl; 

    for (int j= 0; j < 5; j++)
    {
        cout << "enter a number";
        cin >> array[j];
        sumARR= sumARR + array[j];
    }

    //print results 
    cout << "the sum of the elements in the array is: " << sumARR << endl;  


    return 0; 

}
