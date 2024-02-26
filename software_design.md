# Software Design Methodologies

## Design principle

There are three principle design strategies used in software engineering:
* Structured design
* Function oriented design
* Object oriented design



####1. What do we mean by coupling and cohesion when discussing structured design?

Structured-design is based on the ‘divide-conquer’ technique. This means that problems are subdivided, further divided into small problems which is solved iteratingly until gradually the higher level problems are solved. Through structured design, a low coupling and high cohesion is achieved (as each problems gets solved individually before loosely connecting modules/ classes). 

Coupling and Cohesion are some of the concept used to define and measure the quality of a software design. Coupling in a software design refer to classes / modules that are connected to other classes or modules through either data, objects and other bindings. Therefore, High coupling in software design indicates that changes in one classes strongly affect the state or usability of the other class. Whereas low coupling, is the opposite therefore, have less effect on its usability.

Cohesion in software design refer to elements inside a class, working together to full fill the purpose of the class. High cohesion indicates that elements inside the class have been fully used resulting in a better structured class whereas low cohesion means the elements in the class is less structured and connected to each other. This may mean that the class have not been created for a single purpose but multiple purpose (The Single Responsibility in SOLID Principle not being met). 

[^1][^2][^3]


2. What is the difference between top-down and bottom-up design? Which best describes a function oriented design?
   
- The main difference between them is their focus point. 
- Top-down approach focuses on solving issues by breaking down problem into smaller parts whilst bottom up approach design focuses on solving small problems until the bigger pictures starts to shape. 
- Top-down approach involves high level planning and decision making whilst bottom-down approach is mainly focused on executing smaller tasks and slowly developing an understanding into the unknown knowledge. 

Functional Oriented Design is composed of multiple functions which are viewed as sub-system. Therefore the system is made up of the overall picture of all the functions. This design starts designing by looking at the higher level view of the system, then creating functions into more detailed functions as the design is developed thus using the top-down approach. 

[^4][^5]


3. In which design methodology would a class diagram be most useful?
   
The class diagram is a type of structure diagram that describes the structure of a system by showing its class, attributes, operations and relationships between the objects. A class diagram would be most useful on the object-orientated design methodology as it put emphasis on designing a collection of interacting object with its own data and behaviour. This makes every object oriented project very dynamic and the effective way of blueprinting the structure of the software design is through class diagram. [^6]


4. What are the four pillars of object oriented programming? Give a single-sentence description of each.

- Abstraction: Only show the necessary detail of the class / design allowing more focus on essential parts.
- Encapsulation: Data and code enclosed into a unit (data hiding by using private on properties)
- Inheritance: Passing parent class properties into a child class, whilst child class also retaining its own unique features. 
- Polymorphism: Different classes that have the same parent can perform the same behaviour as well as other form of behaviours.
[^7]


5. What is the strategy pattern? How would its implementation differ between a functional and object oriented system?
   
Strategy pattern: algorithm / class behaviour getting changed at run time. Its implementation differs as functional system uses higher order function to promote the behavioural change depending on different type of situations whereas object oriented system makes mostly use of interface, classes and polymorphism.

In functional system - a function would take other functions (strategy) as arguments (one high-level function and many strategy = strategy pattern + functional  oriented design).
In object oriented system = interface, classes and polymorphism (one context class + various objects as strategies = context object algorithm behavioural change due to polymorphism) 
[^8]


6. Imagine you are creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.

Object-Oriented Design methodology, combined with the Strategy Pattern is best for creating a versatile online payment system that is adaptable across various use cases. This is due to, object oriented programming pillars such as encapsulations which ensures data privacy. In this case study, privacy is a requirement for the system as it deals with payments. Another main reason is polymorphism, which makes the development of different type of payment system very flexible as similar operations behave and is implemented differently without changing the interface. As a result, this makes the system widely applicable. 

REFERENCES
[^1]:https://www.javatpoint.com/software-engineering-coupling-and-cohesion
[^2]:https://www.geeksforgeeks.org/software-engineering-coupling-and-cohesion/
[^3]:https://www.scaler.com/topics/software-engineering/design-strategies-in-software-engineering/
[^4]:https://www.simplilearn.com/top-down-approach-vs-bottom-up-approach-article#:~:text=The%20main%20difference%20between%20the,the%20development%20of%20detailed%20knowledge
[^5]:https://www.scaler.com/topics/software-engineering/design-strategies-in-software-engineering/
[^6]:https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-class-diagram/
[^7]:https://datatrained.com/post/four-pillars-of-oops/#:~:text=The%20Four%20pillars%20of%20OOPs%2C%20abstraction%2C%20encapsulation%2C%20inheritance%2C,great%20choice%20for%20software%20development
[^8]:https://www.tutorialspoint.com/design_pattern/strategy_pattern.htm
