# Pass-by-Reference
11.Recursion

A function which calls itself is called recursion.
Eg.
#include<iostream>
using namespace std;
int factorial(int n) {
  if (n==1) {
    return 1;
  }
  else {
    return n * factorial(n-1);
  }
}
int main() {
  cout << factorial(5);
}//Output 120


12.Passing Array into Functions

void printArray ( int arr[], int size ) {
for( int x=0; x<size; x++ ) {
cout << arr[x]<< endl;
}
}
int main() {
int myArr[3]= {42, 33, 88};
printArray(myArr, 3);
}


13.Passing by Reference

Pass-by-reference copies an argument's address into the formal parameter. Inside the function, the address is used to access the actual argument used in the call. This means that changes made to the parameter affect the argument.
To pass the value by reference, argument pointers are passed to the functions just like any other value.
