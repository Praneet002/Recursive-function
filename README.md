# Recursive-function

## Aim: To write a C# program to reverse a number using recursive function.

## Algorithm:

## Step1:
Create a function for reversing.
## Step2:
Get the number from the user.
## Step3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.
## Step4:
Recusively call this function to get the reversed number.
## Step5:
print the reversed number.

## Program:
```
python
using System;
namespace rec
{
    class Program
    {
        int rem = 0, rev = 0;
        public int reverse(int n)
        {
            rem = n % 10;
            if (rem == 0)
            {
                return rev;
            }
            else
            {
                rev = rev * 10 + rem;
                return reverse(n / 10);
            }
        }
        static void Main(string[] args)
        {
            int n;
            Console.WriteLine("Enter a Number to reverse: ");
            n = Convert.ToInt32(Console.ReadLine());
            Program p1 = new Program();
            Console.WriteLine("Reversed Number is " + p1.reverse(n));
        }
    }
}
```
## Output:
![278068294-46ca0995-899f-43c8-9098-0d92d4318492](https://github.com/Naveenvetrivel/Recursive-function/assets/94165322/4acf8ab0-17fe-4514-a63d-2c1c29df2dac)

## Result:
The C# program to reverse a number using recursive function is executed successfully.
