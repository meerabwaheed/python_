print("it's my first Dsa lab")
# 2. Variables
name = "John"
age = 27
print("Name:", name)
print("Age:", age)
# Taking User Input
name = input("Enter your name: ")
print("Hello", name)
a = 10
b = 20
sum = a + b
print("Sum =", sum)
students = ["Ali", "Sara", "Ahmed", "Ayesha"]

print(students)
print(students[0])
data = ["Ali", 20, 3.5, True]

print(data)

students = ["Ali", "Sara", "Ahmed"]

students.append("Ayesha")

print("Students:", students)


from array import array

marks = array('i', [88, 85, 92, 67, 88])

print(marks)
print(marks[0])

from array import array

marks = array('i', [78, 85, 92, 67, 88])

total = sum(marks)
average = total / len(marks)

print("Total Marks:", total)
print("Average Marks:", average)

from collections import deque

queue = deque()

queue.append("Ali")
queue.append("Sara")
queue.append("Ahmed")

print(queue)
print("Removed:", queue.popleft())
print(queue)

import heapq

numbers = [30, 10, 20, 5, 40]

heapq.heapify(numbers)

print("Smallest:", heapq.heappop(numbers))
print("Heap:", numbers)


from array import array

numbers = array('i', [10, 20, 30, 40])

numbers.append(50)

print(numbers)

import math

number = 25

print("Square root:", math.sqrt(number))
print("Power:", math.pow(2, 3))

import random

numbers = []

for i in range(5):
    numbers.append(random.randint(1, 100))

print("Random numbers:", numbers)

import bisect

numbers = [10, 20, 30, 40]

position = bisect.bisect(numbers, 25)

print("Insertion position:", position)
import itertools

items = ["A", "B", "C"]

result = list(itertools.permutations(items))

print(result)
import numpy as np

numbers = np.array([10, 20, 30, 40, 50])

print("Array:", numbers)
print("Sum:", np.sum(numbers))
print("Maximum:", np.max(numbers))
# class Student:
#     """A class to represent a student and manage their basic academic information."""

#     def __init__(self, name, roll_no, department, sem):
#         self.name = name
#         self.roll_no = roll_no
#         self.department = department
#         self.sem = sem

#     def id_card(self):
#         return (
#             f"Name: {self.name}\n"
#             f"Roll no: {self.roll_no}\n"
#             f"Department: {self.department}\n"
#             f"Semester: {self.sem}\n"
#         )

#     def display(self):
#         print(self.name)
#         print(self.roll_no)
#         print(self.department)
#         print(self.sem)


# # Create student object
# student1 = Student("Meerab Waheed", "BSCS-123", "Computer Science", 3)

# # Display student information
# student1.display()

# # Display ID card
# print("\nID Card:")
# print(student1.id_card())

# class Student:
#     def __init__(self, name, roll_no, marks):
#         self.name = name
#         self.roll_no = roll_no
#         self.marks = marks

#     def additional_marks(self, additional_marks):
#         self.marks += additional_marks
#         print(f"Total marks of student {self.name} is {self.marks}")

#     def get_marks(self):
#         return self.marks

#     def calculating_grade(self):
#         # Validate marks range first
#         if self.marks < 0 or self.marks > 100:
#             print("Invalid marks")
#         elif self.marks >= 80:
#             print("A")
#         elif self.marks >= 70:
#             print("B")
#         elif self.marks >= 60:
#             print("C")
#         elif self.marks >= 50:
#             print("D")
#         else:
#             print("F")


# # Creating instance and calling methods
# S1 = Student("meerab", 2, 80)

# S1.additional_marks(10)   # Updates marks from 80 to 90
# S1.calculating_grade()    # Prints "A" because marks are 90

# class BankAccount:
#     def __init__(self, title, balance=0.0):
#         self.title = title
#         self.balance = float(balance)

#     def deposit(self, amount):
#         if amount <= 0:
#             raise ValueError("Pesa do")
#         self.balance += amount

#     def withdraw(self, amount):
#         if amount <= 0:
#             raise ValueError("Withdraw must be positive bhai")
#         if amount > self.balance:
#             raise ValueError("Kum Balance")
#         self.balance -= amount


# # Creating object and testing methods
# account = BankAccount("Ali", 1000)

# try:
#     account.deposit(500)
#     account.withdraw(300)
#     print("Balance:", account.balance)

# except ValueError as err:
#     print("Error:", err)


def linear_search(arr, key):
    # Iterate through the array
    for i in range(len(arr)):
        # Check if the current element matches the key
        if arr[i] == key:
            return i

    # Return -1 if key is not found
    return -1


# Define array and search key
names = ['Meerab', 'Mahad', 'Balach', 'Faran']
search_key = 'Meerab'


# Call linear_search function
result = linear_search(names, search_key)


# Display result
if result != -1:
    print(f"Key '{search_key}' found at index {result}.")
else:
    print(f"Key '{search_key}' not found in the list.")
stackb = []
stackb.append(10)
stackb.append(20)
stackb.append(30)
stackb.append(40)
print("ahmed bhai k passs stackb ki value:", stackb)
index = stackb.index(10)
print("Index of 10 in stackb =", index)
