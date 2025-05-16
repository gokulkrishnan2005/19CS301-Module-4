# 19CS301-Module-4
ExNo.4a DICTIONARY- SORTING IN DICTIONARY
### AIM
To write a  program for Sorting the Keys and Values in alphabetical using Dictionary  value.
### ALGORITHM

Step 1:	 Begin the program.

Step 2:	  Create an empty dictionary d.

Step 3:	 Insert key-value pairs into d.

Step 4:	 Return the dictionary d.

Step 5:	 Call the sorting() function to get the dictionary.

Step 6:  Use sorted() on d.items() with a key that sorts by value, then by key.

Step 7:  Print the sorted list of key-value tuples.

Step 8:	 Terminate the program.

### PROGRAM
```
def sorting():
    d={}
    d[5]=12
    d[1]=2
    d[6]=18
    d[3]=323
    d[2]=56
    d[4]=24
    return d
d=sorting()
print("Keys and Values sorted in alphabetical order by the value")
print(sorted(d.items(),key=lambda kv:(kv[1],kv[0])))
    
```
### OUTPUT
![image](https://github.com/gokulkrishnan2005/19CS301-Module-4/blob/main/11.png)

 
### RESULT
Thus the python program for printing a sort in dictionary, was implemented and executed successfully.

Exp.No:4(b)	EXCEPTION- EXCEPTION HANDLING
### AIM
To create a short program that accept  number of  elements from the user eg. 25,30,40 and print the element .Use index number 6 for print & add statement  "6 is not accepted" instead of index error.
### ALGORITHM

Step 1:	 Begin the program.

Step 2:	 Reads an integer n from input.

Step 3:	 Split the input_str using commas (,) to create a list of grades.

Step 4:	 Reads n integers and appends them to list a.

Step 5:	 Prints the full list a.

Step 6:	 Attempts to print the 7th element (a[6]).

Step 7:  If there’s an IndexError (because a has fewer than 7 elements) or any other error, prints "6 is not accepted".

Step 8:	 Terminate the program.
### PROGRAM
```
try:
        a = []
        n = int(input())
        for i in range(0, n):
            a.append(int(input())) 
        print(a)
        print(a[6])            
except:
        print("6 is not accepted")
```
### OUTPUT
 ![image](https://github.com/gokulkrishnan2005/19CS301-Module-4/blob/main/12.png)

### RESULT
Thus the python program for handling exceptions was implemented and executed successfully.

EXNo.4C File Handling -Count the frequency of each character in a File
### AIM
To write a Python program to read a file and count the frequency of each character in it.
### ALGORITHM

Step 1:	 Begin the program.

Step 2:	 Define the function create file  andAccept two arguments: file_path (the path to the file) and content (the string content to be written into the file).

Step 3:	 Open the file specified by file_path in write mode ('w'), Write the provided content to the file.

Step 4:	Close the file (this is done automatically when exiting the with block).

Step 5:	 Define the function character frequency,Accept one argument: file_path (the path to the file whose character frequency is to be calculated).

Step 6:	 Open the file specified by file_path in read mode ('r'), Read the content of the file into the variable content.

Step 7:	 Initialize an empty defaultdict of type int (which will store the frequency of each character).

Step 8:	 Loop through each character in the content: For each character ch, increment its corresponding frequency in the dictionary d1.

Step 9:	 Return the dictionary d1, which contains the frequency of each character in the file.

Step 10:	 Terminate the program.
### PROGRAM
```
input_str=input()
grades=input_str.split(',')
try:
    l1=[int(item) for item in grades]
except:
    print("The grades you entered were in an invalid format.")
    print(grades)
else:
    l1=[int(item) for item in grades]
    print(l1)
```
### OUTPUT

 ![image](https://github.com/user-attachments/assets/a23ca630-bc9b-439a-b4f1-fcad2a2e0711)

 
### RESULT
Thus the python program for finding character frequency count in a file, was implemented and executed successfully.

ExNo.4(d). CLASS AND OBJECTS- AREA OF CIRCLE

### AIM
To write Python Program to take the radius from the user and find the area of the circle using class name 'umbrella' and function name 'rain'
### ALGORITHM

Step 1:	 Begin the program.

Step 2:	  Create a class named umbrella.

Step 3:	 Define a method rain(self, r) that accepts a radius r as an argument.

Step 4:	 Inside the rain method: Calculate the area of a circle using the formula: Area = π * r^2. Use the math.pi constant to get the value of π and perform the calculation. Print the 
          result, formatted to two decimal places.

Step 5:	 Prompt the user for an integer input to represent the radius of the circle.

Step 6:	 Create an instance of the umbrella class and store it in the variable u.

Step 7:	 Call the rain method of the umbrella class, passing the user-provided radius r as an argument.

Step 8:	 Terminate the program.
### PROGRAM
```
import math
class umbrella:
    def rain(self,r):
        res=math.pi * r * r
        print(f"Area of circle: {res:.2f}")
r=int(input())
u=umbrella()
u.rain(r)
```
### OUTPUT
![image](https://github.com/gokulkrishnan2005/19CS301-Module-4/blob/main/13.png)

 
### RESULT
Thus the python program for calculating the area of a circle was implemented and executed successfully.

Exp.No:4(e)	SEB- KEYS AND VALUES IN DICTIONARY

### AIM
Write a Python program that asks the user to enter a text and return him a dictionary whose keys are the words of the text entered and the values are the reverse of the words that make up the text. Example for the text T = "Python is easy", the program must return the dictionary.
### ALGORITHM

Step 1:	 Begin the program.

Step 2:  Read a string s from input.

Step 3:  Split s into words.

Step 4:  For each word i, add d[i] = reversed(i).

Step 5:  Print the dictionary d.

Step 6: Terminate the program.
### PROGRAM
```
s=input()
d={}
for i in s.split():
    d[i]=i[::-1]
print("The obtained dictionary is d = ",d)
```
### OUTPUT
![image](https://github.com/gokulkrishnan2005/19CS301-Module-4/blob/main/14.png)
 
### RESULT
Thus the  dictionary whose keys are the words of the text entered and the values are the reverse of the words has been  implemented and executed successfully.




