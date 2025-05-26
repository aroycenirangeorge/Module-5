# Exp.No:21  
## Constructors - Parameterized Constructor

---

### AIM  
To write a Python code to create a class for a person with a parameterized constructor, which will take the `name` and `userid` of the person as parameters and print the `userid` of the person.

---

### ALGORITHM

1. Begin the program.  
2. Define a `person` class.  
3. The `person` class should have a parameterized `__init__` method that accepts two parameters: `name` and `userid`.  
4. Inside the `__init__` method, assign the `name` to `self.name` and the `userid` to `self.userid`.  
5. Print the `self.userid`.  
6. Prompt the user to enter their `name` (string) and `userid`.  
7. Create an instance `s1` of the `person` class by passing the entered `name` and `userid` to the constructor.  
8. Terminate the program.

---

### PROGRAM

```
# Reg.No-212223060231
# Name-Royce Niran George A

class Person:
    def __init__(self, name, uid):
        self.name = name
        self.uid = uid

    def dis(self):
        print(self.uid)

name = input()
uid = input()
p = Person(name, uid)
p.dis()
```

### OUTPUT
![image](https://github.com/user-attachments/assets/de78e84a-0f9f-4f4e-9a97-b5d62b136760)

### RESULT
Thus the program to create a class for a person with a parameterized constructor has been implemented and executed successfully.
