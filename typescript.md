### TypeScript Interview Questions and Answers (50+)

Below is a practical, interview-ready collection of **55 TypeScript questions with concise answers and examples**. Use this to review fundamentals, advanced topics, and common coding patterns interviewers expect.

---

## Basics (1–12)

1. **What is TypeScript?**  
   **Answer:** TypeScript is a statically typed superset of JavaScript that adds optional types, interfaces, enums, and compile-time checks. It compiles to plain JavaScript and helps catch errors early while improving IDE tooling and refactoring.

2. **How do you compile TypeScript to JavaScript?**  
   **Answer:** Use the TypeScript compiler: `tsc file.ts`. For projects, run `tsc --project tsconfig.json`. Tooling like `ts-node`, `webpack`, `esbuild`, or `ts-jest` integrate compilation into workflows.

3. **What is `tsconfig.json`?**  
   **Answer:** A configuration file for the TypeScript compiler that sets options (target, module, strict, paths, outDir, etc.) and controls which files are included/excluded.

4. **What does `--strict` do?**  
   **Answer:** Enables a set of strict type-checking options (`strictNullChecks`, `noImplicitAny`, `strictFunctionTypes`, etc.) that make type checking more rigorous and safer.

5. **What is the difference between `any` and `unknown`?**  
   **Answer:** `any` disables type checking (opt-out). `unknown` is safer: you must narrow it (type guard or assertion) before using it. `unknown` forces explicit handling.

6. **What is type inference?**  
   **Answer:** TypeScript automatically infers types from values and context (e.g., `const x = 5` infers `number`). Inference reduces the need for explicit annotations.

7. **How do you declare a variable with a specific type?**  
   **Answer:**  
   ```ts
   let name: string = "Deepak";
   const count: number = 10;
   ```

8. **What are union and intersection types?**  
   **Answer:**  
   - **Union (`A | B`)**: value can be A or B.  
   - **Intersection (`A & B`)**: value must satisfy both A and B.

   ```ts
   type ID = string | number;
   type PersonWithAddress = Person & { address: string };
   ```

9. **What is type alias vs interface?**  
   **Answer:** Both define shapes. `interface` supports declaration merging and is preferred for object shapes; `type` is more flexible (unions, primitives, mapped types). Many use them interchangeably for object types.

10. **What are literal types?**  
    **Answer:** Types that are exact values, e.g., `'left' | 'right'` or `42`. Useful for constrained values and discriminated unions.

11. **What is `never` type?**  
    **Answer:** Represents values that never occur (e.g., a function that always throws or an exhaustive switch that should be unreachable). Useful for exhaustive checks.

12. **What is `void` vs `undefined`?**  
    **Answer:** `void` is used for functions that don’t return a value. `undefined` is a value. A function typed `(): void` may return `undefined` implicitly.

---

## Types & Advanced Type Features (13–26)

13. **What are generics and why use them?**  
    **Answer:** Generics allow writing reusable, type-safe components/functions that work with multiple types. They preserve type information across operations.

    ```ts
    function identity<T>(arg: T): T { return arg; }
    const s = identity<string>("hello");
    ```

14. **What are mapped types?**  
    **Answer:** Types that transform properties of another type (e.g., `Partial<T>`, `Readonly<T>`). Example:

    ```ts
    type Readonly<T> = { readonly [K in keyof T]: T[K] };
    ```

15. **What is `keyof` operator?**  
    **Answer:** Produces a union of property names of a type. Example: `keyof Person` might be `'name' | 'age'`.

16. **What is `typeof` in types?**  
    **Answer:** In type position, `typeof` extracts the type of a value or variable. Example: `type T = typeof someVar`.

17. **What are conditional types?**  
    **Answer:** Types that select one type or another based on a condition: `T extends U ? X : Y`. Useful for type-level logic.

18. **What is `infer` in conditional types?**  
    **Answer:** `infer` extracts a type variable inside a conditional type. Example:

    ```ts
    type ReturnType<T> = T extends (...args: any[]) => infer R ? R : any;
    ```

19. **What are utility types?**  
    **Answer:** Built-in helpers like `Partial<T>`, `Required<T>`, `Pick<T, K>`, `Omit<T, K>`, `Record<K, T>`, `Exclude`, `Extract`, `NonNullable`, `ReturnType<T>`, `InstanceType<T>`.

20. **What is `Record` type?**  
    **Answer:** Creates an object type with keys K and values T: `Record<string, number>` is `{ [key: string]: number }`.

21. **How do you create discriminated unions?**  
    **Answer:** Use a common literal property (tag) to discriminate variants:

    ```ts
    type Shape =
      | { kind: 'circle'; radius: number }
      | { kind: 'square'; size: number };

    function area(s: Shape) {
      if (s.kind === 'circle') return Math.PI * s.radius ** 2;
      return s.size * s.size;
    }
    ```

