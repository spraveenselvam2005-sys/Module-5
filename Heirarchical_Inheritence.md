# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
```
class Details:
def __init__(self, name, age):
self.name = name
self.age = age
def getName(self):
return self.name
def getAge(self):
return self.age
class Employee(Details):
def __init__(self, name, age, employee_id, department):
super().__init__(name, age)
self.employee_id = employee_id
self.department = department
def getEmployeeDetails(self):
print("Employee Information:")
print("Name:", self.getName())
print("Age:", self.getAge())
print("Employee ID:", self.employee_id)
print("Department:", self.department)
class Patient(Details):
def __init__(self, name, age, patient_id, disease):
super().__init__(name, age)
self.patient_id = patient_id
self.disease = disease
def getPatientDetails(self):
print("Patient Information:")
print("Name:", self.getName())
print("Age:", self.getAge())
print("Patient ID:", self.patient_id)
print("Disease:", self.disease)
emp_name = input()
emp_age = int(input())
emp_id = input()
emp_dept = input()
employee = Employee(emp_name, emp_age, emp_id, emp_dept)
11/20/25, 6:12 PM Module-5/Heirarchical_Inheritence.md at main · kirupa169/Module-5
https://github.com/kirupa169/Module-5/blob/main/Heirarchical_Inheritence.md 2/3
The program is successfully excexuted
pat_name = input()
pat_age = int(input())
pat_id = input()
pat_disease = input()
patient = Patient(pat_name, pat_age, pat_id, pat_disease)
employee.getEmployeeDetails()
patient.getPatientDetails()
```
## Sample Output
<img width="1379" height="1087" alt="image" src="https://github.com/user-attachments/assets/a6e31465-0e34-45a5-80d1-dc302302361a" />

## Result
The program is successfully excexuted
