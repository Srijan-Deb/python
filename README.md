
#Assignment 1

#Takes two numbers as input from the user
#perform the basics operations

a = int(input('Enter the first number: '))
b = int(input('Enter the second number: '))

print('Addition: ',a+b)
print('Subtraction: ',a-b)
print('Multiplication :',a*b)
print('Division : ',a/b)

-----------------------------------------------------------------------------

#Assignment 2


# Task 1: Check if a Number is Even or Odd

a =int(input('Enter a number: '))
if a % 2 ==0:
    print( a, 'is an even number')
else:
    print( a, 'is an odd number')


# Task 2: Sum of integers from 1 to 50 Using a Loop
sum=0
for i in range (1,51):
    sum+=i
print('The sum of numbers from 1 to 50 is: ',sum)

--------------------------------------------------------------------------

#Assignment 3

# Task 1: Calculate Factorial using a Function

def factorial(n):
    if n<2:
        return 1
    else:
        return n * (factorial(n-1))

num = int(input("Enter a number: "))
print(f"Factorial of {num} is: {factorial(num)}")


#Task 2: Using the math module for Calculations

from math import *
num=int(input("Enter a number: "))
print(f"Square root: {math.sqrt(num)}")
print(f"Logarithm: {math.log(num)}")
print(f"sine: {math.sin(num)}")

---------------------------------------------------------------------

#Assignment 4
