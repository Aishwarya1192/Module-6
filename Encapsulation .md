# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
class Rectangle:
    def __init__(self, length, breadth):
        # Private member variables
        self.__length = length
        self.__breadth = breadth

    # Setter methods
    def set_length(self, length):
        self.__length = length

    def set_breadth(self, breadth):
        self.__breadth = breadth

    # Getter methods
    def get_length(self):
        return self.__length

    def get_breadth(self):
        return self.__breadth

    # Method to calculate area
    def area(self):
        return self.__length * self.__breadth


# Example usage
rect = Rectangle(10, 5)
print("Length:", rect.get_length())
print("Breadth:", rect.get_breadth())
print("Area:", rect.area())

# Modify values using setters
rect.set_length(12)
rect.set_breadth(6)
print("\nAfter modification:")
print("Length:", rect.get_length())
print("Breadth:", rect.get_breadth())
print("Area:", rect.area())


## Output
Length: 10
Breadth: 5
Area: 50

After modification:
Length: 12
Breadth: 6
Area: 72


## Result
Hence the output is verified
