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
