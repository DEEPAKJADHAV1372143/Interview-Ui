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
