Basic
=====

unlike other languages， Javascript's variable only have scope types: global scope, function scope. check the following code

```javascript
var global = "hello"; // global scope variable

function test_scope() {
  var local = "world"; // local scope variable
}
```

Some features about variable scope in Javascript:
1. no block scope, not like other languages
2. variable hoisting
3. scope chain, related to search for variables

### no block scope

```javascript
if (some_condition) {
  var e = "hello";
}

// code above equals to
 var e;

 if (some_condition) {
  e = "hello";
 }
//
```

### variable hoisting

// see the above demo

### scope chain

Similar to object inheritance OO (Object Oriented), Javascript use scope chain to find variables. When executing code in no function, scope chain has only one node. When in a function, scope chain has two node: global node and corresponding function node, when in a function which is inside another function, scope chain is compositing of three: global node, outside function scope node and nested function scope node.

Some Questions
====

1. [In what scope are module variables stored in node.js?](http://stackoverflow.com/questions/15406062/in-what-scope-are-module-variables-stored-in-node-js)

>Unlike the browser, where variables are by default assigned to the global space \(i.e. window\), in Node variables are scoped to the module \(the file\) unless you explicitly assign them to module.exports.

2. [What is the scope of variables in JavaScript?](http://stackoverflow.com/questions/500431/what-is-the-scope-of-variables-in-javascript)


