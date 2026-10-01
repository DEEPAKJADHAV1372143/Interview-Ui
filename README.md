# Interview-Ui


## 🔹 Core Basics
1. **What is HTML?**  
   A markup language for structuring web content.  

2. **Difference between HTML and HTML5?**  
   HTML5 adds semantic tags, multimedia support, canvas/SVG, and APIs.  

3. **Basic structure of an HTML document?**  
   `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`.  

4. **Difference between a tag and an element?**  
   Tag = markup (`<p>`), Element = tag + content (`<p>Hello</p>`).  

5. **What are attributes in HTML?**  
   Extra info for elements, e.g., `<img src="pic.jpg" alt="text">`.  

---

## 🔹 Semantic & Accessibility
6. **What are semantic elements?**  
   `<header>`, `<footer>`, `<article>` — describe meaning.  

7. **Why is `alt` important in `<img>`?**  
   Accessibility for screen readers, fallback text.  

8. **Difference between `em`/`strong` vs `i`/`b`?**  
   `em`/`strong` = semantic emphasis, `i`/`b` = stylistic.  

9. **What is ARIA in HTML?**  
   Attributes that improve accessibility for assistive tech.  

10. **How does HTML affect SEO?**  
   Proper headings, semantic tags, metadata, alt text.  

---

## 🔹 Forms & Inputs
11. **New input types in HTML5?**  
   `email`, `date`, `number`, `range`.  

12. **Built-in validation attributes?**  
   `required`, `pattern`, `min`, `max`.  

13. **Difference between `placeholder` and `label`?**  
   Label = permanent, Placeholder = temporary hint.  

14. **What is `<datalist>` used for?**  
   Provides autocomplete options for inputs.  

15. **Difference between GET and POST in forms?**  
   GET appends data to URL, POST sends in body.  

---

## 🔹 Multimedia & Graphics
16. **Difference between `<audio>` and `<video>`?**  
   `<audio>` plays sound, `<video>` plays video.  

17. **Purpose of `<track>` in `<video>`?**  
   Adds subtitles/captions.  

18. **What is `<canvas>` used for?**  
   Drawing graphics/animations via JS.  

19. **Difference between `<canvas>` and `<svg>`?**  
   Canvas = pixel-based, SVG = vector-based.  

20. **Difference between inline SVG and external SVG?**  
   Inline = manipulable with CSS/JS, external = static.  

---

## 🔹 Storage & APIs
21. **Difference between localStorage and sessionStorage?**  
   localStorage persists, sessionStorage clears on tab close.  

22. **What is Web Storage API?**  
   Provides key-value storage in browser.  

23. **What is Geolocation API in HTML5?**  
   Retrieves user’s location with permission.  

24. **What is the difference between cookies and localStorage?**  
   Cookies sent to server, localStorage stays client-side.  

25. **What is a PWA (Progressive Web App)?**  
   HTML + service workers + manifest, works offline, installable.  

---

## 🔹 Performance & Best Practices
26. **How to optimize HTML performance?**  
   Lazy-load images, minify HTML, semantic tags, reduce DOM size.  

27. **Difference between inline, block, and inline-block elements?**  
   Inline = same line, Block = new line full width, Inline-block = inline but allows width/height.  

28. **Difference between `<link>` and `<a>`?**  
   `<link>` defines relationships (CSS), `<a>` creates hyperlinks.  

29. **Difference between `<script>` in head vs body?**  
   Head blocks rendering, body loads after content.  

30. **Difference between async and defer in `<script>`?**  
   Async executes immediately, Defer waits until parsing ends.  

---

## 🔹 Browser Behavior & Security
31. **What is `<!DOCTYPE html>`?**  
   Declares HTML5, triggers standards mode.  

32. **Difference between quirks mode and standards mode?**  
   Quirks = old browser behavior, Standards = modern specs.  

33. **What is the sandbox attribute in `<iframe>`?**  
   Restricts iframe capabilities (scripts, forms, etc.).  

34. **Security practices in HTML?**  
   Use `rel="noopener noreferrer"`, sanitize inputs, avoid inline JS.  

35. **Difference between relative, absolute, and fixed paths?**  
   Relative = current file, Absolute = root, Fixed = external URL.  

---

## 🔹 Advanced & Practical
36. **What is the DOM?**  
   Browser-generated tree of HTML, manipulated via JS.  

37. **Difference between innerHTML and textContent?**  
   innerHTML returns markup, textContent returns plain text.  

38. **What happens if you forget to close a tag?**  
   Browser auto-corrects, layout may break.  

39. **Difference between `<noscript>` and JS fallback?**  
   `<noscript>` shows content when JS disabled, fallback handled in JS.  

40. **How does the browser parse HTML?**  
   Tokenization → DOM tree → CSSOM → Render tree → Layout → Paint.  

---

=======================================
## 🔹 CSS Fundamentals
1. **What is CSS?**  
   Cascading Style Sheets control the presentation of HTML elements.  

2. **Difference between inline, internal, and external CSS?**  
   - Inline: inside element (`style=""`).  
   - Internal: inside `<style>` tag in HTML.  
   - External: linked via `.css` file.  

3. **What are pseudo-classes in CSS?**  
   Special states of elements, e.g., `:hover`, `:focus`, `:nth-child()`.  

4. **Difference between relative, absolute, and fixed positioning?**  
   - Relative: positioned relative to itself.  
   - Absolute: relative to nearest positioned ancestor.  
   - Fixed: relative to viewport.  

5. **What is the difference between inline vs block elements in CSS?**  
   Inline doesn’t start a new line, block takes full width.  

---

## 🔹 Selectors & Specificity
6. **What are CSS selectors?**  
   Patterns used to select elements (class, id, attribute, pseudo-class).  

7. **Difference between `id` and `class` selectors?**  
   `id` is unique (`#id`), `class` can be reused (`.class`).  

8. **What is specificity in CSS?**  
   Rules that determine which style applies: inline > id > class > element.  

9. **Difference between `>` and space in selectors?**  
   - `div > p`: selects direct child.  
   - `div p`: selects all descendants.  

10. **What is the difference between `:nth-child()` and `:nth-of-type()`?**  
   - `nth-child`: based on position among siblings.  
   - `nth-of-type`: based on element type.  

