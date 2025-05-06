# Exp.No:25

## Hierarchical Inheritance

---

### AIM

To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class `Details`** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method `display_details()`** to print the values of `id`, `name`, and `gender`.
4. **Create a class `Employee`** that inherits from the `Details` class.

   * Add two additional attributes: `company` and `department`.
   * Override the `display_details()` method to print the employee-specific attributes along with inherited details.
5. **Create a class `Doctor`** that also inherits from the `Details` class.

   * Add two additional attributes: `hospital` and `department`.
   * Override the `display_details()` method to print the doctor-specific attributes along with inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects** of `Employee` and `Doctor`.
8. **Call the `display_details()` method** for both objects.
9. **Terminate the program.**

---

### PROGRAM

```python
#Reg.No:
#Name:

# Parent class
class Details:
    def __init__(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

    def display_details(self):
        print(f"ID: {self.id}")
        print(f"Name: {self.name}")
        print(f"Gender: {self.gender}")

# Child class Employee inheriting from Details
class Employee(Details):
    def __init__(self, id, name, gender, company, department):
        # Initialize the parent class (Details)
        super().__init__(id, name, gender)
        self.company = company
        self.department = department

    def display_details(self):
        super().display_details()  # Call parent's display_details()
        print(f"Company: {self.company}")
        print(f"Department: {self.department}")

# Child class Doctor inheriting from Details
class Doctor(Details):
    def __init__(self, id, name, gender, hospital, department):
        # Initialize the parent class (Details)
        super().__init__(id, name, gender)
        self.hospital = hospital
        self.department = department

    def display_details(self):
        super().display_details()  # Call parent's display_details()
        print(f"Hospital: {self.hospital}")
        print(f"Department: {self.department}")

# Main program execution
def main():
    # Input employee details
    print("Enter Employee Details:")
    emp_id = input("Enter ID: ")
    emp_name = input("Enter Name: ")
    emp_gender = input("Enter Gender: ")
    emp_company = input("Enter Company: ")
    emp_department = input("Enter Department: ")

    # Create an Employee object
    emp = Employee(emp_id, emp_name, emp_gender, emp_company, emp_department)
    print("\nEmployee Details:")
    emp.display_details()

    # Input doctor details
    print("\nEnter Doctor Details:")
    doc_id = input("Enter ID: ")
    doc_name = input("Enter Name: ")
    doc_gender = input("Enter Gender: ")
    doc_hospital = input("Enter Hospital: ")
    doc_department = input("Enter Department: ")

    # Create a Doctor object
    doc = Doctor(doc_id, doc_name, doc_gender, doc_hospital, doc_department)
    print("\nDoctor Details:")
    doc.display_details()

if __name__ == "__main__":
    main()
```

---

### OUTPUT

![image](https://github.com/user-attachments/assets/30c730d9-4968-4e71-bb0e-43e59907ca01)

---

### RESULT

The program correctly implements hierarchical inheritance, allowing the input of employee and doctor details.
