# The Proxy Pattern

The role of proxies is to control and manage access

A remote proxy acts as a *local representative to a remote object*.

Use the Proxy Pattern to create representative object that control access toa another object which may be remote, expensive to create or in need of securing.

Remote Proxy
- the proxy acts as a local representative for an object that lives in a different JVM. A method call on the proxy results in the call being transferred over the wire, invoked remotely, and the result being returned back to the proxy and then to the Client.

Virtual Proxy
- acts as a representative for an object that may be expensive to create.
- the virtual proxy often deffers the creation of the object until it is needed. 
- the virtual proxy also acts as a surrogate for the object before and while it is being created. After that, the proxy delegates requests directly to the real subject.
- a virtual proxy can create objects (subjects) as well.

Protection Proxy
- a proxy that controls access to an object based on access rights. 
