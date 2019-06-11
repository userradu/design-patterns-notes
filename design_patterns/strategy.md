# Strategy

Defines a family of algorithms, encapsulate each one, and makes them interchangeable.
Strategy lets the algorithm vary independently from clients that use it. 

It enables selecting al algorithm at runtime. Instead of implementing a single algorithm directly, code receives run-time instructions as to which in a family of algorithms to use.

A class that performs validation on incoming data may use the strategy pattern to select a validation algorithm depending on the type of data, or other factors. These factors are not known until run-time.
The validation algorithms are encapsulated separately from the validating object and may be used by other objects without code duplication. 

According to the strategy pattern, the behaviors of a class should not be inherited. Instead they should be encapsulated using interfaces => this is compatible with the **open/closed principle**. 

The strategy pattern uses composition instead of inheritance.
The behaviors are defined as separate interfaces and specific classes that implement these interfaces. This allows better decoupling between the behavior and the class that uses the behavior => the behavior can be changed without breaking the class that use it. Behaviors can be changed at run-time as well as at design-time.
