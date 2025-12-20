## Mathematical Model

Consider a bar of 10m long having uniform cross-section. The temperature of one end of the bar is kept at 10 $^0$C and is varying linearly to 50 $^0$C at other end. Find the temperature of the bar at a distance of 3.75 m from the colder end.

Let x represnts the lenght of the bar and y the corresponding temperature.

```py
# Mathematical Model of the system is based on the straight line equation
y=4x+10
```

The execution throw some error related to 'decimal literal' as it does not understand that '4' and 'x' are to be multiplied. We have to use '*' to represent the multiplication of two quantities.
Modify the code

```py
y=4*x+10
```
This again throw error but this time `x is not defined`. To solve this equation, we must know the value of `x` before above this line. So, let us write x=3.75 which in programming language is called the **assignment of a value to a variable**.

```py
x=3.75
y=4*x+10
```

The code is executing but it is not producing and output. Its similar that I ask a question and you process the answer but you do not tell. In this case the expression on RHS is evaluated and the answer is stored (assignment of value) in variable 'y'. We have to tell computer to display the answer. This is achieved by `print()` function.

```
print(y)
```

This is the plain answer. We will discuss later how to make it more readable and formatted. No let us change the value of 'x' to 4 and check the answer.

```py
x=4
y=4*x+10
print(y)
```

See the difference between two, In first case its '25.0' a real number and in second case the answer '26' is an integer. The real numbers in progamming languages are called `float` number and integer as `integer`. The are collectively called **data-type**. So, in first case, the data-type of 'y' is `float` in second case, the data-type is `integer`. The python automatically assign the data-type to a variable according to its assigned value.

We can use python's built-in function `type()` that returns the class of an object. Actually, in python every variable we use **refer** to an `object`.

To go bit deeper, when we write `x = 4'; `4` is an `object` and `x` is a reference (name) pointing to that object.

An object has three things
- Identity : where it lives in memory
- Type : what kind of object it is
- Value : the data it holds

Let us check what you get

```py
x = 10

print(id(x))     # identity
print(type(x))   # type
print(x)         # value
```

## Class

A user-defined prototype for an object that defines a set of attributes that characterize any object is called the class. The attributes are data members (class variables and instance variables) and methods are functions to do a specific task and associated with a class.

The attributes and methods for an object of the class are accessed via dot notation.

Classes allow us to group our data called attributes and methods in a way that is easy to reuse and also easy to build upon when needed.

Let us create a class 'Employee' for a company as each individual employee is going to have specific attributes and methods.