---

## 🔹 Box Model & Layout
11. **Explain the CSS box model.**  
   Content → Padding → Border → Margin.  

12. **Difference between inline vs inline-block?**  
   Inline-block allows width/height control, inline does not.  

13. **What is the difference between relative units (`em`, `%`) and absolute units (`px`)?**  
   Relative units scale with parent, absolute units are fixed.  

14. **What is the difference between `overflow: hidden`, `scroll`, and `auto`?**  
   Hidden = cut off, Scroll = always scrollbars, Auto = scrollbars only if needed.  

15. **Difference between `position: sticky` and `fixed`?**  
   Sticky = toggles between relative and fixed depending on scroll.  
   Fixed = always fixed to viewport.  

---

## 🔹 Flexbox & Grid
16. **What is Flexbox?**  
   A layout model for aligning items in rows/columns.  

17. **Difference between `justify-content` and `align-items`?**  
   - Justify-content: horizontal alignment.  
   - Align-items: vertical alignment.  

18. **Difference between `flex: 1` and `flex: auto`?**  
   - `flex: 1`: grows equally.  
   - `flex: auto`: grows but respects content size.  

19. **What is CSS Grid?**  
   A two-dimensional layout system using rows and columns.  

20. **Difference between Flexbox and Grid?**  
   Flexbox = one-dimensional, Grid = two-dimensional.  

---

## 🔹 Styling & Effects
21. **Difference between relative and absolute colors in CSS?**  
   Relative: `hsl()`, `rgba()` with transparency.  
   Absolute: `#000000`, `red`.  

22. **What is the difference between `inline-style` and CSS variables?**  
   Inline-style applies directly, CSS variables (`--var`) are reusable.  

23. **Difference between `em` and `rem` units?**  
   - `em`: relative to parent font size.  
   - `rem`: relative to root font size.  

24. **What is the difference between `opacity` and `rgba()` transparency?**  
   - `opacity`: affects entire element including children.  
   - `rgba()`: affects only color.  

25. **Difference between `transform` and `translate`?**  
   Transform applies multiple effects (rotate, scale), translate moves element.  

---

## 🔹 Responsive Design
26. **What are media queries in CSS?**  
   Rules that apply styles based on device width/height.  

27. **Difference between `min-width` and `max-width` in media queries?**  
   - Min-width: applies styles above threshold.  
   - Max-width: applies styles below threshold.  

28. **What is mobile-first design in CSS?**  
   Start with small screens, then add styles for larger screens.  

29. **Difference between relative units (`%`, `em`) and viewport units (`vw`, `vh`)?**  
   Relative units depend on parent, viewport units depend on screen size.  

30. **What is the difference between responsive and adaptive design?**  
   Responsive = fluid layouts, Adaptive = fixed breakpoints.  

---

## 🔹 Animations & Transitions
31. **Difference between CSS transitions and animations?**  
   - Transition: triggered by state change.  
   - Animation: runs continuously with keyframes.  

32. **What is the difference between `ease`, `linear`, and `ease-in-out`?**  
   Timing functions controlling speed curve.  

33. **Difference between `@keyframes` and `transition`?**  
   - Keyframes: define multiple stages.  
   - Transition: defines start and end only.  

34. **What is hardware acceleration in CSS?**  
   Using `transform: translateZ(0)` to trigger GPU rendering.  

35. **Difference between `visibility: hidden` and `display: none`?**  
   - Hidden: element invisible but takes space.  
   - None: element removed from layout.  

---

## 🔹 Advanced & Practical
36. **What is the difference between inline CSS and external CSS performance-wise?**  
   External CSS is cached, inline increases page size.  

37. **Difference between absolute, relative, and fixed units in CSS?**  
   Absolute = px, Relative = em/rem, Fixed = viewport units.  

38. **What is the difference between CSS reset and normalize.css?**  
   Reset removes all default styles, Normalize preserves useful defaults.  

39. **Difference between `clip-path` and `mask` in CSS?**  
   Clip-path defines visible area, mask uses image/gradient for visibility.  

40. **What is the difference between CSS variables and SASS variables?**  
   CSS variables are runtime, SASS variables are compile-time.




==========================================

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

---


==================================
Here’s a **comprehensive set of 50 RxJS interview questions with answers**, organized from basics to advanced so you can revise systematically.  

---

## 🔹 Core Basics
1. **What is RxJS?**  
   A library for handling asynchronous data streams using Observables.  

2. **What is an Observable?**  
   A stream that emits multiple values over time.  

3. **What is an Observer?**  
   A consumer of Observables, with `next`, `error`, and `complete` handlers.  

4. **What is a Subscription?**  
   Represents execution of an Observable; can be unsubscribed to stop receiving values.  

5. **Difference between Promise and Observable?**  
   Promise emits one value, Observable emits multiple values and is cancellable.  

---

## 🔹 Operators Basics
6. **What are RxJS operators?**  
   Functions that transform, filter, or combine streams.  

7. **Difference between `map` and `switchMap`?**  
   - `map`: transforms values.  
   - `switchMap`: switches to new Observable, cancels previous.  

8. **Difference between `mergeMap` and `concatMap`?**  
   - `mergeMap`: runs inner Observables concurrently.  
   - `concatMap`: queues Observables sequentially.  

9. **What is `exhaustMap`?**  
   Ignores new Observables until current completes.  

10. **What is `filter` operator?**  
   Emits only values that meet a condition.  

---

## 🔹 Subjects
11. **What is a Subject?**  
   Both Observable and Observer, allows multicasting.  

12. **Difference between Subject and BehaviorSubject?**  
   - Subject: emits values to subscribers.  
   - BehaviorSubject: stores last value, emits immediately to new subscribers.  

13. **What is ReplaySubject?**  
   Replays specified number of past values to new subscribers.  

14. **What is AsyncSubject?**  
   Emits only the last value when completed.  

15. **Use case of BehaviorSubject in Angular?**  
   For state management, always providing latest value.  

---

## 🔹 Error Handling
16. **How do you handle errors in RxJS?**  
   Using `catchError`, `retry`, `retryWhen`.  

17. **What is `catchError` used for?**  
   Catches errors and returns fallback Observable.  

18. **What is `retry` operator?**  
   Retries failed Observable a specified number of times.  

