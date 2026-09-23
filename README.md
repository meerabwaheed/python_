print("it's my first Dsa lab")
# 2. Variables
name = "John"
age = 25
print("Name:", name)
print("Age:", age)
# Taking User Input
name = input("Enter your name: ")
print("Hello", name)
a = 10
b = 30
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

marks = array('i', [78, 85, 92, 67, 88])

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
