# The State Pattern

Allows an object to alter its behavior when its internal state changes. The object will appear to change its class. 

The pattern encapsulates state into separate classes and delegates to the object representing the current state, we know that behavior changes along with the internal state. 

*appear to change its class*
- think from the perspective of a client: if an object you're using can completely change its behavior, then it appears to you that the object is actually instantiated from another class. In reality, however, you know that we are using composition to give the appearance of a class change by simply referencing different state objects. 

**Strategy vs State**

State Pattern
- you have a set of behaviors encapsulated in state objects; at any time the context is delegating to one of those states.
- the client usually knows very little, if anything, about the state objects.
- think of the State Pattern as an alternative to putting lots of conditionals in your context; by encapsulating the behavior within state objects, you can simply change the state object in context to change its behavior. 

Strategy Pattern
- the client usually specifies the strategy object that the context is composed with.
- think of the Strategy Pattern as a flexible alternative to subclassing; if you use inheritance to define the behavior of a class, then you're stuck with that behavior even if you need to change it. With Strategy you can change the behavior by composing with a different object. 
