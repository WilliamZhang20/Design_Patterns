# Design_Patterns

Practicing useful software design patterns in C++. 
Current list:

1. Singleton Design Pattern

Ensures that only one instance of a class exists, such as in the case of a government, a gaming engine, or a company name, etc. It is implemented by maintaining the only instance as a private and static member which can only be accessed via a static method. The constructor is also kept private. To ensure thread safety against copying, accessibility of the singleton instance is locked with a mutex. 

2. Factory Method

Introduces flexible object creation for different class requirements. This is done by defining an abstract class for the created object, aka a product. The actual products will inherit from the abstract product. To create different products, the client will call methods of different 'factories'. These factory classes all inherit from an abstract factory. 

3. Adapter Design Pattern

Provides a wrapper to convert one interface into another, such as a legacy to a new, or more simply, a round peg to a square hole. This wrapper inherits extends the desired/target interface and internally calls the adaptee's interface. For example, in square pegs and circular holes, the adapter calls width of a square when the radius of a desired circule is called.