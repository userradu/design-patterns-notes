# The Decorator Pattern

The Decorator Pattern attaches additional responsabilities to an object dynamically. Decorators provide a flexible alternative to subclassing for extending functionality. 

Decorators have the same supertype as the objects they decorate. 

The decorator adds its own behavior either before and/or after delegating to the object it decorates to do the rest of the job.

Objects can be decorated at any time, so we can decorate objects dynamically at runtime with as many decorators as we like. 

Think of decorator objects as wrappers.