19. **Difference between `throwError` and `catchError`?**  
   - `throwError`: creates error Observable.  
   - `catchError`: handles errors gracefully.  

20. **What is `finalize` operator?**  
   Executes cleanup logic when Observable completes or errors.  

---

## 🔹 Combination Operators
21. **What is `combineLatest`?**  
   Combines latest values from multiple Observables.  

22. **Difference between `forkJoin` and `combineLatest`?**  
   - `forkJoin`: waits for all Observables to complete, emits last values.  
   - `combineLatest`: emits whenever any Observable emits.  

23. **What is `zip` operator?**  
   Combines values from multiple Observables in pairs.  

24. **What is `merge` operator?**  
   Merges multiple Observables into one.  

25. **What is `concat` operator?**  
   Concatenates Observables sequentially.  

---

## 🔹 Utility Operators
26. **What is `tap` operator?**  
   Performs side effects without modifying values.  

27. **What is `delay` operator?**  
   Delays emissions by specified time.  

28. **What is `debounceTime` operator?**  
   Emits value only after silence for given time.  

29. **What is `throttleTime` operator?**  
   Emits first value, then ignores subsequent values for given time.  

30. **Difference between `auditTime` and `sampleTime`?**  
   - `auditTime`: emits last value after time window.  
   - `sampleTime`: emits latest value at fixed intervals.  

---

## 🔹 Higher-Order Observables
31. **What is a higher-order Observable?**  
   An Observable that emits other Observables.  

32. **Difference between `switchMap` and `mergeMap`?**  
   - `switchMap`: cancels previous inner Observable.  
   - `mergeMap`: runs all inner Observables concurrently.  

33. **What is `concatMap` used for?**  
   Ensures Observables run sequentially.  

34. **What is `exhaustMap` used for?**  
   Prevents multiple triggers (e.g., form submissions).  

35. **What is `flatMap`?**  
   Alias for `mergeMap`.  

---

## 🔹 Multicasting
36. **What is multicasting in RxJS?**  
   Sharing one Observable execution among multiple subscribers.  

37. **What is `share` operator?**  
   Converts cold Observable to hot, shares subscription.  

38. **What is `shareReplay` operator?**  
   Shares subscription and replays last emitted values.  

39. **Difference between hot and cold Observables?**  
   - Cold: starts producing values on subscription.  
   - Hot: produces values regardless of subscription.  

40. **Example of hot Observable?**  
   DOM events, WebSocket streams.  

---

## 🔹 Angular Integration
41. **How does Angular use RxJS?**  
   For HTTP requests, reactive forms, event handling, NgRx state management.  

42. **What is `async` pipe in Angular?**  
   Subscribes to Observable/Promise and auto-unsubscribes.  

43. **Why use `takeUntil` in Angular components?**  
   To unsubscribe automatically when component is destroyed.  

44. **What is NgRx?**  
   State management library using RxJS Observables.  

45. **What is the difference between `async` pipe and manual subscription?**  
   Async pipe handles subscription/unsubscription automatically.  

---

## 🔹 Advanced & Practical
46. **What is backpressure in RxJS?**  
   Handling fast producers with slow consumers using operators like `throttleTime`.  

47. **What is `multicast` operator?**  
   Shares Observable using a Subject.  

48. **What is `windowTime` operator?**  
   Splits emissions into windows based on time.  

49. **What is `bufferTime` operator?**  
   Collects values for a time window, emits as array.  

50. **How do you prevent memory leaks in RxJS?**  
   Use `takeUntil`, `async` pipe, and proper unsubscription.  

---
=====================================
Here’s a **comprehensive set of 50 NgRx interview questions with answers**, organized by category so you can revise systematically.  

---

## 🔹 Core Concepts
1. **What is NgRx?**  
   A reactive state management library for Angular based on Redux principles.  

2. **Why use NgRx in Angular?**  
   Provides predictable state, centralized store, immutability, and debugging tools.  

3. **What is a Store in NgRx?**  
   A single source of truth holding application state.  

4. **What are Actions in NgRx?**  
   Plain objects describing events that change state.  

5. **What are Reducers in NgRx?**  
   Pure functions that take current state + action → return new state.  

---

## 🔹 Selectors & State
6. **What are Selectors?**  
   Functions to query slices of state from the store.  

7. **Difference between `createSelector` and `createFeatureSelector`?**  
   - `createFeatureSelector`: selects top-level feature state.  
   - `createSelector`: derives data from feature state.  

8. **Why use selectors instead of direct store access?**  
   Encapsulation, reusability, memoization.  

9. **What is memoization in selectors?**  
   Caches results until inputs change, improving performance.  

10. **How do you structure state in NgRx?**  
   Split into feature modules, each with its own reducer and selectors.  

---

## 🔹 Effects & Async
11. **What are Effects in NgRx?**  
   Handle side effects like API calls outside reducers.  

12. **Difference between Reducers and Effects?**  
   Reducers = pure, synchronous. Effects = async, side effects.  

13. **What is `Actions` stream in NgRx Effects?**  
   Observable of all dispatched actions.  

14. **What is `ofType` operator?**  
   Filters actions by type in effects.  

15. **How do you handle API errors in NgRx Effects?**  
   Use `catchError` and dispatch failure actions.  

---

## 🔹 Entity & Data Management
16. **What is NgRx Entity?**  
   Provides helpers for managing collections of records.  

17. **Benefits of NgRx Entity?**  
   Simplifies CRUD operations, reduces boilerplate.  

18. **Difference between `ids` and `entities` in Entity state?**  
   - `ids`: array of record IDs.  
   - `entities`: dictionary of records keyed by ID.  

19. **What is `createEntityAdapter`?**  
   Generates reducers and selectors for entity collections.  

20. **How do you update multiple entities at once?**  
   Use adapter methods like `updateMany`.  

---

## 🔹 Store Setup & Configuration
21. **How do you register a reducer in NgRx?**  
   Use `StoreModule.forRoot` or `StoreModule.forFeature`.  

22. **Difference between root store and feature store?**  
   Root store = global state, Feature store = module-specific state.  

23. **What is `EffectsModule.forRoot` vs `forFeature`?**  
   Root = global effects, Feature = module-specific effects.  

