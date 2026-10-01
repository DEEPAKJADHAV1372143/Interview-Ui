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
