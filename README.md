#ASSIGNMENT 1


#Takes two numbers as input from the user,perform the basics operations

a = int(input('Enter the first number: '))
b = int(input('Enter the second number: '))

print('Addition: ',a+b)
print('Subtraction: ',a-b)
print('Multiplication :',a*b)
print('Division : ',a/b)

-----------------------------------------------------------------------------

#ASSIGNMENT 2


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

#ASSIGNMENT 3

# Task 1: Calculate Factorial using a Function

def factorial(n):
    if n<2:
        return 1
    else:
        return n * (factorial(n-1))

num = int(input("Enter a number: "))
print(f"Factorial of {num} is: {factorial(num)}")


# Task 2: Using the math module for Calculations

from math import *
num=int(input("Enter a number: "))
print(f"Square root: {math.sqrt(num)}")
print(f"Logarithm: {math.log(num)}")
print(f"sine: {math.sin(num)}")

---------------------------------------------------------------------

#ASSIGNMENT 4

 
# Task 1: Read a File and Handle Errors 

Problem Statement:  Write a Python program that:
1.   Opens and reads a text file named sample.txt.
2.   Prints its content line by line.
3.   Handles errors gracefully if the file does not exist.

#create 'sample.txt' file
Line 1: This is a sample text file.
Line 2: It contains multiple line.

#Read a file and handle errors
try:
    file1=open('sample.txt','r')
    reading_file = file1.read()
    print('Reading file content:\n',reading_file) #print its content line by line
    file1.close()
except FileExistsError():
    print(f"Error: The file '{sample.txt}' was not found")
          -----------------

 # Task 2: Write and Append Data to a File
 
Problem Statement: Write a Python program that:
1.   Takes user input and writes it to a file named output.txt.
2.   Appends additional data to the same file.
3.   Reads and displays the final content of the file.

----input----
text=input("Enter text to write to the file: ")
file1=open('output.txt','w')
write_file=file1.write(text+"\n")
print("Data Successfully written to output.txt.")

Additional_text= input("Enter additional text to append: ")
file1=open('output.txt','a')
append_file=file1.write(Additional_text+"\n")
print("Data Successfully appended.")

print("\n Final content of output.txt:")
file1=open('output.txt','r')
reading_file=file1.read()
print(reading_file)

-----------------------------------------------------------------------------

#ASSIGNMENT 5

# Task 1: Create a Dictionary of Student Marks

Problem Statement: Write a Python program that:
1.   Creates a dictionary where student names are keys and their marks are values.
2.   Asks the user to input a student's name.
3.   Retrieves and displays the corresponding marks.
4.   If the student’s name is not found, display an appropriate message.

-----INPUT-------
students={'Srijan':65,'Ayush':75,'Rijuan':68,'Alice':85}
name=input("Enter the student's name: ")
if name in students:
    print(f"{name}'s marks: {students[name]}")
else:
    print("Student not found .")

    -----------------

  #  Task 2: Demonstrate List Slicing 
    
Problem Statement: Write a Python program that:
1.   Creates a list of numbers from 1 to 10.
2.   Extracts the first five elements from the list.
3.   Reverses these extracted elements.
4.   Prints both the extracted list and the reversed list

-----INPUT-----
numbers=list(range(1,11))
print(f"Original list:{numbers}")
first_five_numbers=numbers[0:5]
print(f"Extracted first five elements: ",first_five_numbers)
first_five_numbers.reverse()
print("Reversed extracted elements: ",first_five_numbers)

-----------------------------------------------------------------------------------------------
