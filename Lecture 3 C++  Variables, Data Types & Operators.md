# **Mastering C++ – Lecture 3**

# **Variables, Data Types & Operators**

---

# **What You Will Learn**

By the end of this lecture, students will be able to:

* Understand what variables are.
* Learn different C++ data types.
* Store and manipulate data.
* Perform calculations using operators.
* Write simple C++ programs.

---

# **What is a Variable?**

A **variable** is a named memory location used to store data.

👉 Simply:

> **A variable is like a box where we store information.**

For example:

* Store age
* Store marks
* Store salary
* Store student name

### Real-Life Example

Imagine your bedroom.

You have different boxes.

* One box contains books.
* One box contains clothes.
* One box contains shoes.

Each box has a **label**.

Similarly,

Variables also have names.

```
Age Box
Marks Box
Salary Box
```

---

# **Variable Declaration**

### Syntax

```cpp
dataType variableName;
```

Example

```cpp
int age;
```

Here

* `int` → Data Type
* `age` → Variable Name

---

# **Variable Initialization**

Assigning a value to a variable is called **initialization**.

```cpp
int age = 20;
```

Another Example

```cpp
float salary = 50000.5;
```

---

# **Rules for Naming Variables**

✅ Can contain letters

```cpp
age
```

✅ Can contain numbers

```cpp
student1
```

✅ Can use underscore

```cpp
total_marks
```

❌ Cannot start with a number

```cpp
1age
```

❌ Cannot use spaces

```cpp
student name
```

❌ Cannot use keywords

```cpp
int int;
```

---

# **What are Data Types?**

A **data type** tells the compiler **what kind of data a variable will store.**

Example

Age → Integer

Salary → Decimal

Grade → Character

Name → Text

---

# **Common C++ Data Types**

| Data Type | Stores                | Example    |
| --------- | --------------------- | ---------- |
| int       | Whole Numbers         | 10         |
| float     | Decimal Numbers       | 10.5       |
| double    | Large Decimal Numbers | 12345.6789 |
| char      | Single Character      | 'A'        |
| bool      | True or False         | true       |
| string    | Text                  | "Nimra"    |

---

# **Example Program**

```cpp
#include <iostream>
using namespace std;

int main()
{
    int age = 20;
    float cgpa = 3.75;
    char grade = 'A';
    bool pass = true;
    string name = "Ali";

    cout << age << endl;
    cout << cgpa << endl;
    cout << grade << endl;
    cout << pass << endl;
    cout << name << endl;

    return 0;
}
```

---

# **Output**

```
20
3.75
A
1
Ali
```

---

# **Taking Input from User**

```cpp
#include <iostream>
using namespace std;

int main()
{
    int age;

    cout << "Enter your age: ";
    cin >> age;

    cout << "Your age is: " << age;

    return 0;
}
```

---

# **Practice Example**

```cpp
#include <iostream>
using namespace std;

int main()
{
    string name;
    int age;

    cout << "Enter Name: ";
    cin >> name;

    cout << "Enter Age: ";
    cin >> age;

    cout << "Name: " << name << endl;
    cout << "Age: " << age;

    return 0;
}
```

---

# **What are Operators?**

Operators are **symbols that perform operations on variables and values.**

Example

```cpp
5 + 3
```

Here

`+` is an operator.

---

# **Types of Operators**

There are several types of operators:

* Arithmetic Operators
* Assignment Operators
* Comparison (Relational) Operators
* Logical Operators
* Increment & Decrement Operators

---

# **1. Arithmetic Operators**

Used for mathematical calculations.

| Operator | Meaning             | Example |
| -------- | ------------------- | ------- |
| +        | Addition            | 5 + 2   |
| -        | Subtraction         | 5 - 2   |
| *        | Multiplication      | 5 * 2   |
| /        | Division            | 10 / 2  |
| %        | Modulus (Remainder) | 10 % 3  |

---

### Example

```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 10;
    int b = 3;

    cout << "Addition: " << a + b << endl;
    cout << "Subtraction: " << a - b << endl;
    cout << "Multiplication: " << a * b << endl;
    cout << "Division: " << a / b << endl;
    cout << "Remainder: " << a % b;

    return 0;
}
```

---

# **Output**

```
Addition: 13
Subtraction: 7
Multiplication: 30
Division: 3
Remainder: 1
```

---

# **2. Assignment Operator**

Used to assign values.

```
=
+=
-=
*=
/=
%=
```

Example

```cpp
int x = 5;

x += 3;
```

Output

```
8
```

---

# **3. Comparison (Relational) Operators**

Used to compare two values.

| Operator | Meaning               |
| -------- | --------------------- |
| ==       | Equal To              |
| !=       | Not Equal             |
| >        | Greater Than          |
| <        | Less Than             |
| >=       | Greater Than or Equal |
| <=       | Less Than or Equal    |

---

### Example

```cpp
int a = 10;
int b = 20;

cout << (a < b);
```

Output

```
1
```

---

# **4. Logical Operators**

Used when working with multiple conditions.

| Operator | Meaning |
| -------- | ------- |
| &&       | AND     |
| ||       | OR      |
| !        | NOT     |

---

### Example

```cpp
int age = 22;

cout << (age >= 18 && age <= 30);
```

Output

```
1
```

---

# **5. Increment & Decrement Operators**

Increment increases the value by **1**.

```cpp
a++;
```

Decrement decreases the value by **1**.

```cpp
a--;
```

---

### Example

```cpp
int a = 5;

a++;

cout << a;
```

Output

```
6
```

---

# **Complete Example Program**

```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 15;
    int b = 4;

    cout << "Addition = " << a + b << endl;
    cout << "Subtraction = " << a - b << endl;
    cout << "Multiplication = " << a * b << endl;
    cout << "Division = " << a / b << endl;
    cout << "Modulus = " << a % b << endl;

    cout << (a > b) << endl;
    cout << (a == b) << endl;

    a++;

    cout << a << endl;

    return 0;
}
```

---

# **Real-Life Activity (Class Practice)**

Suppose a student has:

* English = 85
* Math = 90

Ask students to:

* Store marks in variables.
* Calculate total marks.
* Calculate average.
* Display the results.

---

# **Practice Program**

```cpp
#include <iostream>
using namespace std;

int main()
{
    int english = 85;
    int math = 90;

    int total = english + math;
    float average = total / 2.0;

    cout << "English: " << english << endl;
    cout << "Math: " << math << endl;
    cout << "Total: " << total << endl;
    cout << "Average: " << average;

    return 0;
}
```

---

# **Key Takeaways**

* A **variable** stores data in memory.
* **Data types** define the type of data a variable can hold.
* Use meaningful variable names.
* **Operators** perform calculations, comparisons, and logical operations.
* Practice with simple programs to build confidence before moving to conditional statements and loops.


