# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
      class Demo:
          def __init__(self):
              print("Alive")
          def __del__(self):
              print("The object no longer exists")
              
      obj = Demo()
      del obj

## 🧪 Output
![image](https://github.com/user-attachments/assets/0c1c3edc-b1ef-4b9a-bac7-644be47d2f49)


## Result
Thus, the program has been execueted successfully.

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
    class Details:
        def __init__(self):
            self.__id="<No Id>"
            self.__name="<No Name>"
            self.__gender="<No Gender>"
        def setData(self,id,name,gender):
            self.__id=id
            self.__name=name
            self.__gender=gender
        def showData(self):
            print("Id: ",self.__id)
            print("Name: ",self.__name)
            print("Gender: ",self.__gender)
            
    class Employee(Details):
        def __init__(self):
            self.__company="<No Company>"
            self.__dept="<No Dept>"
        def setEmployee(self,id,name,gender,comp,dept):
            self.setData(id,name,gender)
            self.__company=comp
            self.__dept=dept
        def showEmployee(self):
            self.showData()
            print("Company: ",self.__company)
            print("Department: ",self.__dept)
    class Patient(Details):
        def __init__(self):
            self.__hospital="<No Hospital>"
            self.__dept="<No Dept>"
        def setEmployee(self,id,name,gender,hos,dept):
            self.setData(id,name,gender)
            self.__hospital=hos
            self.__dept=dept 
        def showEmployee(self):
            self.showData()
            print("Hospital: ",self.__hospital)
            print("Department: ",self.__dept) 
            
    id=int(input())
    name=input()
    gender=input()
    comp=input()
    dept=input()
    id1=int(input())
    nam=input()
    gen=input()
    hos=input()
    dep=input()
    
    print("Employee Object")
    e=Employee()
    e.setEmployee(id,name,gender,comp,dept)
    e.showEmployee()
    print("\nPatient Object")
    d=Patient()
    d.setEmployee(id1,nam,gen,hos,dep)
    d.showEmployee() 
    
## Sample Output
![image](https://github.com/user-attachments/assets/64338166-fcad-4459-86cf-ba8d9cf31d80)


## Result
Thus, the program has been execueted successfully.


