# Javascript 
Things I wanted to know more about, or had a question about, relating to JS.

## jsx
JSX => Javascript XML. Extension to JS, XML like. Comes down to nested functions. Created orginally by facebook for React.


## closures
Closures refer to a record storing the function and the enclosed scope(environment). A closure gives the function access to it's outer (parent) scope.

A closure is a persistant local variable scope, even after the code execution has moved through that block of code, provided a reference to it has been kept.

```
outer = function() {
	var a = 1;
	var inner = function() {
		console.log(a);
	}
	return inner
}

var fnc = outer();
fnc();
```

The function `outer` contains the function `inner` which has access to the local variable `a`. Normally when a function exits all it's local variables are blown away. However, by returning the `inner` function and assigning it to the variable `fnc` so it persists, the local variable assigned when `inner` was defined also persist. *The variable `a` is within a closure* and is private (closed off) to `fnc`. `a` belongs to the scope of `outer`, `inner`'s scope points to `outer`'s scope as it's parent, `fnc` is a variable that points to `inner`. `a` persists as long as `fnc` does. `a` is within the closure.

Functions are useful as they let you associated data with a function that acts on that data. In javascript and web development it's super useful as you are often writing event based code. When an event (ie user click) triggers some behaviour, code is attached as a callback, a function defining the response to the event.

## spread operator

*What is the spread operator?* 
Spread syntax can be used when all elements from an object or array need to be included in a new array or object, or should be applied one-by-one in a function call's arguments list.

*List 4 things that the spread operator can do.*
 1. Function arguments list `(myFunction(a, ...iterableObj, b))`
 2. Array literals `([1, ...iterableObj, '4', 'five', 6])`
 3. Object literals `({ ...obj, key: 'value' })`

*Give an example of using the spread operator to combine two arrays.*

```
let arr1 = [0, 1, 2];
const arr2 = [3, 4, 5];

arr1 = [...arr2, ...arr1];
```

*Give an example of using the spread operator to add a new item to an array.*
```
const isSummer = false;
const fruits = ["apple", "banana", ...(isSummer ? ["watermelon"] : [])];
```
*Give an example of using the spread operator to combine two objects into one.*
```
const obj1 = { foo: "bar", x: 42 };
const obj2 = { bar: "baz", y: 13 };

const mergedObj = { ...obj1, ...obj2 };
```