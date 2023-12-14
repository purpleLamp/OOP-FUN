Polymorphism:
- can be implemented with or without inheritance
- method shares the same name but function different

Encapsulation:
- preventing access to variables directly instead uses getters and setters

Abstraction:
- Exposing only the most relavent aspects of the class to the user hiding everything else

Inheritance:
- a subclass gaining access to all the functionality of another class

In this file I have demonstrated abstraction, encapsulation, polymorhism and inheritance 
with some very simple classes.

GenericThing is the function from which the other two functions inherit from. All the public functions and data members are available 
to the derived classes. GenericThing has a private data member and function which are both accessed through public methods show casing 
encapsulation and abstraction. The doSomething method accesses the private print function which is abstracted from the implementation.
The doSomething method is also altered in the derived classes giving multiple forms to the method which is an example of polymorphism.
