# Exp.No:22

## Destructor

---

### AIM

To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.
2. Define the `Student` class.
3. Implement the `__init__` method to initialize and print a message.
4. Implement the `__del__` method to print a message when the object is destroyed.
5. Create an object of the `Student` class.
6. Use the `del` keyword to delete the object and trigger the destructor.
7. End the program.

---

### PROGRAM

```python
# Reg.No: 212223060231
# Name: Royce Niran George A

class Student:
    def __init__(self):
        print("Constructor is called. Student object created.")

    def __del__(self):
        print("Destructor is called. Student object deleted.")

# Creating object
s2 = Student()

# Deleting object
del s2
```

---

### OUTPUT 

![image](https://github.com/user-attachments/assets/ed35b6bb-40b7-44cc-af88-fee36e68ab9d)

---

### RESULT

Thus, the Python program that demonstrates the use of a destructor in the `Student` class was successfully executed and verified.
