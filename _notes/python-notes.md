---
tags: python
---

### @staticmethod in Python

- Python @staticmethod decorator is used to label a class method as a static method, which means that it can be called without >  instantiating the class first. It simply defines a normal function that is logically contained in the class for readability purposes. Here, we do not need to pass the class instance as the first argument via self, unlike other class functions.
    {% highlight python linenos %}
    class Student():
        def __init__(self, mark):
            self.mark = mark
        @staticmethod
        def find_min(mark):
            return min(mark, 100)
    print(Student.find_min(20))
    # output
    # 20
    {% endhighlight %}

- Static methods can also be accessed via class instances or objects. For example :
    {% highlight python linenos %}

    class Bank():
        def __init__(self, balance):
            self.balance = balance
    
        @staticmethod
        def find_interest(loan_money, interest_rate):
            return loan_money * (1 + interest_rate)
    
    bank = Bank(1000)
    print(bank.find_interest(bank.balance, 0.3))
    {% endhighlight %}

- Comparison between @staticmethod, @classmethod, instance method
  ![compatison](../assets/img/staticmethods.png)


### Abstract Method & Class in Python

#### Abstract Method
- An Abstract method is a method which is declared but does not have implementation such type of methods are called as abstract methods. In Python, we can declare an abstract method by using @abstractmethod decorator.

- This abstract method is present in the abc module in python, and hence, while declaring the abstract method, we have to import the abc module compulsory.

- Here the Child class is responsible for providing an implementation for the parent class abstract method.

#### Abstract Class
##### `class abc.ABC`
- The partially implemented classes are called an abstract class; every abstract class in python should be a child of ABC class, which is present in the abc module.
- The following example demonstrates the creation of parent abstract class defining an abstract method, which is partially implemented, creating child classes that are responsible for providing implementation to parent abstract class. These classes are called **concrete classes**. We cannot create an object to the abstract class, but we can create an object to the child's class.

    {% highlight python linenos %}
    
    from abc import ABC, abstractmethod
    class Vehicle(ABC):
        @abstractmethod
        def getNoOfWheels(Self):
            pass

    class Bus(Vehicle):   ##implementing parent abstract class by using child class
        def getNoOfWheels(self):
            return 6

    class Auto(Vehicle):   ##implementing parent abstract class by using child class
        def getNoOfWheels(self):
            return 3

    b=Bus()
    print(b.getNoOfWheels())


    a=Auto()
    print(a.getNoOfWheels())
    {% endhighlight %}

##### `class abc.ABCMeta`
- Metaclass for defining Abstract Base Classes (ABCs).
