# 🧮 SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the **Insertion Sort algorithm** using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

## 🎯 Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the **Insertion Sort** algorithm
- Display the sorted list

---

## 🧠 Algorithm

1. **Start the program**
2. **Define a class** `InsertionSorter`
3. Inside the class:
   - `create_list()`:
     - Read number of elements
     - Store them in a list
   - `insertion_sort()`:
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - `print_list()`:
     - Print the sorted list
4. **Create an object** of the class
5. **Call** the methods in order: `create_list()`, `insertion_sort()`, and `print_list()`
6. **End the program**

---

## 💻 PROGRAM:
```
class IntegerList:
    def __init__(self):
        self.numbers = []

    def create_list(self):
        elements = input("Enter integers separated by spaces: ")
        self.numbers = list(map(int, elements.split()))

    def insertion_sort(self):
        for i in range(1, len(self.numbers)):
            key = self.numbers[i]
            j = i - 1
            while j >= 0 and self.numbers[j] > key:
                self.numbers[j + 1] = self.numbers[j]
                j -= 1
            self.numbers[j + 1] = key

    def display_list(self):
        print("Sorted List:", self.numbers)
obj = IntegerList()
obj.create_list()
obj.insertion_sort()
obj.display_list()
```
## OUTPUT:
```
Input                    Result
 [5 2 9 1 6]           Sorted List: [1, 2, 5, 6, 9]
```
## RESULT:
The program was successful.
