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

The all() function returns True if all items in the list evaluate to True. Otherwise, it returns False.
The any() function takes as arguments the list to check inside, and the item to check for. If "any" of the items in the list match the item to check for, the function returns True.

What is the algorithmic paradigm of quick sort? Divide and conquer


A set is an unordered collection unique items. A list is an ordered collection of non-unique items.


```python
class test:
    def __init__(self):
        print('I came here without your permission lol')
        pass
t1 = test()
>>> 'I came here without your permission lol'
```

What is the purpose of the self keyword when defining or calling methods on an instance of an object? self refers to the instance whose method was called.
Try running the example of the above without passing self argument inside the __init__, you'll understand the reason. You'll get the error like this __init__() takes 0 positional arguments but 1 was given, this means that something is going inside even if haven't specified, which is instance itself.


Proper way to define a function
```python
def get_max_num(list_of_nums):
```


You use the decorator to alter the functionality of a function without having to modify the functions code.


```python
# Python program to illustrate functions
# can be passed as arguments to other functions
def shout(text):
	return text.upper()

def whisper(text):
	return text.lower()

def greet(func):
	# storing the function in a variable
	greeting = func("""Hi, I am created by a function passed as an argument.""")
	print (greeting)

greet(shout)
greet(whisper)

```

```python
```



```python
```



```python
```



```python
```



```python
```



```python
```



```python
```



```python
```



```python
```
