# The Iterator Pattern

Provides a way to access the elements of an aggregate object sequentially without exposing its underlying representation. 

The pattern gives you a way to step through the elements of an aggregate without having to know how things are represented under the covers. 

The Iterator Pattern takes the responsability of traversing elements and gives the responsability to the iterator object, not the aggregate object. This not only keeps the aggregate interface and implementation simpler, it removes the responsability for iteration from the aggregate and keeps the aggregate focused on the things it should be focuses on (managing a collection of objects), not on iteration. 
