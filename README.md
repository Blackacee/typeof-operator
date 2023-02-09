# typeof-operator

// returns 'number'
typeof 3.14;
typeof Infinity;
typeof NaN; // "Not-a-Number" is a "number"
// returns 'string'
typeof "";
typeof "bla";
typeof (typeof 1); // typeof always returns a string
// returns 'boolean'
typeof true;
typeof false;
// returns 'undefined'
typeof undefined;
typeof declaredButUndefinedVariable;
typeof undeclaredVariable;
typeof void 0;
typeof document.all // see above
// returns 'function'
typeof function(){};
typeof class C {};
typeof Math.sin;
// returns 'object'
typeof { /*<...>*/ };
typeof null;
typeof /regex/; // This is also considered an object
typeof [1, 2, 4]; // use Array.isArray or Object.prototype.toString.call.
typeof new Date();
typeof new RegExp();
typeof new Boolean(true); // Don't use!
typeof new Number(1); // Don't use!
typeof new String("abc"); // Don't use!
// returns 'symbol'
typeof Symbol();
typeof Symbol.iterator;
