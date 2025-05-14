# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:
```
class EvenNumberGenerator:
    def __init__(self, start, end):
        self.start = start
        self.end = end

    def generate_even_numbers(self):
        return [num for num in range(self.start, self.end + 1) if num % 2 == 0]
even_number_generator = EvenNumberGenerator(200, 300)
even_numbers = even_number_generator.generate_even_numbers()
print("Even numbers between 200 and 300:")
print(even_numbers)
```
## OUTPUT:
```
  Input                 Result

200  3000           Even numbers between 200 and 300:
                   [200, 202, 204, 206, 208, 210, 212, 214, 216, 218, 220, 222, 224, 226, 228, 230, 232, 234, 236, 238, 240, 242, 244, 246, 248, 250, 252, 254, 
                   256, 258, 260, 262, 264, 266, 268, 270, 272, 274, 276, 278, 280, 282, 284, 286, 288, 290, 292, 294, 296, 298, 300]
```
## RESULT:
The program was successful.
