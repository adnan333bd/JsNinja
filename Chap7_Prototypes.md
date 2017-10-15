How do you test whether an object has access to a particular
property?
------------------------------------------------------------

For own property : 

if(Object.prototype.hasOwnProperty.call(object, "prop_name")) 
{ }
// https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwnProperty


To include inherited properties in the finding: 
 
if(prop in object) { } // https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/in

Note: One may be tempted to use typeof and [ ] property accessor as the following code which doesn't work ...

var loan = { amount: 150 };

loan.installment = undefined;

if("installment" in loan) // correct
{
    // will execute
}

if(typeof loan["installment"] !== "undefined") // incorrect
{
    // will not execute
}


Why is a prototype chain important for working with
objects in JavaScript?
----------------------------------------------------









Do ES6 classes change how JavaScript works with objects?
--------------------------------------------------------