24. **What is `StoreDevtoolsModule`?**  
   Enables Redux DevTools for debugging.  

25. **How do you enable time-travel debugging in NgRx?**  
   Use Store DevTools extension.  

---

## 🔹 Best Practices
26. **Why keep reducers pure?**  
   Predictability, testability, no side effects.  

27. **How do you avoid state mutation in NgRx?**  
   Use spread operator or immutable update patterns.  

28. **What is the difference between smart and dumb components?**  
   Smart = connected to store, Dumb = presentational only.  

29. **Why use feature modules with NgRx?**  
   Scalability, modularity, separation of concerns.  

30. **How do you organize actions in NgRx?**  
   Group by feature, use `createAction` with descriptive types.  

---

## 🔹 Advanced Concepts
31. **What is meta-reducer in NgRx?**  
   Higher-order reducer wrapping other reducers (e.g., logging, persistence).  

32. **Example use case of meta-reducer?**  
   Persist state to localStorage.  

33. **What is state hydration?**  
   Restoring state from storage or server.  

34. **What is lazy loading with NgRx?**  
   Load feature store only when module is loaded.  

35. **What is the difference between optimistic and pessimistic updates?**  
   - Optimistic: update UI before API response.  
   - Pessimistic: wait for API response before updating.  

---

## 🔹 Testing & Debugging
36. **How do you test reducers?**  
   Pass state + action, assert new state.  

37. **How do you test selectors?**  
   Provide mock state, assert derived values.  

38. **How do you test effects?**  
   Use `provideMockActions` and `TestScheduler`.  

39. **What is `MockStore` in NgRx testing?**  
   Provides fake store for unit tests.  

40. **How do you debug NgRx state?**  
   Use Store DevTools, logging meta-reducers.  

---

## 🔹 Integration & Real-World
41. **How does NgRx integrate with Angular services?**  
   Effects call services for API requests.  

42. **How do you unsubscribe from store in Angular?**  
   Use `async` pipe or `takeUntil`.  

43. **What is the difference between `dispatch` and `select`?**  
   - Dispatch: send actions.  
   - Select: read state.  

44. **How do you persist NgRx state across refresh?**  
   Use meta-reducer with localStorage/sessionStorage.  

45. **How do you handle authentication state in NgRx?**  
   Store tokens, user info, and use effects for login/logout.  

---

## 🔹 Advanced Patterns
46. **What is NgRx ComponentStore?**  
   Lightweight store for local component state.  

47. **Difference between NgRx Store and ComponentStore?**  
   Store = global, ComponentStore = local.  

48. **What is NgRx Data?**  
   Simplifies CRUD operations with services and entity management.  

49. **What is the difference between NgRx and Akita?**  
   Both are state management libraries; NgRx is Redux-inspired, Akita is simpler.  

50. **When should you NOT use NgRx?**  
   For small apps with simple state, where services suffice.  

---
=================================
Here’s a **comprehensive set of 50 Angular Testing interview questions with answers**, organized by category so you can prepare thoroughly.  

---

## 🔹 Basics of Angular Testing
1. **What is Angular Testing?**  
   Process of verifying Angular components, services, and modules using frameworks like Jasmine and Karma.  

2. **What is Jasmine?**  
   A behavior-driven testing framework for JavaScript, used in Angular.  

3. **What is Karma?**  
   A test runner that executes Jasmine tests in browsers.  

4. **What is TestBed in Angular?**  
   Utility for configuring and initializing Angular environment for unit tests.  

5. **Difference between unit testing and integration testing in Angular?**  
   - Unit: tests individual components/services.  
   - Integration: tests how components interact together.  

---

## 🔹 Component Testing
6. **How do you test Angular components?**  
   Use `TestBed` to configure module, create component fixture, and assert DOM changes.  

7. **What is a fixture in Angular testing?**  
   Wrapper around component instance and template for testing.  

8. **How do you test component lifecycle hooks?**  
   Trigger change detection using `fixture.detectChanges()`.  

9. **How do you test input properties in components?**  
   Set values via `component.inputName = value;` and call `detectChanges()`.  

10. **How do you test output events in components?**  
   Subscribe to `EventEmitter` and assert emitted values.  

---

## 🔹 Service Testing
11. **How do you test Angular services?**  
   Inject service via `TestBed.inject()` and mock dependencies.  

12. **What is HttpClientTestingModule?**  
   Provides `HttpTestingController` to mock HTTP requests.  

13. **How do you test API calls in Angular services?**  
   Use `httpMock.expectOne()` to intercept requests and provide mock responses.  

14. **Difference between spyOn and createSpy?**  
   - spyOn: spies on existing methods.  
   - createSpy: creates standalone spy functions.  

15. **How do you test observables in services?**  
   Subscribe and assert emitted values, or use marble testing.  

---

## 🔹 Directive & Pipe Testing
16. **How do you test Angular directives?**  
   Apply directive to test host component and assert behavior.  

17. **How do you test Angular pipes?**  
   Instantiate pipe class and call `transform()` method.  

18. **What is a pure vs impure pipe in testing?**  
   - Pure: deterministic, easy to test.  
   - Impure: depends on external state, harder to test.  

19. **How do you test structural directives like *ngIf?**  
   Use `fixture.detectChanges()` and check DOM presence/absence.  

20. **How do you test custom pipes with parameters?**  
   Pass arguments to `transform()` and assert output.  

---

## 🔹 Async Testing
21. **What is fakeAsync in Angular testing?**  
   Utility to test async code synchronously using `tick()`.  

22. **What is async() utility in Angular testing?**  
   Wraps test functions to handle async operations.  

23. **Difference between fakeAsync and async?**  
   - fakeAsync: synchronous simulation.  
   - async: waits for async tasks to complete.  

24. **How do you test Observables with delay?**  
   Use `fakeAsync` + `tick()` to simulate passage of time.  

25. **How do you test Promises in Angular?**  
   Use `async` or `fakeAsync` with `flushMicrotasks()`.  

---

## 🔹 NgRx & Store Testing
26. **How do you test NgRx reducers?**  
   Pass state + action, assert new state.  

27. **How do you test NgRx selectors?**  
   Provide mock state, assert derived values.  

28. **How do you test NgRx effects?**  
   Use `provideMockActions` and `TestScheduler`.  

