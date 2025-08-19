# Classes-and-Objects-in-C-Plus-Plus

# 📘 Classes and Objects in C++

## 🔹 Overview
In C++, **classes and objects** are the core concepts of **Object-Oriented Programming (OOP)**.  
- A **class** is a blueprint or template that defines properties (data members) and behaviors (member functions).  
- An **object** is an instance of a class, created from that blueprint.  

They help in **encapsulation**, **reusability**, and **real-world modeling** in programming.

---

## 🔹 Theory

### 1. Class
- Defined using the keyword `class`.  
- Contains **attributes** (variables) and **methods** (functions).  
- By default, members of a class are **private**, meaning they cannot be accessed outside the class unless specified.

**Syntax:**
```cpp
class ClassName {
public:           // access specifier
    int data;     // attribute (data member)
    void display() {  // method (member function)
        cout << "Data: " << data << endl;
    }
};
```

### 🔹 1. What is an Object?
- An **object** is a **variable** of a class type.  
- It represents a specific entity created from a class.  
- Multiple objects can be created from a single class, each having its own separate data.

**Example:**
```cpp
class Car {
public:
    string brand;
    int speed;
};
```

##  Key Points

###  Classes
- A **class** is a blueprint or template for creating objects.  
- Groups **data members (variables)** and **member functions (methods)** together.  
- Supports **encapsulation** and **abstraction**.  
- Declared using the `class` keyword.  
- Can include **public, private, and protected** access specifiers.  
- Can also have **constructors** and **destructors** for object initialization and cleanup.  

###  Objects
- An **object** is an **instance of a class**.  
- Each object has its **own copy** of non-static data members.  
- **Static members** are shared across all objects of a class.  
- Access members using:
  - `.` (dot operator) for normal objects.  
  - `->` (arrow operator) for object pointers.  
- Objects represent **real-world entities** like Car, Student, Employee, etc.  

---

##  Conclusion
- **Classes** define the **structure** and **behavior** (data + functions).  
- **Objects** are the actual entities created from classes that hold specific values.  
- Together, classes and objects form the **foundation of Object-Oriented Programming (OOP) in C++**.  
- They make code more **organized, modular, reusable, and easy to maintain**.
