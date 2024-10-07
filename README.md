1.Write a blog on Difference between HTTP1.1 vs HTTP2

HTTP/1.1 -

1.development of HTTP but we will focus mainly on HTTP/1.1 which was created in 1997

2.It works on the textual format

3.There is head of line blocking that blocks all the requests behind it until it doesn’t get its all resources.

4.There is head of line blocking that blocks all the requests behind it until it doesn’t get its all resources.

5.It compresses data by itself.

6.HTTP/1.1: For better understanding, let’s assume the situation when you make a request to the server for the geeksforgeeks.html page & server responds to you as a resource geeksforgeeks.html page. before sending the request and the response there is a TCP connection established between client & server. 
  again you make a request to the server for image img.jpg & the server gives a response as an image img.jpg. the connection was not lost here after the first request because we add a keep-alive header which is the part of the request so there is an open connection between the server & client. there is a persistent connection which means several requests & responses are merged in a single connection.

HTTP/2 -

1.development of HTTP new one is HTTP/2 which was created in 2015.

2.It works on the binary protocol.

3.It allows multiplexing so one TCP connection is required for multiple requests.

4.It uses PUSH frame by server that collects all multiple pages.

5.It uses HPACK for data compression.

6.HTTP/2: HTTP/2 was developed over the SPDY protocol. HTTP/2 works on the binary framing layer instead of textual that converts all the messages in binary format.
  it works on fully multiplexed that is one TCP connection is used for multiple requests. HTTP/2 uses HPACK which is used to split data from header. it compresses the header. The server sends all the other files like CSS & JS without the request of the client using the PUSH frame.

  

2.Write a blog about objects and its internal representation in Javascript

blog about objects and its internal representation in Javascript

Objects are important data types in javascript. Objects are different than primitive datatypes (i.e. number, string, boolean, etc.). Primitive data types contain one value but Objects can hold many values in form of Key: value pair. These keys can be variables or functions and are called properties and methods, respectively, in the context of an object.

Objects, in JavaScript, is it’s most important data-type and forms the building blocks for modern JavaScript. These objects are quite different from JavaScript’s primitive data-types(Number, String, Boolean, null, undefined and symbol) in the sense that while these primitive data-types all store a single value each (depending on their types).

Objects are more complex and each object may contain any combination of these primitive data-types as well as reference data-types.
An object, is a reference data type. Variables that are assigned a reference value are given a reference or a pointer to that value. That reference or pointer points to the location in memory where the object is stored. The variables don’t actually store the value.

Loosely speaking, objects in JavaScript may be defined as an unordered collection of related data, of primitive or reference types, in the form of “key: value” pairs. These keys can be variables or functions and are called properties and methods, respectively, in the context of an object.

Objects and properties
A JavaScript object has properties associated with it. A property of an object can be explained as a variable that is attached to the object. Object properties are basically the same as ordinary JavaScript variables, except for the attachment to objects. The properties of an object define the characteristics of the object. You access the properties of an object with a simple dot-notation:

objectName.propertyName
Create JavaScript Object with Object Literal
One of easiest way to create a javascript object is object literal, simply define the property and values inside curly braces as shown below

let bike = {name: 'SuperSport', maker:'BMW s1000rr', engine:'999cc'};
Understanding Objects in JavaScript
In JavaScript, objects are collections of key-value pairs, where keys are strings (or symbols) and values can be of any data type, including other objects. Objects are used to represent real-world entities, data structures, and more complex data types.


const person = {
  name: "Mani M",
  age: 22,
  email: "manicivil@gmail.com"
};
Internal Representation of Objects
Internally, JavaScript engines use various data structures to represent objects efficiently. One common approach is using a hash table or a similar structure to store the object’s properties and their corresponding values. This allows for fast access and manipulation of properties.

Internal Representation:
{
  name: "Mani M",
  age: 22,
  email: "manicivil@gmail.com"
}
