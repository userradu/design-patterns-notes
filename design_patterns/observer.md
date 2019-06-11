# Observer

Defines a one-to-many dependency between objects so that when one object changes state, all of its dependent are notified and updated automatically. 

The Subject interface
- objects use this interface to register as observers and also to remove themselves from being observers.
- a concrete subject implements a notifyObservers() method that is used to update all the current observers when state changes.

The Observer interface
- this interface has one method, update() that gets called when the Subject's state changes. 

The Observer Pattern provides an object design where subjects and observers are loosely coupled. 

We can add new observers at any time. 
