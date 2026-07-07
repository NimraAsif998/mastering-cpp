# **Input and Output & Comments in C++**

## **What is Input?**

**Input** means taking data from the user while the program is running.

**Simple Definition:**

> **Input is the information entered by the user.**

### Example

* Enter your name
* Enter your age
* Enter your marks

In C++, we use **`cin`** to take input from the user.

### Syntax

```cpp
cin >> variableName;
```

### Example

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

# **What is Output?**

**Output** means displaying information on the screen.

👉 **Simple Definition:**

> **Output is the result shown to the user.**

In C++, we use **`cout`** to display output.

### Syntax

```cpp
cout << "Message";
```

### Example

```cpp
#include <iostream>
using namespace std;

int main()
{
    cout << "Welcome to C++ Programming!";

    return 0;
}
```

**Output:**

```
Welcome to C++ Programming!
```

---

# **Using Input and Output Together**

```cpp
#include <iostream>
using namespace std;

int main()
{
    string name;

    cout << "Enter your name: ";
    cin >> name;

    cout << "Hello, " << name << "! Welcome to C++.";

    return 0;
}
```

---

# **Key Points**

* **`cin`** → Used to take **input** from the user.
* **`cout`** → Used to display **output** on the screen.
* **`>>`** is the **input operator**.
* **`<<`** is the **output operator**.

### **Real-Life Example**

Think of a **calculator**:

* **You enter numbers** → **Input**
* **The calculator shows the answer** → **Output**

This is exactly how **`cin`** and **`cout`** work in C++.

# **Comments in C++**

## **What are Comments?**

**Comments** are notes written inside the code to explain what the code does.

 **Simple Definition:**

> **Comments are ignored by the compiler and are only for humans to read.**

They make the code **easy to understand** and **maintain**.

---

# **Types of Comments in C++**

There are **two types** of comments:

### **1. Single-Line Comment (`//`)**

Used for writing a comment on **one line**.

### Syntax

```cpp
// This is a single-line comment
```

### Example

```cpp
#include <iostream>
using namespace std;

int main()
{
    // Display a welcome message
    cout << "Welcome to C++ Programming!";

    return 0;
}
```

---

### **2. Multi-Line Comment (`/* ... */`)**

Used when the comment spans **multiple lines**.

### Syntax

```cpp
/*
This is a
multi-line comment.
*/
```

### Example

```cpp
#include <iostream>
using namespace std;

int main()
{
    /*
      This program
      prints a welcome message.
    */

    cout << "Hello, World!";

    return 0;
}
```

---

# **Why Do We Use Comments?**

* ✅ Explain the purpose of the code.
* ✅ Make the code easier to read.
* ✅ Help during debugging and maintenance.
* ✅ Improve teamwork by making code understandable for others.

---

# **Key Points**

* **`//`** → Single-line comment.
* **`/* ... */`** → Multi-line comment.
* Comments are **ignored by the compiler**.
* Comments are written **for programmers, not for the computer**.

---

## **Real-Life Example**

Think of a **textbook**:

* The **main content** is like your **C++ code**.
* The **notes or highlights** in the margins are like **comments**—they help you understand the content but are **not part of the program execution**.

