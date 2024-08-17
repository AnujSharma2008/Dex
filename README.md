<h1 align="center">IP file class - XI science</h1>

# Index

| Sr No. | Name of the programme                             |
|--------|---------------------------------------------------|
| 1      | Swapping of two numbers individually.             |
| 2      | Palindrome of Numbers and Strings.                |
| 3      | Factorial of Number.                              |
| 4      | Even and Odd numbers individually.                |
| 5      | Even and Odd count in loop.                       |
| 6      | Prime Number.                                     |
| 7      | Fibonacci Series.                                 |
| 8      | Printing of a series in a fraction format.        |
| 9      | List with function.                               |
| 10     | List with function sort ascending and descending. |
| 11     | List with Delete, Drop and Remove.                |
| 12     | List with function Slice.                         |
| 13     | Vowels finding using If Else.                     |
| 14     | Calculate a building using If Else.               |
| 15     | Loop for printing Table.                          |
| 16     | Loop for printing Pyramid Pattern.                |
| 17     | Finding largest or smallest number.               |
| 18     | Calculate Simple Interest.                        |
| 19     | Calculate Average.                                |
| 20     | Calculate Sum.                                    |
| 21     | Calculate the Grade on the basis of Percentage.   |
| 22     | Calculator using If Else.                         |
---
# Page 1
### #1 Swapping of two numbers individually.
```
num1 = int(input("Enter your first number: "))
num2 = int(input("Enter your second number: "))
temp = num1
num1 = num2
num2 = temp
print("\nValue of first number:", num1, "\nValue of second number:", num2)
```
**Output**

![Test Case 1](https://i.postimg.cc/HsJGGztG/1.png)

---

# Page 2
### #2 Palindrome of Numbers and Strings.
```
string = input("Enter you word or number: ")
if isinstance(string, str):
    string = string.lower()
temp = ""
length = int(len(string))
for i in range(0,length):
    temp = string[i] + temp
if string == temp:
    print("Yes, it's a palindrome.")
else:
    print("No, it's not a palindrome.")
```
**Output**

![For String](https://i.postimg.cc/x8k9YfTv/2a.png)
![For Numbers](https://i.postimg.cc/KcVZfMJJ/2b.png)

---

# Page 3
### #3 	Factorial of Number.
```
num = int(input("Enter your number: "))
factorial = 1
for i in range(1,num + 1):
    factorial = factorial * i
if num == 0:
    print("Factorial of 0 is 1")
elif num < 0:
    print("Factorial of negative numbers not exists")
else: 
    print("Factorial of", num, "is", factorial)
```
**Output**

![Test Case 1](https://i.postimg.cc/T1mYg2MR/image.png)

---

# Page 4
### #4 	Even and Odd numbers individually.
```
num = int(input("Enter your number: "))
if num % 2 == 0:
    print(num, "is an even number.")
else:
    print(num, "is an odd number.")
```
**Output**

![Test Case 1](https://i.postimg.cc/P579sW-vR/4.png)