29. **What is MockStore in NgRx testing?**  
   Provides fake store for unit tests.  

30. **How do you test NgRx entity adapter?**  
   Call adapter methods and assert updated state.  

---

## 🔹 Integration & E2E Testing
31. **What is Protractor in Angular testing?**  
   End-to-end testing framework for Angular apps (deprecated in Angular 15+).  

32. **What is Cypress in Angular testing?**  
   Modern E2E testing tool, faster and more reliable than Protractor.  

33. **Difference between unit tests and E2E tests?**  
   Unit = isolated, E2E = full app flow.  

34. **How do you test routing in Angular?**  
   Use `RouterTestingModule` with mock routes.  

35. **How do you test guards in Angular?**  
   Call guard methods with mock `ActivatedRouteSnapshot` and `RouterStateSnapshot`.  

---

## 🔹 Mocking & Dependency Injection
36. **What is dependency injection in Angular testing?**  
   Providing mock services/components via `TestBed`.  

37. **How do you mock services in Angular tests?**  
   Use `useClass`, `useValue`, or `useFactory` in providers.  

38. **Difference between stub and mock?**  
   - Stub: simple fake implementation.  
   - Mock: fake with behavior verification.  

39. **How do you mock ActivatedRoute in Angular tests?**  
   Provide custom `ActivatedRoute` with `params` or `queryParams`.  

40. **How do you mock Router in Angular tests?**  
   Use `RouterTestingModule` or spy on `navigate()` method.  

---

## 🔹 Best Practices & Advanced
41. **Why should tests be deterministic?**  
   To ensure consistent results across runs.  

42. **How do you achieve high test coverage in Angular?**  
   Test components, services, directives, pipes, and edge cases.  

43. **What is code coverage in Angular testing?**  
   Percentage of code executed by tests, generated with `ng test --code-coverage`.  

44. **How do you test Angular forms?**  
   Set values in `FormControl`/`FormGroup` and assert validation.  

45. **How do you test async validators in Angular forms?**  
   Use `fakeAsync` + `tick()` to simulate async validation.  

46. **How do you test change detection strategy OnPush?**  
   Trigger `fixture.detectChanges()` and assert DOM updates.  

47. **How do you test Angular interceptors?**  
   Provide interceptor in `TestBed` and assert modified requests/responses.  

48. **How do you test Angular resolvers?**  
   Call resolver with mock route and assert returned data.  

49. **How do you test Angular animations?**  
   Use `NoopAnimationsModule` to disable animations for predictable tests.  

50. **What are common pitfalls in Angular testing?**  
   Forgetting `detectChanges()`, not unsubscribing, improper async handling.  

---
=================================
Here’s a **comprehensive set of 50 Angular interview questions with answers**, organized by category so you can cover the full spectrum — from fundamentals to advanced topics.  

---

## 🔹 Angular Basics
1. **What is Angular?**  
   A TypeScript-based framework for building single-page applications.  

2. **Difference between AngularJS and Angular?**  
   AngularJS = JavaScript, MVC; Angular = TypeScript, component-based, faster.  

3. **What are Angular components?**  
   Building blocks of UI, combining template, logic, and styles.  

4. **What is a module in Angular?**  
   Container for components, directives, pipes, and services.  

5. **What is a template in Angular?**  
   HTML view with Angular bindings and directives.  

---

## 🔹 Data Binding & Directives
6. **What are the types of data binding in Angular?**  
   - Interpolation `{{}}`  
   - Property binding `[property]`  
   - Event binding `(event)`  
   - Two-way binding `[(ngModel)]`  

7. **Difference between structural and attribute directives?**  
   - Structural (`*ngIf`, `*ngFor`) change DOM structure.  
   - Attribute (`[ngClass]`, `[ngStyle]`) change appearance/behavior.  

8. **What is `ngIf` vs `hidden`?**  
   - `ngIf`: removes element from DOM.  
   - `hidden`: hides element but keeps in DOM.  

9. **What is `ngFor` used for?**  
   Iterates over collections to render lists.  

10. **What is `ngSwitch`?**  
   Conditional rendering based on matching cases.  

---

## 🔹 Components & Lifecycle
11. **What are Angular lifecycle hooks?**  
   Methods like `ngOnInit`, `ngOnChanges`, `ngOnDestroy`.  

12. **Difference between `ngOnInit` and constructor?**  
   Constructor initializes class, `ngOnInit` runs after inputs are set.  

13. **What is `ngOnChanges` used for?**  
   Detects changes in input properties.  

14. **What is `ngOnDestroy` used for?**  
   Cleanup tasks like unsubscribing Observables.  

15. **What is Change Detection in Angular?**  
   Mechanism to update view when data changes.  

---

## 🔹 Services & Dependency Injection
16. **What are Angular services?**  
   Classes for business logic, reusable across components.  

17. **What is Dependency Injection (DI)?**  
   Design pattern where dependencies are provided instead of created.  

18. **Difference between `providedIn: root` and module providers?**  
   Root = singleton across app, module providers = scoped.  

19. **What is hierarchical injector in Angular?**  
   DI system where child injectors can override parent services.  

20. **What is `Injectable()` decorator?**  
   Marks class as available for DI.  

---

## 🔹 Routing
21. **What is Angular Router?**  
   Manages navigation between views.  

22. **Difference between `routerLink` and `href`?**  
   `routerLink` uses Angular routing, `href` reloads page.  

23. **What is lazy loading in Angular?**  
   Loading modules only when needed.  

24. **What are route guards?**  
   Services controlling navigation (`CanActivate`, `CanDeactivate`).  

25. **What is `ActivatedRoute`?**  
   Provides route parameters and data.  

---

## 🔹 Forms
26. **Difference between template-driven and reactive forms?**  
   - Template-driven: simple, uses directives.  
   - Reactive: more control, uses FormGroup/FormControl.  

27. **What is FormControl?**  
   Tracks value and validation of input.  

28. **What is FormGroup?**  
   Collection of FormControls.  

29. **What is FormBuilder?**  
   Utility to create forms quickly.  

30. **How do you add custom validators?**  
   Create function returning validation errors.  

---

## 🔹 Pipes
31. **What are Angular pipes?**  
   Transform data in templates (e.g., `date`, `currency`).  

