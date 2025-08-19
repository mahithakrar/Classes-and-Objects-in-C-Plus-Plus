# Classes-and-Objects-in-C-Plus-Plus

#  Classes and Objects in C++

##  Overview
In C++, **classes and objects** are the core concepts of **Object-Oriented Programming (OOP)**.  
- A **class** is a blueprint or template that defines properties (data members) and behaviors (member functions).  
- An **object** is an instance of a class, created from that blueprint.  

They help in **encapsulation**, **reusability**, and **real-world modeling** in programming.

---

##  Theory

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

#  Access Specifiers in C++

---

##  Theory

Access specifiers in C++ define the **scope and visibility** of class members (variables and functions).  
They control how data and functions inside a class can be accessed from outside the class.  
This is a crucial feature of **Encapsulation** in Object-Oriented Programming.  

There are **three main access specifiers** in C++:

---

### 1. **Public**
- Members declared as `public` are **accessible from anywhere** in the program.  
- They can be accessed both **inside** and **outside** the class.  
- Often used for functions that define the **interface** of the class.  

```cpp
class Student {
public:
    string name;
    void display() {
        cout << "Name: " << name;
    }
};
```

#  Private Access Specifier in C++

##  Theory

In C++, when a class member is declared as **private**, it can only be accessed **within the class itself**.  
It **cannot** be accessed directly from outside the class or by objects of the class.  

By default, if no access specifier is mentioned inside a **class**, the members are treated as **private**.  

The main purpose of `private` is **data hiding** and **encapsulation** — ensuring sensitive data cannot be accessed or modified directly.

---

#  Protected Access Specifier in C++

---

##  Theory

In C++, the **protected** access specifier is similar to **private** but with one key difference:  
- Protected members **cannot be accessed** directly from outside the class.  
- However, they **can be accessed in derived (child) classes** through inheritance.  

This makes `protected` useful when we want to allow access to data members by derived classes but still keep them hidden from outside the class.  

---

# 1. Student Class Program in C++

##  Theory
This program demonstrates the use of **classes and objects** in C++.  
- A class `Student` is defined with data members like `name`, `branch`, `subject`, `year`, and `result`.  
- Two objects `s1` and `s2` are created to store and display the details of different students.  
- This highlights how **objects act as real-world entities** and can hold **independent values** for the same class structure.  

---

##  Algorithm
1. Start the program.  
2. Define a class `Student` with public members: `name`, `branch`, `subject`, `year`, and `result`.  
3. In the `main()` function:  
   - Create object `s1` of class `Student`.  
   - Assign values to its members (`name`, `branch`, `subject`, `year`, `result`).  
   - Print the values.  
4. Create another object `s2` of class `Student`.  
   - Assign values to its members.  
   - Print the values.  
5. End the program.  

---

# 2. Car Class Program in C++

##  Theory
This program demonstrates the use of **classes and objects** in C++ for managing car information.  
- A class `Car` is defined with members like `member`, `name`, `brand`, `price`, and `year`.  
- Two objects `c1` and `c2` are created, and data is input by the user for each car.  
- Finally, the entered details are displayed on the screen.  

This shows how **objects store separate sets of data**, even though they are created from the same class.  

---

##  Algorithm
1. Start the program.  
2. Define a class `Car` with public members: `member`, `name`, `brand`, `price`, and `year`.  
3. In the `main()` function:  
   - Create object `c1` of class `Car`.  
   - Ask the user to input details (`member`, `name`, `brand`, `price`, `year`).  
   - Print the details of `c1`.  
4. Create another object `c2` of class `Car`.  
   - Ask the user to input details for `c2`.  
   - Print the details of `c2`.  
5. End the program.  

---

# 3. Rectangle Class Program in C++

##  Theory
This program demonstrates the concept of **classes, objects, and member functions** in C++.  
- A class `rectangle` is defined with attributes `length` and `width`.  
- A member function `area()` calculates the area of the rectangle.  
- The program checks if the rectangle is a **square** (when length = width).  
- Otherwise, it calculates and displays the area.  

This illustrates **object-oriented programming (OOP)** concepts like **encapsulation** and **methods inside a class**.  

---

##  Algorithm
1. Start the program.  
2. Define a class `rectangle` with members:  
   - `length`, `width`  
   - function `area()` to compute `length * width`.  
3. In the `main()` function:  
   - Create an object `r1` of class `rectangle`.  
   - Input `length` and `width`.  
   - If `length == width`, print "It is a square".  
   - Otherwise, call the `area()` function.  
4. End the program.  

---

# 4. Volume Calculation using Classes in C++

##  Theory
This program demonstrates how to define **member functions inside and outside a class** in C++.  
- A class `MyClass` is created with attributes: `height`, `width`, and `length`.  
- It has two functions to calculate the volume:  
  - `Volume()` → defined **inside the class**.  
  - `myVolume()` → defined **outside the class** using the scope resolution operator `::`.  
- Both functions calculate the volume of a cuboid as `height * width * length`.  

This shows the flexibility of defining class functions in multiple ways.  

---

##  Algorithm
1. Start the program.  
2. Define a class `MyClass` with:  
   - Data members: `height = 20`, `width = 6`, `length = 15`.  
   - Function `Volume()` → calculates volume inside the class.  
   - Function `myVolume()` → declared inside, but defined outside the class.  
3. In `main()`:  
   - Create an object `M1`.  
   - Call `M1.Volume()` → prints volume.  
   - Call `M1.myVolume()` → prints volume again.  
4. End program.  

---

# 5. Calculator Program using Classes in C++

##  Theory
This program demonstrates the use of **classes and objects** in C++ to implement a simple calculator.  

- A class `Calculator` is created with two data members `a` and `b`.  
- The class contains member functions to perform:  
  - Addition  
  - Subtraction  
  - Multiplication  
  - Division  
- An object `c1` of the class is created in `main()`, which takes user input for two numbers and performs all operations.

This showcases **object-oriented programming (OOP)** principles where **data (a, b)** and **operations (methods)** are encapsulated inside a class.  

---

##  Algorithm
1. Start the program.  
2. Define a class `Calculator` with two float variables `a` and `b`.  
3. Create member functions for addition, subtraction, multiplication, and division.  
4. In the `main()` function:  
   - Create an object `c1` of class `Calculator`.  
   - Take user input for two numbers.  
   - Call all four functions (`addition()`, `subtraction()`, `multiplication()`, `division()`).  
5. Display the results.  
6. End program.  

---

# 6. Error in Code Program in C++

---

##  Theory
This program demonstrates the use of **classes and objects** in C++.  

- A class `cube` is defined with three data members: `height`, `width`, and `length`.  
- A member function `volume()` calculates the cube's volume using the formula:  

\[
\text{Volume} = \text{height} \times \text{width} \times \text{length}
\]

- In the `main()` function, an object `cube1` is created.  
- The program prints the height and the calculated volume.

This shows **encapsulation** and the use of **member functions** to perform operations on object data.  

---

##  Algorithm
1. Start the program.  
2. Define a class `cube` with data members `height`, `width`, and `length`.  
3. Define a function `volume()` to calculate volume = height × width × length.  
4. In `main()`, create an object `cube1` of class `cube`.  
5. Call `volume()` using the object and store the result.  
6. Print the height and the calculated volume.  
7. End program.  

---


##  Conclusion
- **Classes** define the **structure** and **behavior** (data + functions).  
- **Objects** are the actual entities created from classes that hold specific values.  
- Together, classes and objects form the **foundation of Object-Oriented Programming (OOP) in C++**.  
- They make code more **organized, modular, reusable, and easy to maintain**.
