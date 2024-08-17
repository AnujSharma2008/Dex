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

```
Enter your first number: 
100
Enter your second number: 
200

Value of first number: 200 
Value of second number: 100


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

---

# Page 2
### #2 Palindrome of Numbers and Strings.
```
string = input("Enter your word or number: ")
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

**Test Case - 1**
```
Enter you word or number: 
Racecar
Yes, it's a palindrome.


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
**Test Case - 2**
```
Enter you word or number: 
Racecar
Yes, it's a palindrome.


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

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

```
Enter your number: 
5
Factorial of 5 is 120


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

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

**Test Case - 1**
```
Enter your number: 
7
7 is an odd number.


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
**Test Case - 2**
```
Enter your number: 
154
154 is an even number.


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```


# Page 5
### #5 	Even and Odd count in loop.
```
num = int(input("Enter a number: "))
count_even = 0
count_odd = 0
for i in range(1, num + 1):
    if i % 2 == 0:
        count_even += 1
    else:
        count_odd += 1
print("Even numbers:", count_even)
print("Odd numbers:", count_odd)
```
**Output**

```
Enter a number: 
138
Even numbers: 69
Odd numbers: 69


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

# Page 6
### #6 	Prime Number.
```
num = int(input("Enter your number: "))
if num == 1:
    print(num, "is not a prime number.")
