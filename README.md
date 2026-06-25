# Python DSA Practice Problems (Basic to Intermediate)

This document contains beginner to intermediate Data Structures and Algorithms (DSA) problems focused on:

- Lists
- Strings
- Dictionaries

Each problem contains:
- Problem Statement
- Sample Input
- Sample Output
- Explanation
- Logic Hint

---

# List Problems

## Problem 1: Find the Largest Number

### Problem

Given a list of integers, find the largest element.

### Sample Input

```text
5
12 45 3 89 21
```

### Sample Output

```text
89
```

### Explanation

The largest number among all elements is **89**.

### Logic

- Assume the first element is the largest.
- Traverse the list.
- If a larger element is found, update the maximum.
- Print the maximum.

---

## Problem 2: Find the Second Largest Number

### Problem

Find the second largest unique number in a list.

### Sample Input

```text
6
10 20 50 40 50 30
```

### Sample Output

```text
40
```

### Explanation

The largest unique number is 50.

The second largest unique number is 40.

### Logic

- Remove duplicate values.
- Sort the list.
- Return the second last element.

---

## Problem 3: Reverse a List

### Problem

Reverse the given list.

### Sample Input

```text
5
1 2 3 4 5
```

### Sample Output

```text
5 4 3 2 1
```

### Explanation

The list is printed in reverse order.

### Logic

- Use two pointers or reverse iteration.
- Swap first and last elements until the middle.

---

## Problem 4: Remove Duplicate Elements

### Problem

Remove duplicate values while maintaining the original order.

### Sample Input

```text
8
1 2 2 3 4 3 5 1
```

### Sample Output

```text
1 2 3 4 5
```

### Explanation

Duplicate elements are removed without changing the first occurrence order.

### Logic

- Create an empty result list.
- Traverse the list.
- Add an element only if it has not been seen before.

---

## Problem 5: Rotate List Left by K Positions

### Problem

Rotate the list to the left by K positions.

### Sample Input

```text
5
1 2 3 4 5
2
```

### Sample Output

```text
3 4 5 1 2
```

### Explanation

After rotating left twice, the first two elements move to the end.

### Logic

- Split the list into two parts.
- Join the second part with the first part.

---

## Problem 6: Find Missing Number

### Problem

Numbers from 1 to N are given except one. Find the missing number.

### Sample Input

```text
5
1 2 4 5
```

### Sample Output

```text
3
```

### Explanation

The numbers should be 1,2,3,4,5.

Number 3 is missing.

### Logic

- Calculate expected sum using

```
N × (N + 1) / 2
```

- Subtract the actual sum.

---

## Problem 7: Count Even and Odd Numbers

### Problem

Count how many even and odd numbers exist in the list.

### Sample Input

```text
6
2 5 8 9 11 14
```

### Sample Output

```text
Even = 3
Odd = 3
```

### Explanation

Even numbers are 2,8,14.

Odd numbers are 5,9,11.

### Logic

Traverse the list and check

```
number % 2
```

---

## Problem 8: Merge Two Sorted Lists

### Problem

Merge two already sorted lists into one sorted list.

### Sample Input

```text
List1
1 3 5

List2
2 4 6
```

### Sample Output

```text
1 2 3 4 5 6
```

### Explanation

The final merged list remains sorted.

### Logic

Use two pointers and compare current elements.

---

# String Problems

## Problem 9: Reverse a String

### Problem

Reverse the given string.

### Sample Input

```text
Python
```

### Sample Output

```text
nohtyP
```

### Explanation

Characters appear in reverse order.

### Logic

Traverse from the last character to the first.

---

## Problem 10: Count Vowels

### Problem

Count the number of vowels in a string.

### Sample Input

```text
OpenAI
```

### Sample Output

```text
4
```

### Explanation

Vowels are

```
O
e
A
I
```

### Logic

Check whether each character belongs to

```
aeiouAEIOU
```

---

## Problem 11: Check Palindrome

### Problem

Determine whether the given string is a palindrome.

### Sample Input

```text
madam
```

### Sample Output

```text
Palindrome
```

### Explanation

The string reads the same from both directions.

### Logic

Compare the string with its reverse.

---

## Problem 12: Count Character Frequency

### Problem

Print how many times each character appears.

### Sample Input

```text
banana
```

### Sample Output

```text
b : 1
a : 3
n : 2
```

### Explanation

Each character's occurrence is counted.

### Logic

Use a dictionary.

Increase the count every time the character appears.

---