22. **What is type narrowing and how is it done?**  
    **Answer:** Narrowing reduces a broad type to a more specific one using `typeof`, `instanceof`, property checks, user-defined type guards, or control flow analysis.

23. **What are type guards and how to write one?**  
    **Answer:** Functions that assert a type using a `param is Type` return signature.

    ```ts
    function isString(x: any): x is string { return typeof x === 'string'; }
    ```

24. **What are index signatures?**  
    **Answer:** Define types for dynamic property names: `{ [key: string]: number }`. Useful for dictionaries.

25. **What is `unknown[]` vs `any[]`?**  
    **Answer:** `unknown[]` forces you to narrow elements before use; `any[]` allows any operations without checks.

26. **How to model optional properties?**  
    **Answer:** Use `?` on property: `name?: string`. Optional properties may be `undefined`.

---

## Functions, Classes & OOP (27–36)

27. **How do you type function overloads?**  
    **Answer:** Provide multiple function signatures followed by a single implementation.

    ```ts
    function combine(a: string, b: string): string;
    function combine(a: number, b: number): number;
    function combine(a: any, b: any) { return a + b; }
    ```

28. **What is `this` typing in TypeScript?**  
    **Answer:** You can annotate `this` in function signatures: `function f(this: HTMLElement) { ... }`. In classes, `this` is typed to the instance.

29. **How do you declare a class and implement an interface?**  
    **Answer:**
    ```ts
    interface Person { name: string; greet(): void; }
    class User implements Person {
      constructor(public name: string) {}
      greet() { console.log(`Hi ${this.name}`); }
    }
    ```

30. **What are access modifiers?**  
    **Answer:** `public` (default), `private`, `protected`, and `readonly`. They control visibility and mutability.

31. **What are abstract classes?**  
    **Answer:** Classes that cannot be instantiated and can contain abstract methods that subclasses must implement.

    ```ts
    abstract class Animal { abstract speak(): void; }
    class Dog extends Animal { speak() { console.log('woof'); } }
    ```

32. **What is structural typing?**  
    **Answer:** Type compatibility is based on shape (members), not nominal identity. Two types with the same shape are compatible.

33. **How to type constructors and `new` signatures?**  
    **Answer:** Use `new (...args: any[]) => T` to type constructor signatures, useful for factories.

34. **What are mixins and how to implement them?**  
    **Answer:** Mixins are functions that extend classes. Example pattern uses `class extends Base { ... }` inside a factory function.

---

## Generics & Advanced Patterns (37–44)

35. **How to constrain generics?**  
    **Answer:** Use `extends` to constrain: `function f<T extends { id: string }>(x: T) { ... }`.

36. **What is generic default type?**  
    **Answer:** Provide default: `function f<T = string>(x: T) { ... }`.

37. **How to write a generic React component in TypeScript?**  
    **Answer:**  
    ```tsx
    type Props<T> = { items: T[]; render: (item: T) => JSX.Element };
    function List<T>({ items, render }: Props<T>) { return <>{items.map(render)}</>; }
    ```

38. **What are conditional mapped types?**  
    **Answer:** Combine mapped and conditional types to transform properties based on conditions (advanced type-level programming).

39. **How to type a fluent API?**  
    **Answer:** Return `this` or a generic `this` type to preserve chaining. Use `this: this` in methods for correct typing in subclasses.

40. **What is variance (covariance/contravariance) in TypeScript?**  
    **Answer:** Variance describes how subtyping of complex types relates to subtyping of their components. TypeScript uses structural typing and has specific rules for function parameter bivariance in some contexts; `strictFunctionTypes` enforces contravariance for parameters.

41. **How to create a type-safe event emitter?**  
    **Answer:** Use generics and mapped types:

    ```ts
    type Events = { click: MouseEvent; change: string };
    class Emitter<E extends Record<string, any>> {
      on<K extends keyof E>(k: K, cb: (v: E[K]) => void) { ... }
    }
    ```

42. **What are template literal types?**  
    **Answer:** Build string literal unions using template syntax: `type T = \`on${Capitalize<'click' | 'hover'>}\`` — useful for generating event names or keys.

43. **How to type deeply nested objects safely?**  
    **Answer:** Use utility types, `Partial`, `Required`, and mapped types, or create helper functions that accept typed paths and return typed values.

44. **What are branded types and how to implement them?**  
    **Answer:** Create nominal-like types by intersecting with a unique symbol:

    ```ts
    type Brand<K, T> = K & { __brand: T };
    type UserId = Brand<string, 'UserId'>;
    ```

---

## Tooling, Ecosystem & Runtime (45–55)

45. **How does TypeScript interoperate with JavaScript libraries?**  
    **Answer:** Use type definitions (`.d.ts`) from DefinitelyTyped (`@types/*`) or write your own declaration files. Use `declare module` for simple cases.