else:
    for i in range(2, (num//2)+1):
        if (num % i) == 0:
            print(num, "is not a prime number.")
            break
    else:
        print(num, "is a prime number.")
```
**Output**

**Test Case - 1**
```
Enter your number: 
101
101 is a prime number.


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
**Test Case - 2**
```
Enter your number: 
54
54 is not a prime number.


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 7
### #7 	Fibonacci Series.
```
num = int(input("Enter the digit"))
x = 0
y = 1
print(x)
print(y)
for i in range(1,num):
    z = x + y
    print(z)
    x,y = y,z
```
**Output**

```
Enter the digit
12

0
1
1
2
3
5
8
13
21
34
55
89
144


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 8
### #8 	Printing of a series in a fraction format.
```
from fractions import Fraction
num = int(input("Enter your number: "))
for i in range(1, num + 1):
    print(Fraction(i, num))
```
**Output**

```
Enter your number: 
5

1/5
2/5
3/5
4/5
1


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 9
### #9 	List with function.
```
import random
pokemon = []
poke_inp = input("Enter Pokémon names separated by spaces: ").split()
pokemon.extend(poke_inp)
poke_rnd = random.choice(pokemon)
print("The random pokemon selected is", poke_rnd)
```
**Output**

```
Enter Pokémon names separated by spaces: 
Pikachu Charizard Calyrex Mewtwo Arceus
The random pokemon selected is Charizard


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 10
### #10 List with function sort ascending and descending.
```
num = []
num_inp = input("Enter numbers separated by spaces: ").split()
for i in num_inp:
    num.append(int(i))
num.sort()
print("Numbers in ascending order", num)
num.sort(reverse=True)
print("Numbers in descending order", num)
```
**Output**

```
Enter numbers separated by spaces: 
69 54 78 25 46 86 66 7 458
Numbers in ascending order [7, 25, 46, 54, 66, 69, 78, 86, 458]
Numbers in descending order [458, 86, 78, 69, 66, 54, 46, 25, 7]


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 11
### #11 List with Delete, Drop and Remove.
```
list1 = ["apple", "banana", "cherry"]
print("Original List: ",list1)
remove = input("Enter a value to remove :")
list1.remove(remove)
print("Updated List: ",list1)
delete = int(input("Enter a index to delete"))
del list1[delete]
print("Updated List: ",list1)
```
**Output**

```
Original List:  ['apple', 'banana', 'cherry']
Enter a value to remove :
banana
Updated List:  ['apple', 'cherry']
Enter a index to delete
1
Updated List:  ['apple']


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 12
### #12 List with Slice.
```
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
slice_index = input("Enter a ratio for slicing :").split()
print(numbers[int(slice_index[0]):int(slice_index[1])])
```
**Output**

```
Enter a ratio for slicing :
3 7
[4, 5, 6, 7]


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 13
### #13 Vowels finding using If Else.
```
word = input("Enter a word: ")
vowels = ''
if 'a' in word.lower():
    vowels += 'a '
if 'e' in word.lower():
    vowels += 'e '
if 'i' in word.lower():
    vowels += 'i '
if 'o' in word.lower():
    vowels += 'o '
if 'u' in word.lower():
    vowels += 'u '
if vowels:
    print("The word contains vowels:", vowels)
else:
    print("The word does not contain vowels.")
```
**Output**

```
Enter a word: 
anuj sharma
The word contains vowels: a u 


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 14
### #14 Calculate a building using If Else.

Leave a page for it.

# Page 15
### #15 Loop for printing Table.
```
num = int(input("Enter your number: "))
for i in range(1, 11):
    print(f"{num} * {i} = {num*i}")
```
**Output**

```
Enter your number: 
16
16 * 1 = 16
16 * 2 = 32
16 * 3 = 48
16 * 4 = 64
16 * 5 = 80
16 * 6 = 96
16 * 7 = 112
16 * 8 = 128
16 * 9 = 144
16 * 10 = 160


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 16
### #16 Loop for printing Pyramid Pattern.
```
num = int(input("Enter your number: "))
for i in range(1, num + 1):
    print(i*"*")
```
**Output**

```
Enter your number: 
5
O 
O O 
O O O 
O O O O 
O O O O O 


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
# Page 17
### #17 Finding largest or smallest number.
```
numbers = [12, 45, 7, 23, 56, 89, 34]
largest = numbers[0]
smallest = numbers[0]
for num in numbers:
    if num > largest:
        largest = num
    elif num < smallest:
        smallest = num
print(f"Largest number: {largest}")
print(f"Smallest number: {smallest}")
```
**Output**

```
Largest number: 89
Smallest number: 7


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

# Page 18
### #18 Calculate Simple Interest.
```
principal = float(input("Enter the principal amount: "))
rate = float(input("Enter the interest rate (in %): "))
time = float(input("Enter the time period (in years): "))
si = (principal * rate * time) / 100
print(f"The simple interest is: {si:.2f}")
```
**Output**

```
Enter the principal amount: 
50
Enter the interest rate (in %): 
100
Enter the time period (in years): 
2
The simple interest is: 100.00


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

# Page 19
### #19 Calculate Average.
```
numbers = [10, 20, 30, 40, 50]
add = 0
size = 0
for i in numbers:
    add += i
    size += 1
avg = add / size
print(f"The average is: {avg:.2f}")
```
**Output**

```
The average is: 30.00


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

# Page 20
### #20 Calculate Sum.
```
numbers = [100, 250, 32540, 4450, 9820]
add = 0
size = 0
for i in numbers:
    add += i
print(f"The addition is: {add}")
```
**Output**

```
The addition is: 47160


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

# Page 21
### #21 Calculate the Grade on the basis of Percentage.
```
percentage = float(input("Enter the percentage: "))

if percentage >= 95:
    grade = "A+"
elif percentage >= 90:
    grade = "A"
elif percentage >= 85:
    grade = "B+"
elif percentage >= 80:
    grade = "B"
elif percentage >= 75:
    grade = "C+"
elif percentage >= 70:
    grade = "C"
elif percentage >= 65:
    grade = "D+"
elif percentage >= 60:
    grade = "D"
elif percentage >= 55:
    grade = "E+"
elif percentage >= 50:
    grade = "E"
else:
    grade = "F"

print(f"Grade: {grade}")
```
**Output**

```
Enter the percentage: 
80.2
Grade: B


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

# Page 22
### #22 Calculator using If Else.
```
print("Simple Calculator")
print("1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Division")

choice = int(input("Enter your choice (1/2/3/4): "))

if choice == 1:
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    result = num1 + num2
    print("Result: ", result)

elif choice == 2:
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    result = num1 - num2
    print("Result: ", result)

elif choice == 3:
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    result = num1 * num2
    print("Result: ", result)

elif choice == 4:
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    if num2 != 0:
        result = num1 / num2
        print("Result: ", result)
    else:
        print("Error! Division by zero is not allowed.")

else:
    print("Invalid choice. Please choose a valid option.")
```
**Output**

```
Simple Calculator
1. Addition
2. Subtraction
3. Multiplication
4. Division
Enter your choice (1/2/3/4): 
2
Enter first number: 
1.5
Enter second number: 
6.5
Result:  -5.0


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```
## ❤️ Like my github!! :)
