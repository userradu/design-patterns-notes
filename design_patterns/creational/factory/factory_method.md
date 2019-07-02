# Factory method

Encapsulates object creation by letting subclasses decide what objects to create.

It defines an interface for creating an object, but lets subclasses decide which class to instantiate.
Factory method lets a class defer instantiation to subclasses.

Factory method is to creating objects as Template Method is to implementing an algorithm. A superclass specifies all standard and generic behavior and then delegates the creation details to subclasses that are supplied by the client.

Uses inheritance: object creation is delegated to subclasses which implement the factory method to create object.  
