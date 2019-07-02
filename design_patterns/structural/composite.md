# The Composite Pattern

Allows to compose objects into tree structures to represent part-whole hierarchies.
Composite lets clients treat individual objects and composition of objects uniformly.

The Composite Pattern allows us to build structures of objects in the form of trees that contain both compositons of objects and individual objects as nodes. 

Using a composite structure, we can apply the same operations over both composite and individual objects. In other words, in mose cases we can *ignore* the difference between composition of objects and individual objects.

**Component, Composite, Trees**

A composite contains components.
Components come in 2 flavors: composites and leaf elements
A composite holds a set of children, those children may be other composites or leaf nodes.  

Use this pattern when you have collections of objects with whole-part relationships and you want to be able to treat those objects uniformly. 

Simplify the life for clients: the clients don't have to worry whether they are dealing with a composite object or a leaf object, so they don't have to write if statements everywhere to make sure they're calling the right methods on the right objects. 
