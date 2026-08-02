# 🔒 Protected Members & Inheritance in C++

> A clear C++ program demonstrating the role of the `protected` access specifier in inheritance. It illustrates how a derived class can access protected members of the base class, while private members remain hidden.

---

## 📋 Overview

This program demonstrates the three access specifiers in C++ (private, protected, public) within the context of inheritance:

- **Private (`i`)**: Accessible only within the `Base` class.
- **Protected (`j`)**: Accessible within the `Base` class and its derived classes.
- **Public (`k`)**: Accessible everywhere.

The `Derived` class inherits from `Base` using **public inheritance**. It can freely modify `j` and `k`, but attempting to modify `i` would result in a compilation error.

---

## 🧮 Program Logic & Execution Flow

1. A `Base` class is defined with:
   - A private integer `i`.
   - A protected integer `j`.
   - A public integer `k`.
   - A constructor that initializes these members with default values `(0, 1, 2)`.
   - A `printData()` method to display the values of `i`, `j`, and `k`.
2. A `Derived` class inherits from `Base` publicly.
   - It contains a method `changeData()` that increments `j` and `k` (demonstrating access to protected and public members).
   - It comments out access to `i`, which would cause an error.
3. In `main()`:
   - A `Derived` object `d` is created.
   - `printData()` is called to show initial values.
   - `changeData()` is called.
   - `printData()` is called again to show the updated values.

---

## 💻 Sample Output
Before changing
i (Private) = 0
j (Protected) = 1
k (Public) = 2
After changing
i (Private) = 0
j (Protected) = 2
k (Public) = 3


---

## 🛠️ How to Compile and Run (Windows & Linux)

Follow the instructions below based on your operating system.

### 🪟 For Windows Users (Using MinGW/G++ or any C++ compiler)
| Step | Command |
| :---: | :--- |
| **1. Compile** | `g++ protected_inheritance.cpp -o protected_inheritance.exe` |
| **2. Run** | `protected_inheritance.exe` |

> **Note:** If `g++` is not recognized, make sure MinGW is installed and added to your System PATH.

---

### 🐧 For Linux / macOS Users (Terminal)
| Step | Command |
| :---: | :--- |
| **1. Compile** | `g++ protected_inheritance.cpp -o protected_inheritance` |
| **2. Run** | `./protected_inheritance` |

> **Prerequisite:** Ensure GCC/G++ is installed on your system. (On Linux: `sudo apt install g++` | On macOS: `xcode-select --install`)

---

## 📂 Project Structure
cpp-protected-members-inheritance/
│
├── protected_inheritance.cpp # Main source code file
└── README.md # Project documentation (this file)


---

## 👩‍💻 Author

**Iqra Maqsood Mughal**  
*C++ Developer | Programming Enthusiast*

---

## 📅 Date

**August 2, 2026**

---

## 📄 License

This project is open-source and intended for educational purposes.