32. **Difference between pure and impure pipes?**  
   Pure = deterministic, Impure = recalculates often.  

33. **How do you create a custom pipe?**  
   Use `@Pipe` decorator and implement `transform()`.  

34. **What is async pipe?**  
   Subscribes to Observable/Promise and auto-unsubscribes.  

35. **What is chaining pipes?**  
   Applying multiple pipes sequentially.  

---

## 🔹 Performance & Optimization
36. **What is Ahead-of-Time (AOT) compilation?**  
   Compiles templates at build time, faster runtime.  

37. **Difference between JIT and AOT?**  
   JIT compiles at runtime, AOT compiles at build time.  

38. **What is tree-shaking in Angular?**  
   Removes unused code during build.  

39. **What is ChangeDetectionStrategy.OnPush?**  
   Updates view only when inputs change, improves performance.  

40. **What is Angular Universal?**  
   Server-side rendering for SEO and performance.  

---

## 🔹 Testing & Debugging
41. **What is TestBed in Angular testing?**  
   Utility for configuring Angular environment in tests.  

42. **How do you test components in Angular?**  
   Use `TestBed.createComponent()` and `fixture.detectChanges()`.  

43. **What is HttpClientTestingModule?**  
   Provides `HttpTestingController` for mocking HTTP requests.  

44. **What is fakeAsync in Angular testing?**  
   Simulates async code synchronously with `tick()`.  

45. **What is Protractor vs Cypress?**  
   Protractor = Angular E2E (deprecated), Cypress = modern E2E.  

---

## 🔹 Advanced Topics
46. **What is Angular Ivy?**  
   Next-gen rendering engine, smaller bundles, faster compilation.  

47. **What is Angular Zone.js?**  
   Library that tracks async tasks for change detection.  

48. **What is Angular Material?**  
   UI component library following Material Design.  

49. **What is NgRx in Angular?**  
   State management library using RxJS.  

50. **What is Angular CDK?**  
   Component Dev Kit providing utilities like overlays, accessibility.  

---
================================
Got it — you want **scenario-based Angular interview questions with answers**, plus the reasoning behind why interviewers ask them. This is a smart way to prepare, because Angular interviews often test not just theory but how you’d handle real-world situations. Let’s break it down:  

---

## 🔹 Component & Lifecycle Scenarios
**Q1. Scenario:** You have a parent component passing data to a child via `@Input()`. The child doesn’t update when the parent changes.  
- **Answer:** Use `ngOnChanges()` in the child to detect changes, or ensure change detection strategy isn’t set to `OnPush` without immutable updates.  
- **Reason:** Interviewers want to see if you understand **data flow and lifecycle hooks**, critical for debugging UI issues.  

**Q2. Scenario:** A component keeps re-rendering unnecessarily, slowing performance.  
- **Answer:** Use `ChangeDetectionStrategy.OnPush` and immutable data structures.  
- **Reason:** Tests your knowledge of **performance optimization** in Angular.  

---

## 🔹 Services & Dependency Injection
**Q3. Scenario:** You need a singleton service across the app, but also a different instance per feature module.  
- **Answer:** Provide service at root for global singleton, and override in feature module providers for scoped instances.  
- **Reason:** Interviewers check if you understand **hierarchical injectors** and DI scope.  

**Q4. Scenario:** You want to share data between unrelated components.  
- **Answer:** Use a shared service with RxJS `BehaviorSubject` or NgRx store.  
- **Reason:** Tests your ability to handle **state management and communication**.  

---

## 🔹 Routing & Navigation
**Q5. Scenario:** A user tries to access a route without being logged in.  
- **Answer:** Implement `CanActivate` guard to check authentication before navigation.  
- **Reason:** Interviewers want to see if you can enforce **security and access control**.  

**Q6. Scenario:** You need to preload certain modules for faster navigation.  
- **Answer:** Use Angular’s `PreloadAllModules` strategy or custom preloading.  
- **Reason:** Tests your knowledge of **lazy loading and performance tuning**.  

---

## 🔹 Forms & Validation
**Q7. Scenario:** You need a form with complex validation (e.g., password confirmation).  
- **Answer:** Use reactive forms with custom validators. Example: compare password and confirm password fields.  
- **Reason:** Interviewers want to see if you can handle **real-world form logic**.  

**Q8. Scenario:** You need async validation (e.g., check if username already exists).  
- **Answer:** Implement an async validator returning an Observable/Promise.  
- **Reason:** Tests your ability to integrate **backend checks into forms**.  

---

## 🔹 RxJS & Async Handling
**Q9. Scenario:** You have multiple API calls, but you need results only when all are complete.  
- **Answer:** Use RxJS `forkJoin`.  
- **Reason:** Interviewers check if you know **RxJS operators for async orchestration**.  

**Q10. Scenario:** A search box should not call API on every keystroke.  
- **Answer:** Use `debounceTime` and `distinctUntilChanged`.  
- **Reason:** Tests your ability to **optimize API calls with RxJS**.  

---

## 🔹 NgRx & State Management
**Q11. Scenario:** You need to handle API success and failure differently in state.  
- **Answer:** Dispatch `LoadSuccess` and `LoadFailure` actions, handle in reducer/effect.  
- **Reason:** Interviewers want to see if you understand **NgRx patterns for async workflows**.  

**Q12. Scenario:** You want to persist state across page refresh.  
- **Answer:** Use meta-reducers with localStorage.  
- **Reason:** Tests your ability to handle **real-world persistence**.  

---

## 🔹 Testing & Debugging
**Q13. Scenario:** You need to test a component that makes HTTP calls.  
- **Answer:** Use `HttpClientTestingModule` and `HttpTestingController` to mock requests.  
- **Reason:** Interviewers check if you can write **unit tests for services/components**.  

**Q14. Scenario:** You want to test async code in Angular.  
- **Answer:** Use `fakeAsync` and `tick()` or `async` utilities.  
- **Reason:** Tests your ability to handle **async testing scenarios**.  

---

## 🔹 Advanced & Real-World
**Q15. Scenario:** SEO is required for your Angular app.  
- **Answer:** Use Angular Universal for server-side rendering.  
- **Reason:** Interviewers want to see if you know **SSR for SEO and performance**.  

