# Experiment-14
## AIM-
To learn about recursion in c++.

### Problem Statement

1.) Write a c++ program to get factorial of a number using recursion.
## THEORY-
Recursion involves a function calling itself to solve smaller instances of the same problem. This approach helps in tackling complex problems by breaking them into simpler, more manageable tasks.

Though recursion can be initially tricky to grasp, experimenting with recursive functions and understanding their base and recursive cases can provide clarity and insight into their operation and applications.

### CODE-
```javascript
//Mohit Rawat
//23070123086
#include<iostream>
using namespace std;

int factorial(int n);
int main() {
    int n;
    cout << "Enter a number: ";
    cin >> n;
    cout << "Factorial of " << n << " = " << factorial(n);
    return 0;
}

int factorial(int n) {
    if(n==0){
        return 1;
    } else{
        return n*factorial(n - 1);
    }
}
```
### OUTPUT-
<img width="318" alt="image" src="https://github.com/user-attachments/assets/6da517cd-a2a7-4453-938d-1cad8bc5ee8e">

## CONCLUSION-
Recursion is a powerful technique for solving complex problems by breaking them into simpler, smaller sub-problems through a function that calls itself. While it may initially seem challenging, experimenting with recursive functions and understanding their structure—comprising base and recursive cases—can enhance comprehension and reveal its utility in various problem-solving scenarios.







