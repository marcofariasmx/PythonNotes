# PythonNotes
PythonNotes

An abstract class can be considered as a blueprint for other classes. It allows you to create a set of methods that must be created within any child classes built from the abstract class

```python
# Python program showing
# abstract base class work

from abc import ABC, abstractmethod

class Polygon(ABC):

	@abstractmethod
	def noofsides(self):
		pass

class Triangle(Polygon):

	# overriding abstract method
	def noofsides(self):
		print("I have 3 sides")

class Pentagon(Polygon):

	# overriding abstract method
	def noofsides(self):
		print("I have 5 sides")

class Hexagon(Polygon):

	# overriding abstract method
	def noofsides(self):
		print("I have 6 sides")

class Quadrilateral(Polygon):

	# overriding abstract method
	def noofsides(self):
		print("I have 4 sides")

# Driver code
R = Triangle()
R.noofsides()

K = Quadrilateral()
K.noofsides()

R = Pentagon()
R.noofsides()

K = Hexagon()
K.noofsides()

```


Static methods in Python are extremely similar to python class level methods, the difference being that a static method is bound to a class rather than the objects for that class. This means that a static method can be called without an object for that class. This also means that static methods cannot modify the state of an object as they are not bound to it

```python
class Calculator:

    def addNumbers(x, y):
        return x + y

# create addNumbers static method
Calculator.addNumbers = staticmethod(Calculator.addNumbers)

print('Product:', Calculator.addNumbers(15, 110))

```


Python class attributes are variables of a class that are shared between all of its instances. They differ from instance attributes in that instance attributes are owned by one specific instance of the class only, and are not shared between instances.

Attributes defined under the class, arguments goes under the functions. arguments usually refer as parameter, whereas attributes are the constructor of the class or an instance of a class

```python
class Student:
    school = "freeCodeCamp.org"
    
    def __init__(self, name, course):
        self.name = name
        self.course = course
    
Student1 = Student("Jane", "JavaScript")
Student2 = Student("John", "Python")

print(Student1.name) # Jane
print(Student2.name) # John

```


List and Tuple in Python are the classes of Python Data Structures. The list is dynamic, whereas the tuple has static characteristics. This means that lists can be modified whereas tuples cannot be modified, the tuple is faster than the list because of static in nature. Lists are denoted by the square brackets but tuples are denoted as parenthesis.

| SR.NO. | LIST                                                                          | TUPLE                                                     |   |   |
|--------|-------------------------------------------------------------------------------|-----------------------------------------------------------|---|---|
| 1      | Lists are mutable                                                             | Tuples are immutable                                      |   |   |
| 2      | The implication of iterations is Time-consuming                               | The implication of iterations is comparatively Faster     |   |   |
| 3      | The list is better for performing operations, such as insertion and deletion. | Tuple data type is appropriate for accessing the elements |   |   |
| 4      | Lists consume more memory                                                     | Tuple consumes less memory as compared to the list        |   |   |
| 5      | Lists have several built-in methods                                           | Tuple does not have many built-in methods.                |   |   |
| 6      | The unexpected changes and errors are more likely to occur                    | In tuple, it is hard to take place.                       |   |   |


Doctest format:
```python
def sum(a, b):
    """
    >>> sum(4, 3)
    7

    >>> sum(-4, 5)
    1
    """
    return a + b

```
    
```python
```

```python
```

```python
```

```python
```