**Q16. Scenario:** You need to support multiple themes dynamically.  
- **Answer:** Use CSS variables or Angular Material theming.  
- **Reason:** Tests your ability to handle **dynamic styling in enterprise apps**.  

---

✨ **Why interviewers ask scenario-based questions:**  
- To check if you can **apply theory in practice**.  
- To see how you **debug and optimize real-world problems**.  
- To evaluate if you understand **Angular’s ecosystem (RxJS, NgRx, DI, testing)**.  
- To test your ability to **think critically under pressure**.  

---

===================================
Perfect, let’s expand with **more scenario-based Angular interview questions, answers, and the reasoning behind why they’re asked**. These are the kinds of practical situations senior-level interviewers love to throw at candidates.  

---

## 🔹 Change Detection & Performance
**Q17. Scenario:** Your Angular app slows down because a large list is re-rendering on every change.  
- **Answer:** Use `trackBy` in `*ngFor` to optimize rendering, and consider `OnPush` change detection.  
- **Reason:** Interviewers want to see if you understand **performance tuning and efficient rendering**.  

**Q18. Scenario:** You need to update only part of the UI when data changes.  
- **Answer:** Use `ChangeDetectorRef.markForCheck()` or `detectChanges()` for fine-grained control.  
- **Reason:** Tests your ability to handle **manual change detection**.  

---

## 🔹 State & Data Flow
**Q19. Scenario:** Two sibling components need to share state without a parent.  
- **Answer:** Use a shared service with RxJS `Subject` or NgRx store.  
- **Reason:** Checks if you know **state sharing patterns** beyond parent-child.  

**Q20. Scenario:** You need to persist user preferences across sessions.  
- **Answer:** Store preferences in NgRx + localStorage via meta-reducer.  
- **Reason:** Tests your ability to handle **real-world persistence**.  

---

## 🔹 Routing & Guards
**Q21. Scenario:** You want to prevent users from leaving a form with unsaved changes.  
- **Answer:** Implement `CanDeactivate` guard to prompt confirmation.  
- **Reason:** Interviewers check if you can enforce **UX safeguards**.  

**Q22. Scenario:** You need role-based access control for routes.  
- **Answer:** Use `CanActivate` guard with role checks from auth service.  
- **Reason:** Tests your ability to implement **authorization logic**.  

---

## 🔹 Forms & Validation
**Q23. Scenario:** You need a dynamic form where fields depend on user input.  
- **Answer:** Use reactive forms with `FormArray` and dynamically add/remove controls.  
- **Reason:** Checks if you can handle **complex, dynamic forms**.  

**Q24. Scenario:** You need to validate a field against server-side data.  
- **Answer:** Implement async validator calling API, returning Observable.  
- **Reason:** Tests your ability to integrate **backend validation**.  

---

## 🔹 RxJS & Async
**Q25. Scenario:** You need to cancel ongoing API requests when a new search query is entered.  
- **Answer:** Use `switchMap` to cancel previous Observable.  
- **Reason:** Interviewers want to see if you understand **RxJS cancellation patterns**.  

**Q26. Scenario:** You need to retry failed API calls with exponential backoff.  
- **Answer:** Use `retryWhen` with delay logic.  
- **Reason:** Tests your ability to handle **resilient async workflows**.  

---

## 🔹 Testing & Debugging
**Q27. Scenario:** You want to test a component that uses `@Input()` and emits `@Output()`.  
- **Answer:** Set input values in test, subscribe to output, and assert emitted values.  
- **Reason:** Checks if you can write **realistic component tests**.  

**Q28. Scenario:** You need to test a service making HTTP calls.  
- **Answer:** Use `HttpClientTestingModule` and `HttpTestingController`.  
- **Reason:** Tests your ability to mock **API calls in unit tests**.  

---

## 🔹 Advanced & Enterprise
**Q29. Scenario:** Your Angular app must support multiple languages.  
- **Answer:** Use Angular i18n or ngx-translate for internationalization.  
- **Reason:** Interviewers want to see if you can handle **globalization requirements**.  

**Q30. Scenario:** You need to implement dark mode toggle.  
- **Answer:** Use CSS variables or Angular Material theming with dynamic switching.  
- **Reason:** Tests your ability to handle **dynamic theming**.  

**Q31. Scenario:** You need SEO optimization for a blog built in Angular.  
- **Answer:** Use Angular Universal for server-side rendering.  
- **Reason:** Checks if you know **SSR for SEO and performance**.  

**Q32. Scenario:** You need to integrate WebSocket live updates.  
- **Answer:** Use RxJS `webSocket` or wrap WebSocket in a service.  
- **Reason:** Tests your ability to handle **real-time data streams**.  

---

✨ **Why interviewers ask these scenarios:**  
- To see if you can **apply Angular concepts in real-world problems**.  
- To test your **debugging, optimization, and architectural thinking**.  
- To evaluate your ability to **balance performance, UX, and maintainability**.  

---

Alright Deepak, let’s build out a **full set of 50 scenario-based Angular interview questions with answers and the reasoning behind why they’re asked**. These are practical, real-world situations that interviewers use to test whether you can apply Angular concepts beyond theory.  

---

## 🔹 Component & Lifecycle (1–10)
1. **Parent → Child data not updating**  
   - **Answer:** Use `ngOnChanges()` or immutable updates with `OnPush`.  
   - **Reason:** Tests lifecycle awareness.  

2. **Component re-renders too often**  
   - **Answer:** Use `ChangeDetectionStrategy.OnPush`.  
   - **Reason:** Checks performance optimization.  

3. **Need to run code after view init**  
   - **Answer:** Use `ngAfterViewInit`.  
   - **Reason:** Tests lifecycle hook knowledge.  

4. **Cleanup before component destroy**  
   - **Answer:** Use `ngOnDestroy` to unsubscribe Observables.  
   - **Reason:** Tests memory leak prevention.  

5. **Dynamic component creation**  
   - **Answer:** Use `ViewContainerRef.createComponent()`.  
   - **Reason:** Tests advanced component handling.  

6. **Child component needs to notify parent**  
   - **Answer:** Use `@Output()` with EventEmitter.  
   - **Reason:** Checks event binding understanding.  

7. **Component needs to access DOM element**  
   - **Answer:** Use `@ViewChild`.  
   - **Reason:** Tests DOM interaction.  

