HTTP1.1
**There is head of line blocking that blocks
 all the requests behind it until it doesn't get its all resource.
**It works on the textual format
**relies on the transport layer to avoid buffer overflow, so each new TCP connection requires a separate flow control mechanism.
**pipelining (the second request is sent before the response to the first is adequately served)
**content negotiation (an exchange between client and server to determine the media type, it also provides the provision to serve different versions of a resource at the same URI)
**cache control (used to specify caching policies in both requests and responses)
**Introduces a warning header field to carry additional information about the status of a message. Can define 24 status codes, error reporting is quicker and more efficient.




HTTP2
**It allows multiplexing so one TCP connection is required for multiple requests.
** It works on the binary protocol.
**It introduces the concept of a server push where the server anticipates the resources that will be required by the client and pushes them prior to the client making requests. The client retains the authority to deny the server push; however, in most cases, this feature adds a lot of efficiency to the process
**Underlying semantics of HTTP such as headers, status codes remains the same.





Write a blog about objects and its internal representation in Javascript
**Objects, in JavaScript, is it’s most important data-type and forms the building blocks for modern JavaScript.

**These objects are quite different from JavaScript’s primitive data-types(Number, String, Boolean, null, undefined and symbol) in the sense that while these primitive data-types all store a single value each (depending on their types)
**Every object has some property associated with some value. These values can be accessed using these properties associated with them.
**The syntax for adding a property to an object is :
ObjectName.ObjectProperty = propertyValue;
**create a javascript object is object literal, simply define the property and values inside curly braces as shown below
let bike = {name: 'SuperSport', maker:'Ducati'}
