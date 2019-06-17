**The one constant in software development is change**

Identify the aspects of your application that vary and separate them from what stays the same.
Take what varies and "encapsulate" it so it won't affect the rest of your code => fewer unintended consequences from code changes and more flexibility in your systems.

Program to an interface, not an implementation.
"Program to an interface" really means "Program to a supertype".

Favor composition over inheritance. This gives you more flexibility and it also lets you change the behavior at runtime. 

Strive for loosely coupled design between objects that interact.

The Open/Closed Principle: classes should be open for extension, but closes for modification.
What do we get if we acomplish this? Designs that are resilient to change and flexible enough to take on new functionality to meet changing requirements. 

**Dependency inversion principle**
Depend upon abstractions. Do not depend upon concrete classes. 
High-level components should not depend on low-level components; rather, they should both depend on abstractions(interfaces). 
A *high-level component* is a class with behavior defined in terms of other, *low-level components*.
A system where each module specifically refers to its collaborators is a tight coupled system, *it lacks sufficient layers of abstractions*.
**The goal** of the dependency inversion principle is to avoid a high coupled distribution with the mediation of an abstract layer, and to increase the reusability of higher components.

**Why is tight-coupling bad?**
Software changes all the time. You want to be able to modify a module without having to change all other modules which are dependent on this first module. 

Practical example:
If somebody wants their output in a CSV file rather than JSON etc., or if you want to switch from MySQL to PostGreSQL you should be able to make those changes extremely easily in your code, without having to rewrite the entire class etc. In other words, you do not want to tightly couple your application with a specific database implementation (e.g. Mysql) or to a particular output (e.g. CSV files). Because, as is inevitable in software, changes will come. When they do come, it's much easier if your parts of your code are loosely coupled. 

**The principle of Least Knowledge**
- talk only to your immediate friends
- this principle prevents us from creating designs that have a large number of classes coupled together so that changes in one part of the system cascade to other pats. - when you build a lot of dependencies between many classes, you are building a fragile system that will be costly to maintain and complex for others to understand. 

**The Hollywood Principle: Don't call us, we'll call you**
- gives us a way to prevent "dependency rot". Dependency rot hapens when you have high-level components depending on low-level components depending on high-level components depending on sideways components depending on low-level components and so on. When rot sets in, no one can easely understand the way a system is designed. 
- with the Hollywood principle, we allow low-level components to hook themselves into a system, but the high-level components determine when they are needed, and how. In other words, the high-level components give the low-level components a "don't call us, we'll call you" treatment. 
- principle defined with the *Template Method Pattern*
