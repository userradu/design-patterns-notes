**The one constant in software development is change**

Identify the aspects of your application that vary and separate them from what stays the same.
Take what varies and "encapsulate" it so it won't affect the rest of your code => fewer unintended consequences from code changes and more flexibility in your systems.

Program to an interface, not an implementation.
"Program to an interface" really means "Program to a supertype".

Favor composition over inheritance. This gives you more flexibility and it also lets you change the behavior at runtime. 

Strive for loosely coupled design between objects that interact.

The Open/Closed Principle: classes should be open for extension, but closes for modification.
What do we get if we acomplish this? Designs that are resilient to change and flexible enough to take on new functionality to meet changing requirements. 
