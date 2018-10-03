
# Practice With Classes and Instances

## Introduction
Okay, we learned how to declare classes and create instances in our last lesson. Let's put these new skills to the test!

## Objectives

* Practice defining classes
* Practice instantiating instances of classes

## Defining Classes


Let's define a `Ride`, `Driver`, and `Passenger` class as these are all crucial parts to a single ride. We have provided files for you aptly named ride.py, driver.py, and passenger.py where you can define the appropriate classes. Below, we import the classes from those files so we can use them in our code. The import syntax in Python is as follows: the keyword `from` followed by the name of the file then the keyword `import` and finally the name of the object we are importing (i.e. `from` `[filename]` `import` `[object_name]`). The first import is done for you, follow its example to import the other two classes.

> **Reminder:** *since we need to have some Python code in our class when we define it, we can simply write the keyword `pass` on the first line under our class definition*

> **Note:** the next cell imports an extension, `autoreload`, from IPython which reloads our import just before we execute our code, so that if we make a change in one of our files (i.e. ride.py), that change will be reflected below. Don't worry about it right now, but know that it is just updating our imported code.


```python
%load_ext autoreload
%autoreload 2
```


```python
from ride import Ride
```


```python
# import Driver class here
from driver import Driver
```


```python
# import Passenger class here
from passenger import Passenger
```

## Creating Instances

Let's now practice using our classes to make instances of those classes. Make two instances of the Passenger class and assign them to the variables `meryl` and `daniel`, respectively.


```python
meryl = Passenger()
daniel = Passenger()
print(meryl, daniel)
```

    <passenger.Passenger object at 0x00000217E9A109B0> <passenger.Passenger object at 0x00000217E9A10978>
    

Next, make one instance of the driver class and assign it to the variable, `flatiron_taxi`.


```python
flatiron_taxi = Driver()
print(flatiron_taxi)
```

    <driver.Driver object at 0x00000217E9A108D0>
    

Finally, make two instances of the Ride class and assign them to `ride_to_school` and `ride_home`. 


```python
ride_to_school = Ride()
ride_home = Ride()
print(ride_to_school, ride_home)
```

    <ride.Ride object at 0x00000217E9A10BA8> <ride.Ride object at 0x00000217E9A10B70>
    

## Summary
Great! In this lab, we were able to define multiple classes and create instances of those classes.