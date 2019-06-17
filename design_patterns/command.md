# The Command Pattern

Encapsulates a request as an object, thereby letting you parameterize other objects with different requests, queue or log requests, and support undoable operations. 

When you need to decouple an object making requests from the object that know how to perform the requests, use the Command Pattern. 

The following types of objects are being used by this pattern:

**Command**
- knows about the *receiver* and invokes a method on the receiver. 
- exposes a method called *execute()*

**Receiver**
- does the work when the *execute()* method in the *command* is called. 

**Invoker**
- knows how to execute a *command*
- does not know anything about a concrete command, it knows only about the command *interface*

**Client**
- invoker objects, command objects and receiver objects are held by a client object
- the client decides which receiver object it assigns to the command objects, and which commands it assigns to the invoker. 
- the client decides which commands to execute at which points. 
- to execute a command, it passes the command object to the invoker object. 