46. **What is declaration file (`.d.ts`)?**  
    **Answer:** A file that describes the types of a module without implementation. Used to provide typings for JS libraries or to expose types from TS libraries.

47. **How to publish a TypeScript library?**  
    **Answer:** Compile to JS, include `.d.ts` files (via `declaration: true`), set `types` in `package.json`, and publish to npm. Provide ESModule and CommonJS builds if needed.

48. **What is `ts-node`?**  
    **Answer:** A tool to run TypeScript directly in Node.js for development by transpiling on the fly.

49. **How to configure ESLint for TypeScript?**  
    **Answer:** Use `@typescript-eslint/parser` and `@typescript-eslint/eslint-plugin` with recommended rules. Replace TSLint (deprecated) with ESLint + TypeScript plugin.

50. **How to debug TypeScript in the browser?**  
    **Answer:** Generate source maps (`"sourceMap": true` in `tsconfig.json`) so the browser maps compiled JS back to TS files for breakpoints and stack traces.

51. **What is `isolatedModules` and when to enable it?**  
    **Answer:** Ensures each file can be transpiled independently (required by Babel/ts-loader in transpile-only mode). It disallows certain type-only constructs that require whole-program analysis.

52. **How to handle third-party types that are missing or incorrect?**  
    **Answer:** Create a local `.d.ts` with `declare module 'lib' { ... }`, contribute fixes to DefinitelyTyped, or use `as unknown as` casts carefully.

53. **What are `type` vs `interface` trade-offs in public APIs?**  
    **Answer:** `interface` supports declaration merging and is often preferred for public object shapes; `type` is more flexible (unions, tuples). For library authors, `interface` can be extended by consumers.

54. **How to migrate a JS project to TypeScript incrementally?**  
    **Answer:** Enable `allowJs` and `checkJs` in `tsconfig`, rename files gradually to `.ts/.tsx`, add `noImplicitAny` and `strict` progressively, and add declaration files for external modules.

55. **What runtime checks should you still do even with TypeScript?**  
    **Answer:** Validate external input (network, user input), ensure runtime invariants, and guard against mismatches between compile-time types and runtime data (e.g., JSON from APIs). TypeScript is compile-time only.

---

## Practical Coding Questions (short exercises with answers)

56. **Write a typed function to merge two objects preserving types.**  
```ts
function merge<A, B>(a: A, b: B): A & B {
  return { ...(a as any), ...(b as any) };
}
const merged = merge({ name: 'D' }, { age: 30 }); // type: { name: string } & { age: number }
```

57. **Type-safe `pluck` function that extracts property values.**  
```ts
function pluck<T, K extends keyof T>(obj: T, key: K): T[K] {
  return obj[key];
}
const name = pluck({ name: 'D', age: 30 }, 'name'); // string
```

58. **Create a typed `mapValues` utility.**  
```ts
function mapValues<T, U>(obj: T, fn: (v: T[keyof T]) => U): { [K in keyof T]: U } {
  const res: any = {};
  for (const k in obj) res[k] = fn((obj as any)[k]);
  return res;
}
```

59. **Type-safe event emitter example.**  
```ts
type Events = { data: string; error: Error };
class Emitter<E extends Record<string, any>> {
  private handlers: { [K in keyof E]?: ((v: E[K]) => void)[] } = {};
  on<K extends keyof E>(k: K, cb: (v: E[K]) => void) {
    (this.handlers[k] ||= []).push(cb);
  }
  emit<K extends keyof E>(k: K, v: E[K]) {
    (this.handlers[k] || []).forEach(h => h(v));
  }
}
```

60. **Write a typed `Promise` retry helper.**  
```ts
async function retry<T>(fn: () => Promise<T>, attempts = 3): Promise<T> {
  let lastErr: any;
  for (let i = 0; i < attempts; i++) {
    try { return await fn(); } catch (e) { lastErr = e; }
  }
  throw lastErr;
}
```

---

## Interview Tips and Common Pitfalls

- **Prefer `strict` mode** in real projects; it prevents many runtime bugs.  
- **Avoid `any`** except as a last resort; prefer `unknown` and explicit narrowing.  
- **Use utility types** to reduce boilerplate and express intent.  
- **Write small, well-typed functions**; they’re easier to test and reason about.  
- **Remember TypeScript is erased at runtime** — runtime validation is still necessary for external data.  
- **Be careful with type assertions (`as`)** — they bypass the compiler and can hide bugs.

---


- **Expand any of the 55 items** into a deeper explanation with more examples and edge cases.  
- **Generate 30+ TypeScript coding exercises** with full solutions and tests.  
- **Create a printable one-page cheat sheet** of TypeScript utility types and common patterns.  

