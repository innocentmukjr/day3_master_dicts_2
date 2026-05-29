# Day 3 – Employee Dictionary Manipulation

## 📘 The Exercise Instructions

Given the following dictionary:
```python
employees = {
    "emp_1": {"name": "Alice", "salary": 5000},
    "emp_2": {"name": "Bob", "salary": 4500},
    "emp_3": {"name": "Charlie", "salary": 6000}
}
Perform these tasks:

Increase Alice’s salary by 10%.

Change Bob’s name to “Robert”.

Add a new employee (any name and salary).

Add a new field department to Charlie.

Print all employees with salary above 5000.

🧠 My Approach
Salary increase: Accessed Alice’s salary with employees["emp_1"]["salary"] and multiplied by 1.1.

Name change: Assigned "Robert" to employees["emp_2"]["name"].

Add employee: Created a new key "emp_4" with a dictionary {"name": "Inno", "salary": 9000}.

Add department: Added "department" key to Charlie’s inner dict: employees["emp_3"]["department"] = "Teaching".

Filter & print: Looped through employees.values() and printed info['name'] if info['salary'] > 5000.

🚧 Challenges I Faced
Remembering the double bracket syntax for nested dictionaries ([key1][key2]).

Avoiding KeyError when accessing salary – made sure the key exists.

Deciding whether to use .items() or .values() – chose .values() because I didn’t need the outer key (emp_1, etc.).

✅ What I Learned
Dictionaries are mutable – changes happen directly in the original dict.

Adding a new key to a nested dictionary works the same as adding to a flat dictionary.

Looping through .values() is cleaner when the outer keys are irrelevant.

Multiplying by 1.1 is the correct way to increase a number by 10% in Python.

🖥️ How to Run My Code
Make sure you have Python installed (3.x).

Save the code as main.py.

Open a terminal in the same folder.

Run:

bash
python main.py
Expected output (order may vary depending on Python version):

text
Employees with salary above 5000:
Alice
Charlie
Inno
📅 Part of My AI/ML Learning Journey
This is Day 3 of my Python basics. Dictionaries are essential for managing structured data – later I’ll use them for feature stores, model hyperparameters, and configuration files in machine learning projects.
