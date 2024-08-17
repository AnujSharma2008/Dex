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
