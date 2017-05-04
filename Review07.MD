# Review Ques 7

## Patterns:

1. What is a visitor pattern and why is it useful? 

In object-oriented programming and software engineering, the visitor design pattern is a way of separating an algorithm from an object structure on which it operates. A practical result of this separation is the ability to add new operations to extant object structures without modifying the structures. In essence, the visitor allows adding new virtual functions to a family of classes, without modifying the classes. Instead, a visitor class is created that implements all of the appropriate specializations of the virtual function. The visitor takes the instance reference as input, and implements the goal through double dispatch.


The nature of the Visitor makes it an ideal pattern to plug into public APIs thus allowing its clients to perform operations on a class using a “visiting” class without having to modify the source.

2. Give an example where factory pattern is suitable in class design. How could factory be usefully combined with visitor.

The creation of an object makes reuse impossible without significant duplication of code.



3. What is a singleton pattern? Give an example. What is the connection between factory and singleton?

Ensure a class only has one instance and provide a global point of access to it.

A Factory which itself is a Singleton, that creates a Singleton. This factory than can be used to return an implementation of a interface which a range of Singletons could define the implementations of. The single most important factor that makes a class a Singleton is a “private constructor”. By having a private constructor, there is NO other Class except for itself that can create an Object instance of that class.

4. What is coupling and cohesion among classes? Ideally, how should design alter these values? Justify your answer.

1)Cohesion refers to what the class (or module) will do. Low cohesion would mean that the class does a great variety of actions and is not focused on what it should do. High cohesion would then mean that the class is focused on what it should be doing, i.e. only methods relating to the intention of the class. 2) Coupling refers to how related are two classes / modules and how dependent they are on each other. Being low coupling would mean that changing something major in one class should not affect the other. High coupling would make your code difficult to make changes as well as to maintain it, as classes are coupled closely together, making a change could mean an entire system revamp.

All good software design will go for high cohesion and low coupling.

5. What is the layered patterns? Name one advantage and one disadvantage for layers. 



6. What is the proxy pattern? What does it offer to coupling? What does it offer to layers?



7. A body has several limbs. Limbs have extremities (hands or feet).  Extremeties contain toes or fingers. 
   -  Which design pattern is similar to this structure?
Composite pattern


   - Briefly describe the components of that design pattern.
  
COmpose objects into tree structures to represent part-whole hierarchies. Let clients treat individual objects and compositions of objects uniformly. 

## Anti patterns:

8. What is a god class? How to recognize it? How to fix it?

A "God Class" is an object that controls way too many other objects in the system and has grown beyond all logic to become The Class That Does Everything. Seperate into smaller classes that solves only a small part of the problems or only one problem.

9. For OO purists, "type switching" statements are bad. What is an example of such a statement. How to fix it? What general principle of OO is demonstrated by that fix?



10. Do all bad smells really matter? Explain.



11. Give two examples of each of the following bad smells:
    - Bloating

    Long Method; Large Class; Primitive Obsession; Long Parameter List; Data Clumps 

    - Dispensable

    A dispensable is something pointless and unneeded whose absence would make the code cleaner, more efficient and easier to understand.
    
    Comments; Duplicate Code; Lazy Class; Data Class; Dead Code; Speculative Generality

    - OO abusers

    All these smells are incomplete or incorrect application of object-oriented programming principles.

    Switch Statements; Temporary Field; Refused Bequest; Alternative Classes with Different Interfaces

    
12. Below are a list of OO designs and Arthur Riel's OO  heuristics. Describe how to fix the design so that it agrees with the heuristic:
    - **Design:** One central class has 20 distinct methods for account creation, 60 distinct methods for account auditing, 50 distinct methods for writing objects to a SQL database.   
  **Heuristic 3.3** Beware of classes that have many accessor methods defined in their public interface, many of them imply that related data and behavior are not being kept in one place.



    - **Design:** You need to use a commercial API that highly couples the business logic and GUI layers.  
  **Heuristic 3.5:** In applications which consist of an object-oriented model interacting with a user interface, the model should never be dependent on the interface. The interface should be dependent on the model.




    - **Design:** In your math API, integer class inherits from fractions class.  
  **Heuristic 5.1** Inheritance should only be used to model a specialization hierarchy.