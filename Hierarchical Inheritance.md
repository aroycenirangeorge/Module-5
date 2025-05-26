# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
```
# Reg.No-212223060231
# Name-Royce Niran George A

class Details:
    def __init__(self):
        self.__id = ""
        self.__name = ""
        self.__gender = ""

    def setData(self, id, name, gender):
        self.__id = id
        self.__name = name
        self.__gender = gender

    def showData(self):
        print("Id: ", self.__id)
        print("Name: ", self.__name)
        print("Gender: ", self.__gender)


class Employee(Details):  # Inheritance
    def __init__(self):
        super().__init__()
        self.__company = ""
        self.__dept = ""

    def setEmployee(self, id, name, gender, comp, dept):
        self.setData(id, name, gender)
        self.__company = comp
        self.__dept = dept

    def showEmployee(self):
        self.showData()
        print("Company: ", self.__company)
        print("Department: ", self.__dept)


class Doctor(Details):  # Inheritance
    def __init__(self):
        super().__init__()
        self.__hospital = ""
        self.__dept = ""

    def setEmployee(self, id, name, gender, hos, dept):
        self.setData(id, name, gender)
        self.__hospital = hos
        self.__dept = dept

    def showEmployee(self):
        self.showData()
        print("Hospital: ", self.__hospital)
        print("Department: ", self.__dept)


# Input
id = int(input())
name = input()
gender = input()
comp = input()
dept = input()

id1 = int(input())
nam = input()
gen = input()
hosp = input()
dep = input()

# Creating and displaying Employee object
print("Employee Object")
e = Employee()
e.setEmployee(id, name, gender, comp, dept)
e.showEmployee()

# Creating and displaying Doctor object
print("\nDoctor Object")
d = Doctor()
d.setEmployee(id1, nam, gen, hosp, dep)
d.showEmployee()


```

### OUTPUT  
![image](https://github.com/user-attachments/assets/45d0cbc2-1be3-487b-9205-eee868963420)


### RESULT
Thus the program to get the employee and doctor details and display them using hierarchical inheritance has been implemented and executed successfully.
