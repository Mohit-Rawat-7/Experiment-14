# Experiment-14
## AIM-
To learn about recursion in c++.

### Problem Statement

1.) Write a c++ program to get factorial of a number using recursion.

2.) Write a c++ program to find fibonacci number in the fibonacci sequence using recursion.

3.) Write a c++ program to find sum of n natural numbers using recursion.


## THEORY-
Recursion involves a function calling itself to solve smaller instances of the same problem. This approach helps in tackling complex problems by breaking them into simpler, more manageable tasks.

Though recursion can be initially tricky to grasp, experimenting with recursive functions and understanding their base and recursive cases can provide clarity and insight into their operation and applications.

The Fibonacci series is a sequence of numbers where each number is the sum of the two preceding ones, typically starting with 0 and 1.

The natural sum refers to the sum of the first 
𝑛
n natural numbers (1, 2, 3, ..., 
𝑛
n). 

### CODE-
1)
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
2)
```javascript
//Mohit Singh Rawat
//23070123086
# include<iostream>
using namespace std;
int fib(int n)
{
    if(n==0)
    {
        return 0;
    }
    if(n==1)
    {
        return 1;
    }
    else
    {
     return (fib(n-1) + fib(n-2));
    }

}
int main()
{
    int f,n;
    cout << "Enter number of elements: "<<endl;
    cin >> n ;

    cout << n <<"th Fibonacci number in Fibonacci series is: "<<fib(n) ;
 
}
```
3)
```javascript
//Mohit Singh Rawat
//23070123086
# include<iostream>
using namespace std;
int sum(int n)
{
    if(n==0)
    {
        cout<< " Number should be greater than 1"<<endl;
    }
    if(n==1)
    {
        return 1;
    }
    else
    {
     return (n+sum(n-1));

    }
}
    int main()
{
    int f,n;
    cout << "Enter a number : "<<endl;
    cin >> n ;

    cout  <<"Sum of numbers from 1 to "<<n<<" is: "<<" : "<<sum(n) ;
 
}
```


### OUTPUT-
1)<img width="318" alt="image" src="https://github.com/user-attachments/assets/6da517cd-a2a7-4453-938d-1cad8bc5ee8e"><br>
2)<img width="417" alt="Screenshot 2024-10-11 at 9 01 29 AM" src="https://github.com/user-attachments/assets/49fe9d43-77e3-4132-9937-da42e15d74c7"><br>
3)<img width="321" alt="Screenshot 2024-10-11 at 8 54 48 AM" src="https://github.com/user-attachments/assets/e58265a4-f1e8-45b3-9787-bf582d5c60e8"><br>

## CONCLUSION-
 In conclusion, recursion is a powerful technique that simplifies complex problems by breaking them into smaller tasks through self-referential calls. While it enhances clarity in solutions like the Fibonacci series and natural sum, it can also lead to inefficiencies and stack overflow. Thus, balancing its advantages and disadvantages is essential for effective implementation.







