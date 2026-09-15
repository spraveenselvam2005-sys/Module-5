# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
```
class pen:
    def __init__(self,a,b,c):
        self.a=a
        self.b=b
        self.c=c
    def show(self):
        print(f"{self.a} {self.b} {self.c}")

a=input()
b=int(input())
c=int(input())
ob=pen(a,b,c)
ob.show()
```

## Sample Output
<img width="1414" height="506" alt="image" src="https://github.com/user-attachments/assets/9db6f5a0-cfcb-4e0c-a5c0-c608ada671ba" />

## Result
The program is successfully excexuted
