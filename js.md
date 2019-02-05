## 1. typeof bar === 'object'

null === 'object => true

function() === 'object => false

array === 'object => true

## 2. 'use strict'

The short and most important answer here is that use strict is a way to voluntarily enforce stricter parsing and error handling on your JavaScript code at runtime. Code errors that would otherwise have been ignored or would have failed silently will now generate errors or throw exceptions.
    
  * makes debugging easier

  * prevents polluting global

  * disallow duplicates

## 3. return statement

```
function foo1()
{
  return {
      bar: "hello"
  };
}

function foo2()
{
  return
  {
      bar: "hello"
  };
}
```

foo1() returns the object, foo2() returns undefined. When the line containing the return statement (with nothing else on the line) is encountered in foo2(), a semicolon is automatically inserted immediately after the return statement.

## 4. NaN

* typeof NaN => Number

* NaN === NaN => false

Use isNaN() or Number.isNaN() to determine NaN.


