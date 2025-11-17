INHERITANCE
Activity 1:

class Animal:
    def speak(self):
        print("Animal makes a sound")

class Dog(Animal):
    def speak(self):
        print("Dog barks")

class Cat(Animal):
    def speak(self):
        print("Cat meows")
        
dog = Dog()
cat = Cat()

dog.speak()
cat.speak()

Activity 2:

class Vehicle:
    def __init__(self, brand, fuel):
        self.brand = brand
        self.fuel = fuel

class Car(Vehicle):
    def __init__(self, brand, fuel, doors):
        super().__init__(brand, fuel)
        self.doors = doors

    def drive(self):
        self.fuel -= 1
        print(f"{self.brand} is driving. Fuel left: {self.fuel}")

car = Car("Toyota", 5, 4)
car.drive()

ENCAPSULATION
Activity 1:

class BankAccount:
    def __init__(self, balance):
        self.__balance = balance

    def deposit(self, amount):
        self.__balance += amount

    def get_balance(self):
        return self.__balance

account = BankAccount(1000)
account.deposit(500)
print(account.get_balance())

Activity 2:

class Person:
    def __init__(self, age):
        self._age = None
        self.age = age

    @property
    def age(self):
        return self._age

    @age.setter
    def age(self, value):
        if value > 0:
            self._age = value
        else:
            print("Invalid age!")

p = Person(20)
print(p.age)

POLYMORPHISM 
Activity 1:

class InkPrinter:
    def print_document(self):
        print("Printing using ink...")

class LaserPrinter:
    def print_document(self):
        print("Printing using laser...")

for printer in [InkPrinter(), LaserPrinter()]:
    printer.print_document()


Activity 2:

def make_it_speak(obj):
    obj.speak()

class Bird:
    def speak(self):
        print("Chirp!")

class Robot:
    def speak(self):
        print("Beep!")

make_it_speak(Bird())
make_it_speak(Robot())

ABSTRACTION
Activity 1:

from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Circle(Shape):
    def __init__(self, r):
        self.r = r

    def area(self):
        return 3.14 * self.r ** 2

print(Circle(5).area())


Activity 2: 

from abc import ABC, abstractmethod

class Employee(ABC):
    @abstractmethod
    def calculate_pay(self):
        pass

class HourlyEmployee(Employee):
    def __init__(self, hours, rate):
        self.hours = hours
        self.rate = rate

    def calculate_pay(self):
        return self.hours * self.rate

print(HourlyEmployee(40, 200).calculate_pay())
