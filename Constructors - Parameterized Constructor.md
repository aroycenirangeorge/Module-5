# Exp.No:21

## Constructors - Parameterized Constructor

---

### AIM

To write a Python code to create a class for a person with a parameterized constructor, which takes the `name` and `userid` of the person as parameters and prints the `userid`.

---

### ALGORITHM

1. Begin the program.
2. Define a class `person`.
3. Create a parameterized constructor `__init__(self, name, userid)` that sets and prints values.
4. Use user input to get `name` and `userid`.
5. Instantiate an object of `person` class using the given inputs.
6. End the program.

---

### PROGRAM

```python
# Reg.No: 212223060231
# Name: Royce Niran George A

class person:
    def __init__(self, name, userid):
        self.name = name
        self.userid = userid
        print("UserID of the person is:", self.userid)

# Input from user
name = input("Enter your name: ")
userid = input("Enter your UserID: ")

# Create an instance of person
s1 = person(name, userid)
```

---

### OUTPUT 

![image](https://github.com/user-attachments/assets/2657e3ee-eb3f-47d7-9d54-54495b359fa9)

---

### RESULT

Thus, the Python program using a parameterized constructor to initialize and print a person’s `userid` was successfully executed and verified.

