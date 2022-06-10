# day-02-
Difference between HTTP1.1 vs HTTP2  
 HTTP/1.1 – (The standardized protocol More than 15 years of extensions)
Ithe usest works on the textual format.
There is head of line blocking that blocks all the requests behind it until it doesn’t get its all resources.
It uses requests resource Inlining for use getting multiple pages
It compresses data by itself.
 It supports connection reuse i.e. for every TCP connection there could be multiple requests and responses, and pipelining where the client can request several resources from the server at once. However, pipelining was hard to implement due to issues such as head-of-line blocking and was not a feasible solution.
 
HTTP/2 – (A protocol for greater performance)
HTTP2 is much faster and more reliable than HTTP1.
It works on the binary protocol.
It allows multiplexing so one TCP connection is required for multiple requests.
It uses PUSH frame by server that collects all multiple pages 
it uses HPACK for data compression.
 Uses multiplexing, where over a single TCP connection resources to be delivered are interleaved and arrive at the client almost at the same time. It is done using streams which can be prioritized, can have dependencies and individual flow control. It also provides a feature called server push that allows the server to send data that the client will need but has not yet requested.

[objects and its internal representation in Javascript]
In simple terms. “A JavaScript object is a collection of named values having state and behavior (properties and method)”.
example
var player ="ronaldo";
Objects are variables too. But objects can contain many values.

The following code assigns many values (ronaldo ,speed,jump) to a variable named player:
var car = {Make: “ronaldo”, Color: “White”, Fuel: Diesel, Weight: “65kg”, Rating: 4.5};
The values are written as name:value pairs (name and value separated by a colon).

Syntax:

var <object-name> = {key1: value1, key2: value2,... keyN: valueN};
So, conclusion and definition for JS objects is “JavaScript objects are containers for named values”.
  
  2)Object Properties
  The name:values pairs (in JavaScript objects) are called properties.
  The object properties can be different primitive values, other objects and functions.

Properties can usually be changed, added, and deleted, but some are read only.

The syntax for adding a property to an object is :

ObjectName.ObjectProperty = propertyValue;
  So, Conclusion and simple definition for Java Script properties is “Properties are the values associated with a JavaScript object”.
  
  3)Object Methods
An object method is an object property containing a function definition.

i.e.,

Let’s assume to start the car there will be a mechanical functionality
  function(){return ignition.on}
  So, Conclusion and simple definition for Java Script Object methods is “Methods are actions that can be performed on objects.”.
