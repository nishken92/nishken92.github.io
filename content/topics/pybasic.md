+++
date = '2025-11-16T09:15:59+05:30'
draft = false
title = 'Python Class'
+++
Classes helps to encapsulate attributes and methods. Creating a class creates a data type (class) where we can create objects of that specific type. Objects of a class can have attributes to define it’s state and methods to modify it’s state. Class inheritance allows the inheritance of attributes and methods from multiple base classes. A method in child class can overide the method in parent class. A child class can overide a method from parent class, but at the same time it can still call the method from parent class using a super() function. Python classes are mutable in nature. They are created in runtime and can be modified in runtime.
The basic data types in python are immutable like integer, string. However, the user defined data types are mutable in nature. Different variable names can be assigned to a same object. In other programming languages it is known as aliasing. In case of mutable data types, when a variable referring to a mutable object only passes the variable reference point to function. If that variable is changed, then the aliased other variable will also get reflected. In simple words, Python doesn’t have different kind of argument passing like pass by value or pass by reference. All argument passing are pass by reference only in python. 

## Namespaces

Namespace is a mapping of names to objects. One example is the set of built in errors. Each built in error name is mapped to an error object. There is absolutely no connection between the same names in different namespaces. Users can differentiate between the same names of different namespaces by putting the name of the module in front of it. All the names that denotes the state of an object are it’s attributes. It can be either immutable or mutable. The mutable attributes of a namespace can even be modifed or deleted. The namespaces are created at different times. Builtin namespaces are created when the python interpreter starts and never get deleted. Top level invocation means the python scripts called from the terminal. They are considered as part of __main__. Likewise all the built in namespaces are considered as a part of the module __builtins__.

A local namespace is created when a function is called and they are deleted once the function returns the value or returns an exception. Recursive functions have their own namespaces. Scope is a textual region in the artifact of program where an unqualified reference of a name is referred directly to the name in that namespace. Unqualified reference means the attribute reference without a module name before it. Scope is found dynamically. In any program execution we can find multiple enclosed scopes whose namespaces are directly accessible. The innermost scope’s namespace is first searched for. Then the nearest enclosed scope will be searched for non-local and non-local namespaces. Third step is the global namespace search for that program. Fourth step is the built in namespace search. 

If a variable is declared global, the variable’s global version only get modified whenever acted upon. It is no more a local variable within a scope. To bind the variables of a scope to outside of the innermost scope, we can use non local keyword. If they are not mentioned on nonlocal then they are just a local variable within the function scope. 

Once a class is defined, a new namespace is created. Function definitions binds the name of the function here in the class’s namespace. 

## Class Objects

Class object has two functions, one is attribute reference and another one is instantiation. Attribute reference syntax is the standard one as obj.name. The names of the attributes depends on the names in the corresponding class’s namespace. 

## Instance Objects.

Instance objects are not required to be instantiated along with the class. If a class is defined, in any subsequent line after the class defintition, a attribute can be added to the class via simple dot product.

class Numbers:
	pass
Numbers.i = 10

The above lines are completely accepted. Please note, a value must be assigned to the variable. Method references of an instance object is valid only when the method name is defined inside the class body. However, the class method instance method are referring to two different memory locations. 

## Method Objects

In the below example, function mouth is bounded to the class Human. Argument self is given as method takes the calling object itself as an input first Once the instance object x is created, it can call the mount function without any argument. This is because any method will automatically pass the calling object as first argument. In other words, if a function is called with N arguments by an object of P data attributes, the function is actually called with N + P arguments. 

class Human:
    def mount(self):
        print("Humans use mouth to speak")
x = Human()
x.mount()
 
