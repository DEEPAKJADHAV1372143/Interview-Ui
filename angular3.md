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
