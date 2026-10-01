### JavaScript Overview
**JavaScript** is a high-level, dynamic programming language used for web development, server-side apps (Node.js), scripting, and automation. It supports **imperative, functional, and object-oriented** styles, runs in browsers and runtimes, and is standardized as **ECMAScript**. Key features: dynamic typing, first-class functions, prototype-based objects, event-driven and asynchronous programming.

---

### Core Syntax and Data Types
#### Primitive types
- **`undefined`** — absence of value.  
- **`null`** — intentional empty value.  
- **`boolean`** — `true` or `false`.  
- **`number`** — integers and floats (IEEE‑754).  
- **`bigint`** — arbitrary precision integers (e.g., `123n`).  
- **`string`** — text.  
- **`symbol`** — unique identifiers.

#### Structural types
- **`Object`** — key/value map.  
- **`Array`** — ordered list.  
- **`Function`** — callable object.  
- **`Date`, `RegExp`, `Map`, `Set`, `WeakMap`, `WeakSet`, `Promise`** — built‑ins.

#### Literals and basic syntax
```javascript
const s = "hello";           // string
let n = 42;                  // number
let b = true;                // boolean
const obj = { a: 1, b: 2 };  // object
const arr = [1,2,3];         // array
```

#### Operators (selected)
- **Arithmetic**: `+ - * / % **`  
- **Assignment**: `=, +=, -=, *=, /=`  
- **Comparison**: `==, ===, !=, !==, <, >, <=, >=`  
- **Logical**: `&&, ||, !`  
- **Nullish coalescing**: `??`  
- **Optional chaining**: `?.`  
- **Spread / Rest**: `...`  
- **Ternary**: `cond ? a : b`

---

### Functions and Object Oriented Patterns
#### Function forms
```javascript
// Function declaration
function add(a, b) { return a + b; }

// Function expression
const mul = function(a, b) { return a * b; };

// Arrow function
const sub = (a, b) => a - b;
```
- **`this`** behavior differs: arrow functions inherit `this` lexically; regular functions get `this` from call site.
- **Default parameters**, **rest parameters**, and **destructuring** are common.

#### Closures and higher-order functions
- Functions capture surrounding scope — used for **encapsulation**, **factories**, **memoization**.
```javascript
function makeCounter() {
  let count = 0;
  return () => ++count;
}
```

#### Prototypes and classes
- Prototype-based inheritance; ES6 `class` is syntactic sugar.
```javascript
class Person {
  constructor(name) { this.name = name; }
  greet() { return `Hi ${this.name}`; }
}
```

#### Common object patterns
- **Factory functions**, **module pattern**, **mixins**, **composition over inheritance**.

---

### Asynchronous JavaScript
#### Promises
```javascript
fetch(url)
  .then(res => res.json())
  .then(data => console.log(data))
  .catch(err => console.error(err));
```
- **States**: pending, fulfilled, rejected.  
- **Promise.all**, **Promise.race**, **Promise.allSettled**, **Promise.any**.

#### Async Await
```javascript
async function getData() {
  try {
    const res = await fetch(url);
    const json = await res.json();
    return json;
  } catch (err) {
    throw err;
  }
}
```

#### Event loop essentials
- **Call stack**, **microtask queue** (Promises), **task queue** (setTimeout, I/O).  
- Microtasks run before next macrotask; use this to reason about ordering.

---

### DOM, Events, and Browser APIs
#### DOM basics
- **Select**: `document.querySelector`, `getElementById`.  
- **Modify**: `element.textContent`, `element.innerHTML`, `element.classList`.  
- **Create**: `document.createElement`, `appendChild`, `replaceChild`.

#### Events
- `element.addEventListener('click', handler, { once: true, capture: false })`  
- Event object: `event.target`, `event.currentTarget`, `event.preventDefault()`, `event.stopPropagation()`.

#### Useful browser APIs
- **Fetch** for HTTP, **LocalStorage / SessionStorage**, **IndexedDB**, **WebSockets**, **Service Workers**, **Geolocation**, **History / Location**, **Canvas / WebGL**, **Web Audio**.

---

### Modules, Tooling, and Best Practices
#### Modules
- **ES Modules**: `export`, `export default`, `import { x } from './mod.js'`.  
- **CommonJS** (Node): `module.exports`, `require()`.

#### Error handling
- Use `try/catch` for synchronous and `try { await } catch` for async.  
- Prefer throwing `Error` objects: `throw new Error('message')`.

#### Testing and tooling
- Linters: **ESLint**.  
- Formatters: **Prettier**.  
- Bundlers: **Webpack**, **Rollup**, **Vite**.  
- Test frameworks: **Jest**, **Mocha**, **Jasmine**.

#### Performance and security tips
- **Avoid blocking the main thread**; use web workers for heavy CPU tasks.  
- **Debounce/throttle** frequent handlers.  
- **Sanitize** user input before `innerHTML`.  
- Use **CSP** headers and avoid eval-like constructs.  
- Minimize reflows by batching DOM reads/writes.

---

### Quick Reference Snippets
#### Deep clone (simple)
```javascript
const clone = JSON.parse(JSON.stringify(obj)); // limitations: functions, Dates, undefined lost
```
#### Debounce
```javascript
function debounce(fn, ms) {
  let t;
  return (...args) => {
    clearTimeout(t);
    t = setTimeout(() => fn.apply(this, args), ms);
  };
}
```
#### Promise retry
```javascript
async function retry(fn, attempts = 3) {
  let lastErr;
  for (let i = 0; i < attempts; i++) {
    try { return await fn(); } catch (e) { lastErr = e; }
  }
  throw lastErr;
}
```

---

If you want, I can now:
- **Expand any section** into a deeper guide (e.g., full ES6+ features, event loop internals, or Node.js core APIs).  
- **Provide 50+ interview coding problems** in JavaScript with solutions and explanations.  
- **Create a printable cheat sheet** of common methods and patterns.  

Which would you like next?
