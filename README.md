# TypeScript: Object is possibly 'undefined' with string | null parameter

This example demonstrates a common TypeScript error related to type guards and optional parameters.  The `printName` function accepts a parameter that can be a string or null.  While a null check is performed, passing `undefined` results in a type error because TypeScript's type system doesn't automatically narrow `undefined` to `null` in this case.

The solution involves either explicitly handling `undefined` or changing the function's parameter type.