8. **Component should only render once**  
   - **Answer:** Use `ngOnInit` for initialization logic.  
   - **Reason:** Tests lifecycle vs constructor.  

9. **Component should react to input changes**  
   - **Answer:** Use `ngOnChanges`.  
   - **Reason:** Tests input property handling.  

10. **Component should run code after content projection**  
   - **Answer:** Use `ngAfterContentInit`.  
   - **Reason:** Tests advanced lifecycle hooks.  

---

## 🔹 Services & Dependency Injection (11–20)
11. **Singleton service across app**  
   - **Answer:** Provide service in root.  
   - **Reason:** Tests DI scope.  

12. **Different service instance per module**  
   - **Answer:** Provide service in feature module.  
   - **Reason:** Tests hierarchical injectors.  

13. **Share data between unrelated components**  
   - **Answer:** Use shared service with RxJS Subject.  
   - **Reason:** Tests communication patterns.  

14. **Lazy-loaded module needs its own service instance**  
   - **Answer:** Provide service in that module.  
   - **Reason:** Tests DI scoping.  

15. **Service depends on another service**  
   - **Answer:** Use constructor injection.  
   - **Reason:** Tests DI chaining.  

16. **Mock service in unit tests**  
   - **Answer:** Use `useClass` or `useValue` in providers.  
   - **Reason:** Tests testing skills.  

17. **Service should be tree-shakable**  
   - **Answer:** Use `providedIn: 'root'`.  
   - **Reason:** Tests optimization knowledge.  

18. **Service should be available only in one component**  
   - **Answer:** Provide service in component’s providers array.  
   - **Reason:** Tests DI scoping.  

19. **Service should persist data across refresh**  
   - **Answer:** Use localStorage or NgRx meta-reducer.  
   - **Reason:** Tests persistence handling.  

20. **Service should handle API calls**  
   - **Answer:** Use HttpClient in service.  
   - **Reason:** Tests separation of concerns.  

---

## 🔹 Routing & Navigation (21–30)
21. **Prevent navigation if not logged in**  
   - **Answer:** Use `CanActivate` guard.  
   - **Reason:** Tests security.  

22. **Prevent leaving form with unsaved changes**  
   - **Answer:** Use `CanDeactivate` guard.  
   - **Reason:** Tests UX safeguards.  

23. **Preload modules for faster navigation**  
   - **Answer:** Use `PreloadAllModules`.  
   - **Reason:** Tests performance.  

24. **Role-based route access**  
   - **Answer:** Implement guard checking roles.  
   - **Reason:** Tests authorization.  

25. **Pass data via route**  
   - **Answer:** Use `data` property in route config.  
   - **Reason:** Tests routing features.  

26. **Get route parameters**  
   - **Answer:** Use `ActivatedRoute.params`.  
   - **Reason:** Tests parameter handling.  

27. **Redirect after login**  
   - **Answer:** Use `Router.navigate()`.  
   - **Reason:** Tests navigation control.  

28. **Lazy load feature module**  
   - **Answer:** Use `loadChildren`.  
   - **Reason:** Tests modularity.  

29. **Dynamic route configuration**  
   - **Answer:** Use `Router.resetConfig()`.  
   - **Reason:** Tests advanced routing.  

30. **Handle 404 page**  
   - **Answer:** Add wildcard route `**`.  
   - **Reason:** Tests error handling.  

---

## 🔹 Forms & Validation (31–40)
31. **Simple form validation**  
   - **Answer:** Use template-driven forms with `required`.  
   - **Reason:** Tests basics.  

32. **Complex form validation**  
   - **Answer:** Use reactive forms with custom validators.  
   - **Reason:** Tests advanced forms.  

33. **Async validation**  
   - **Answer:** Use async validator returning Observable.  
   - **Reason:** Tests backend integration.  

34. **Dynamic form fields**  
   - **Answer:** Use `FormArray`.  
   - **Reason:** Tests dynamic forms.  

35. **Cross-field validation**  
   - **Answer:** Compare values in custom validator.  
   - **Reason:** Tests complex logic.  

36. **Form should auto-save**  
   - **Answer:** Subscribe to valueChanges.  
   - **Reason:** Tests reactive patterns.  

37. **Form should reset after submit**  
   - **Answer:** Use `form.reset()`.  
   - **Reason:** Tests form lifecycle.  

38. **Form should disable submit until valid**  
   - **Answer:** Bind button disabled to `form.valid`.  
   - **Reason:** Tests UX.  

39. **Form should show error messages**  
   - **Answer:** Use `form.controls.field.errors`.  
   - **Reason:** Tests validation handling.  

40. **Form should support nested groups**  
   - **Answer:** Use `FormGroup` inside another `FormGroup`.  
   - **Reason:** Tests complex forms.  

---

## 🔹 RxJS, NgRx & Async (41–50)
41. **Cancel previous API request on new search**  
   - **Answer:** Use `switchMap`.  
   - **Reason:** Tests RxJS cancellation.  

42. **Run multiple API calls concurrently**  
   - **Answer:** Use `forkJoin`.  
   - **Reason:** Tests async orchestration.  

43. **Retry failed API calls**  
   - **Answer:** Use `retryWhen`.  
   - **Reason:** Tests resilience.  

44. **Handle API success/failure in state**  
   - **Answer:** Dispatch success/failure actions in NgRx.  
   - **Reason:** Tests state management.  

45. **Persist state across refresh**  
   - **Answer:** Use meta-reducer with localStorage.  
   - **Reason:** Tests persistence.  

46. **Prevent memory leaks in Observables**  
   - **Answer:** Use `takeUntil` or async pipe.  
   - **Reason:** Tests cleanup.  

47. **Throttle API calls**  
   - **Answer:** Use `debounceTime`.  
   - **Reason:** Tests optimization.  

48. **Handle optimistic updates**  
   - **Answer:** Update UI before API response, rollback on error.  
   - **Reason:** Tests UX patterns.  

49. **Handle pessimistic updates**  
   - **Answer:** Wait for API response before updating UI.  
   - **Reason:** Tests reliability.  

50. **Debug state changes**  
   - **Answer:** Use Store DevTools.  
   - **Reason:** Tests debugging skills.  

---






