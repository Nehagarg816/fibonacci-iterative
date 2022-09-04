# fibonacci-iterative
This is a program for finding fibonacci series of a number using iterative approach using functions.


#include <stdio.h>
int fib_iterative(int a);
int main()
{
    int n;
    printf("Enter the number whose fibonacci series to be calculated:");
    scanf("%d", &n);
    int s;
    s = fib_iterative(n);
    printf("Fibonacci series of entered number is %d", s);
    return 0;
}
int fib_iterative(int x)
{
    int a = 0;
    int b = 1;
    int i;
    for (i = 0; i < x; i++)
    {
        b = a + b;
        a = b - a;
    }
    return a;
}
