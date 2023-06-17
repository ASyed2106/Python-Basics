### Whats an object 🍄 
    - In(CS) object can be a variable, a data structure, a function, or a method; therefore,
      a location in memory having a value that can be referenced by an identifier
    - In OOP is an instance of a class where this object can be either a variable, a function, a data structure or a combination of such
        - A combination of data and functional code. This is because real-world objects have states and behaviour.
### What is OOP
    - Programming practice to design modular reusable software systems
    - designs programs with creation of Objects
    - focuses on the definition of data rather than the input → processing → output logic
    - meant to create an object that can define/ provide functionality to solve problems

### Procedure vs OOP
Procedure oriented 
            A human may require:
            Calculations
            Logical Evaluations
            Complete Repetitive tasks
            Database
OOP
            What’s their name
            What’s their address
            What functions can this object have?
   
 **“OOP focuses on how to manipulate the data of the object rather than the logic required to manipulate them” **

Object: A combination of data and functional code. This is because real-world objects have states and behaviour.

States: The characteristic, Measurable data of an object

Behaviour: The available functionality of the object (what can it do?)

Object’s Data → called: attributes

Object’s Code → called: methods

### Class
    - An abstract description of all objects that can be made from this set class where an object can be instantiated from.
    - A Class Contains Attributes
    - Attributes: An Object’s accessible tools
#### Creating a class
    1. First define the name of the class with the keyword: class
    2. In its code block (indentation) define its attributes
    3. Then you can assign a variable with an instantiation of the class to interact with it
    Make sure to use parentheses when calling the class name.

#### __init__ method 
    - The __init__ method (double underscores).
    - The initialization method is executed as soon as an object of the class is instantiated
    - It helps us to do any initialization for the object’s attributes
    - self parameter is used to denote that the method is applied and accessible for the object itself
    - self will also treat its own attributes as local
    
### Encapsulation
    - Information Hiding: Restricting the access to the classes/objects’ certain attributes and methods.
        - Why?
            - Data Protection
            - Restricting certain methods to be callable
    - In Python, this isn’t really possible: hence we use a special system. → We hide attributes and methods by using a double underscore __ as a prefix. 
    
##### Setter / Getter methods
    - we need a setter and a getter if values encapsulated 
    - setter methods helps us update encapsulated values
    - we write public methods in order to access encapsulated values
    - this allows us to access it from outside but also restricts how we can access/control
    - Implementing the getter and setter pattern requires: 
            - Making your attributes non-public ( ENCAPSULATING IT)
            - Writing getter and setter methods for each encapsulated attribute
                    - Getter: A method that allows you to access an attribute in a given class
                    - Setter: A method that allows you to set or mutate the value of an attribute in a class

### Overloading 
    - Two methods in one class that have the same method name, but different parameters
            - There are NO OVERLOADING IN Python 3.
    
### Overriding
    - Two methods with the same method name and parameters.
            - One method is in the parent class (lesson 3)
            - One method is in the child class (lesson 3)
            - Overriding allows the child class to provide specific implementation for a method that exists in the parent class
            - You can also override built-in magic-methods. OR Base-functions

### Polymorphism 
    - Polymorphism: A method that can be used across different classes and object that is dependent on the parameters.
        Poly → Many
        Morphism → Forms
    - Ideas:
         - Different Classes (non-inherited) can have the same named methods (Simple) → Polymorphism
         - Within a set of inherited classes have the same methods

### Base override
- allows us to override python features,functions to help with the functionability of our object
       - example:
            - When we try to make our custom objects printable, we actually need to override __repr__ and __str__
                    __repr__ → Allows us to present a printable version of our object
                    __str__ → Allows us to convert our object to a string

### Inheritance
- When an object or class is based on another class; where its features are from a parent class
        **Single Inheritance**: A subclass inheriting the features of a single superclass / parent class
       **Multiple Inheritance**: A subclass inheriting the features of a multiple parent classes
        **Multilevel Inheritance**: A subclass is inheriting from another subclass… A → B → C
                Types:
                    **Multi-Generational**: Grandparent → Parent → Child
                    **Multi-Parent** (Not limited to two)
                                Parent A \
                                            > Child
                                Parent B /
                    **Mixture of 1 and 2**
                    
 #### What can we do with inheritance
- A child will receive all attributes and methods of the parent
- A child can then enhance itself with new attributes and new methods
- A child **can OVERRIDE attributes** and methods for their **own liking/speciality**
    
- **If** a child class inherits the parent class:
    - The child does not need a new __init__() method UNLESS it requires new attributes
    - The child does not need to reinstate the parent’s methods UNLESS you override them

 