## Problem 13: Remove Spaces

### Problem

Remove all spaces from the given string.

### Sample Input

```text
Hello World Python
```

### Sample Output

```text
HelloWorldPython
```

### Explanation

Only whitespace is removed.

### Logic

Traverse every character.

Skip spaces while building the result.

---

## Problem 14: Find First Non-Repeating Character

### Problem

Find the first character that appears only once.

### Sample Input

```text
swiss
```

### Sample Output

```text
w
```

### Explanation

Character frequencies:

```
s = 3
w = 1
i = 1
```

The first unique character is **w**.

### Logic

- Count frequencies.
- Traverse again.
- Return the first frequency equal to one.

---

## Problem 15: Check Anagram

### Problem

Determine whether two strings are anagrams.

### Sample Input

```text
listen
silent
```

### Sample Output

```text
Yes
```

### Explanation

Both words contain exactly the same characters.

### Logic

Sort both strings and compare.

---

## Problem 16: Capitalize First Letter of Every Word

### Problem

Convert every word so its first letter becomes uppercase.

### Sample Input

```text
python is awesome
```

### Sample Output

```text
Python Is Awesome
```

### Explanation

Only the first letter of every word is capitalized.

### Logic

Split the sentence into words.

Capitalize each word.

Join them back.

---

# Dictionary Problems

## Problem 17: Count Word Frequency

### Problem

Count how many times every word appears.

### Sample Input

```text
apple mango apple orange mango apple
```

### Sample Output

```text
apple : 3
mango : 2
orange : 1
```

### Explanation

Each word's frequency is stored.

### Logic

Split the sentence into words.

Use a dictionary to count occurrences.

---

## Problem 18: Student Marks Lookup

### Problem

Given student names and marks, print the marks of a requested student.

### Sample Input

```text
Rahul 80
Amit 90
Riya 75

Search:
Amit
```

### Sample Output

```text
90
```

### Explanation

The dictionary stores student names as keys.

### Logic

Store

```
{name : marks}
```

Retrieve using the key.

---

## Problem 19: Merge Two Dictionaries

### Problem

Merge two dictionaries.

### Sample Input

```text
{'a':1,'b':2}

{'c':3,'d':4}
```

### Sample Output

```text
{'a':1,'b':2,'c':3,'d':4}
```

### Explanation

Both dictionaries are combined into one.

### Logic

Copy one dictionary.

Insert all key-value pairs from the second dictionary.

---

## Problem 20: Find Key with Maximum Value

### Problem

Find the key whose value is the largest.

### Sample Input

```text
{
'Alice':80,
'Bob':95,
'John':88
}
```

### Sample Output

```text
Bob
```

### Explanation

Bob has the highest score.

### Logic

Track the maximum value while traversing the dictionary.

---

## Problem 21: Invert a Dictionary

### Problem

Swap dictionary keys and values.

### Sample Input

```text
{
'a':1,
'b':2,
'c':3
}
```

### Sample Output

```text
{
1:'a',
2:'b',
3:'c'
}
```

### Explanation

Keys become values and values become keys.

### Logic

Create a new dictionary.

Insert

```
new[value] = key
```

---

## Problem 22: Group Words by First Letter

### Problem

Group words according to their first character.

### Sample Input

```text
apple
ant
banana
ball
cat
```

### Sample Output

```text
a : apple ant

b : banana ball

c : cat
```

### Explanation

Words beginning with the same letter are grouped together.

### Logic

Use the first character as the dictionary key.

Append words into a list.

---

# Challenge Problems (Intermediate)

## Problem 23: Rotate String

### Problem

Determine whether one string is a rotation of another.

### Sample Input

```text
ABCD

CDAB
```

### Sample Output

```text
Yes
```

### Explanation

Rotating "ABCD" left twice produces "CDAB".

### Logic

Append the original string to itself.

If the second string is a substring, it is a valid rotation.

---

## Problem 24: Find Common Elements Between Two Lists

### Sample Input

```text
1 2 3 4 5

3 4 5 6 7
```

### Sample Output

```text
3 4 5
```

### Explanation

Only these values appear in both lists.

### Logic

Convert one list into a set or dictionary for fast lookup.

---

## Problem 25: Most Frequent Element

### Problem

Find the element that occurs the maximum number of times.

### Sample Input

```text
1 2 2 3 3 3 4
```

### Sample Output

```text
3
```

### Explanation

Number 3 appears three times.

### Logic

Count occurrences using a dictionary.

Track the highest frequency.

---