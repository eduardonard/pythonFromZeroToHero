Object-oriented programming (OOP) is a programming paradigm that allows you to structure your code around objects, which are instances of classes. Python is an object-oriented programming language that fully supports OOP concepts.

In Python, a class is a blueprint or a template for creating objects. It defines the attributes (variables) and methods (functions) that objects of that class will have. Here's an example of a simple class definition in Python:

```python

class Car:
    def __init__(self, make, model, year):
        self.make = make
        self.model = model
        self.year = year

    def start_engine(self):
        print(f"The {self.make} {self.model}'s engine is starting.")

    def drive(self, distance):
        print(f"The {self.make} {self.model} is driving {distance} miles.")

    def stop_engine(self):
        print(f"The {self.make} {self.model}'s engine is stopping.")
```



In this example, we have defined a class called `Car`. The `__init__` method is a special method called the constructor, which is executed when an object of the class is created. It initializes the attributes of the object (`make`, `model`, and `year`) using the values passed as arguments.

The other methods (`start_engine`, `drive`, and `stop_engine`) define the behavior of a car object. These methods can access the object's attributes using the `self` parameter, which refers to the instance of the class.

To create an object of the `Car` class and use its methods, you can do the following:

```python

my_car = Car("Toyota", "Camry", 2020)
my_car.start_engine()
my_car.drive(50)
my_car.stop_engine()
```



This will output:

```swift

The Toyota Camry's engine is starting.
The Toyota Camry is driving 50 miles.
The Toyota Camry's engine is stopping.
```



In addition to defining classes, you can also create inheritance relationships between classes. Inheritance allows a class to inherit attributes and methods from another class, known as the superclass or base class. The derived class, also called the subclass, can add its own attributes and methods or override the ones inherited from the superclass.

Here's an example of class inheritance in Python:

```python

class ElectricCar(Car):
    def __init__(self, make, model, year, battery_capacity):
        super().__init__(make, model, year)
        self.battery_capacity = battery_capacity

    def charge(self):
        print(f"The {self.make} {self.model} is charging.")
```



In this example, the `ElectricCar` class is derived from the `Car` class. It inherits the `__init__`, `start_engine`, `drive`, and `stop_engine` methods from the `Car` class. The `__init__` method of the `ElectricCar` class extends the functionality by adding a `battery_capacity` attribute.

You can create an object of the `ElectricCar` class and use its methods, similar to the `Car` class:

```python

my_electric_car = ElectricCar("Tesla", "Model S", 2022, 100)
my_electric_car.start_engine()
my_electric_car.drive(75)
my_electric_car.stop_engine()
my_electric_car.charge()
```



This will output:

```swift

The Tesla Model S's engine is starting.
The Tesla Model S is driving 75 miles.
The Tesla Model S's engine is stopping.
The Tesla Model S is charging.
```



In summary, object-oriented programming in Python allows you to create classes, define their attributes and methods, and create objects (instances) of those classes
