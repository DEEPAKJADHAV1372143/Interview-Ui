Here’s a **comprehensive set of 50 JavaScript interview questions with clear answers**, organized by category so you can revise efficiently.  

---

## 🔹 Core Basics
1. **What are the different data types in JavaScript?**  
   Primitive: string, number, boolean, null, undefined, symbol, bigint.  
   Non-primitive: objects, arrays, functions.  

2. **Difference between `var`, `let`, and `const`?**  
   - `var`: function-scoped, hoisted.  
   - `let`: block-scoped, mutable.  
   - `const`: block-scoped, immutable reference.  

3. **Explain hoisting.**  
   Variable and function declarations are moved to the top of scope during compilation.  

4. **Difference between `==` and `===`?**  
   - `==`: loose equality (performs type coercion).  
   - `===`: strict equality (no coercion).  

5. **What is a closure?**  
   A function that remembers variables from its outer scope even after that scope has finished.  

---

## 🔹 Functions & Objects
6. **Difference between function declaration and function expression?**  
   Declaration is hoisted, expression is not.  

7. **Arrow functions vs normal functions?**  
   Arrow functions don’t have their own `this`, shorter syntax.  

8. **Difference between call, apply, and bind?**  
   - `call`: invokes with arguments.  
   - `apply`: invokes with array of arguments.  
   - `bind`: returns new function with bound `this`.  

9. **What is an IIFE?**  
   Immediately Invoked Function Expression — runs as soon as defined.  

10. **What are pure functions?**  
   Functions with no side effects, same output for same input.  

---

## 🔹 Asynchronous JavaScript
11. **Difference between synchronous and asynchronous code?**  
   Sync executes line by line, async allows non-blocking operations.  

12. **Explain the event loop.**  
   Handles async tasks by moving callbacks from queue to call stack.  

13. **Microtasks vs macrotasks?**  
   Microtasks (Promises) run before macrotasks (setTimeout).  

14. **Difference between callbacks, promises, and async/await?**  
   - Callbacks: nested functions.  
   - Promises: chainable async results.  
   - Async/await: cleaner syntax for promises.  

15. **What is callback hell?**  
   Nested callbacks making code unreadable. Avoided using promises/async-await.  

---

## 🔹 DOM & BOM
16. **Difference between `document.querySelector` and `getElementById`?**  
   `querySelector` selects first match with CSS selector, `getElementById` selects by ID only.  

17. **Explain event bubbling and capturing.**  
   Bubbling: event propagates upward. Capturing: event propagates downward.  

18. **What is event delegation?**  
   Attaching event listener to parent to handle child events.  

19. **Difference between `innerHTML`, `innerText`, and `textContent`?**  
   - `innerHTML`: includes HTML markup.  
   - `innerText`: visible text only.  
   - `textContent`: all text, including hidden.  

20. **Difference between localStorage, sessionStorage, and cookies?**  
   - localStorage: persists until cleared.  
   - sessionStorage: cleared on tab close.  
   - cookies: sent to server with requests.  

---

## 🔹 Advanced Concepts
21. **What are ES6 features?**  
   Let/const, arrow functions, classes, template literals, modules, promises, destructuring.  

22. **Explain destructuring.**  
   Extracting values from arrays/objects into variables.  

23. **Difference between `Map` and `Set`?**  
   - Map: key-value pairs.  
   - Set: unique values only.  

24. **What are generator functions?**  
   Functions that yield values using `yield` keyword, can pause/resume.  

25. **What is memoization?**  
   Caching results of expensive function calls.  

26. **Explain currying.**  
   Breaking function with multiple arguments into nested single-argument functions.  

27. **Difference between mutable and immutable data?**  
   Mutable can be changed (objects), immutable cannot (strings).  

28. **What are symbols in JavaScript?**  
   Unique identifiers, often used as object keys.  

29. **Explain polyfills.**  
   Code that implements modern features in older browsers.  

30. **Difference between CommonJS and ES6 modules?**  
   CommonJS uses `require`, ES6 uses `import/export`.  

---

## 🔹 Practical & Performance
31. **What is debouncing?**  
   Delays function execution until after a pause in events.  

32. **What is throttling?**  
   Limits function execution to once per interval.  

33. **Difference between `setTimeout` and `setInterval`?**  
   Timeout runs once, Interval runs repeatedly.  

34. **Difference between `process.nextTick()` and `setImmediate()` (Node.js)?**  
   `nextTick` runs before next event loop, `setImmediate` runs after.  

35. **What is the difference between shallow copy and deep copy?**  
   Shallow copies references, deep copies entire structure.  

36. **Difference between `Object.freeze()` and `Object.seal()`?**  
   Freeze prevents changes, Seal allows property value changes but no new properties.  

37. **What is optional chaining?**  
   Safely access nested properties: `obj?.prop?.subProp`.  

38. **What is nullish coalescing (`??`)?**  
   Returns right-hand value only if left is null/undefined.  

39. **Difference between `== null` and `=== null`?**  
   `== null` matches null or undefined, `=== null` matches only null.  

40. **What is the difference between `typeof` and `instanceof`?**  
   - `typeof`: returns type string.  
   - `instanceof`: checks prototype chain.  

---

## 🔹 Modern JavaScript
41. **What is a promise chain?**  
   Linking `.then()` calls to handle sequential async tasks.  

42. **Difference between `Promise.all` and `Promise.race`?**  
   - All: resolves when all promises resolve.  
   - Race: resolves when first promise resolves.  

43. **What is `Promise.any`?**  
   Resolves when any promise resolves, rejects only if all reject.  

44. **What is `Promise.allSettled`?**  
   Returns results of all promises regardless of success/failure.  

45. **What is the difference between `for...in` and `for...of`?**  
   - `for...in`: iterates keys.  
   - `for...of`: iterates values.  

46. **What is the difference between `Object.keys()`, `Object.values()`, and `Object.entries()`?**  
   Keys = property names, Values = property values, Entries = key-value pairs.  

47. **What is the difference between synchronous iteration and asynchronous iteration?**  
   Sync uses `for...of`, async uses `for await...of`.  

48. **What is a Proxy in JavaScript?**  
   Object that intercepts operations (get, set) with custom behavior.  

49. **What is the difference between `undefined` and `not defined`?**  
   - Undefined: variable declared but not assigned.  
   - Not defined: variable never declared.  

50. **What is the difference between `NaN` and `isNaN()`?**  
   - NaN: “Not a Number” value.  
   - isNaN(): checks if value is NaN.  

-
