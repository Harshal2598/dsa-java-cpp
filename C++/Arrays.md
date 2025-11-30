✅ Arrays in C++ (Simple Explanation)

An array in C++ is a collection of multiple values of the same data type stored in continuous memory locations.

Think of an array like a row of lockers — each locker has an index (0,1,2,…) and stores one value.

✅ Syntax of an Array
datatype arrayName[size];


Example:

int numbers[5];


This creates an integer array that stores 5 integers.

✅ Array Initialization
1️⃣ Initialize one by one
numbers[0] = 10;
numbers[1] = 20;
numbers[2] = 30;

2️⃣ Initialize at the time of declaration
int numbers[5] = {10, 20, 30, 40, 50};

3️⃣ Let compiler count size
int numbers[] = {10, 20, 30, 40};


Size becomes 4 automatically.

✅ Accessing Array Elements
cout << numbers[0];   // prints 10
cout << numbers[3];   // prints 40

✅ Looping Through an Array
int arr[5] = {1, 2, 3, 4, 5};

for (int i = 0; i < 5; i++) {
    cout << arr[i] << " ";
}

✅ Example Program
#include <iostream>
using namespace std;

int main() {
    int marks[5] = {90, 85, 76, 92, 88};

    cout << "Marks are: ";
    for (int i = 0; i < 5; i++) {
        cout << marks[i] << " ";
    }

    return 0;
}

✅ Types of Arrays
1. One-dimensional array

Like a single row.

int arr[10];

2. Two-dimensional array (matrix)

Rows × Columns.

int matrix[3][3] = {
    {1,2,3},
    {4,5,6},
    {7,8,9}
};
