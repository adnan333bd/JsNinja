How do you test whether an object has access to a particular
property?

----------------------------------------------------------------

For own property : 

if(Object.prototype.hasOwnProperty.call(object, "prop_name")) 
{ }
// https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwnProperty


To include inherited properties in the finding: 
 
if(prop in object) { } // https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/in


Why is a prototype chain important for working with
objects in JavaScript?

------------------------------------------------------------
