

## 🔥 50+ JavaScript Code-Level Interview Q&A

### String & Array Manipulation
1. Reverse a string  
2. Check palindrome string  
3. Count vowels in a string  
4. Find longest word in a sentence  
5. Reverse words in a sentence  
6. Remove duplicates from an array  
7. Find intersection of two arrays  
8. Flatten nested arrays  
9. Find missing number in array (1–N)  
10. Find second largest number in array  

### Object & Data Handling
11. Deep clone an object  
12. Compare two objects for equality  
13. Convert object to array of keys/values  
14. Group array of objects by property  
15. Sort array of objects by key  
16. Merge two objects  
17. Remove property from object  
18. Count frequency of elements in array  
19. Find unique values in array of objects  
20. Convert array to object (key-value map)  

### Functions & Closures
21. Implement debounce function  
22. Implement throttle function  
23. Create memoization function  
24. Write a curry function  
25. Implement once() function (runs only once)  
26. Write a function that returns another function (closure)  
27. Implement compose() function  
28. Implement pipe() function  
29. Write factorial using recursion  
30. Fibonacci sequence generator  

### ES6+ Features
31. Use destructuring to swap variables  
32. Use rest/spread operator in function  
33. Implement default parameters  
34. Use template literals for dynamic strings  
35. Create class with constructor & methods  
36. Implement inheritance using `extends`  
37. Static methods in class  
38. Private fields in class (# syntax)  
39. Async/Await example with fetch  
40. Promise.all usage  

### Algorithms & Logic
41. Find prime numbers up to N  
42. Check if number is Armstrong number  
43. Find GCD of two numbers  
44. Find factorial iteratively  
45. Binary search implementation  
46. Linear search implementation  
47. Find duplicates in string  
48. Anagram check between two strings  
49. Find max consecutive 1s in binary array  
50. Rotate array by K steps  

### Advanced / Tricky
51. Implement custom bind()  
52. Implement custom call()  
53. Implement custom apply()  
54. Polyfill for Array.map()  
55. Polyfill for Array.filter()  
56. Polyfill for Array.reduce()  
57. Event delegation example  
58. Implement custom EventEmitter  
59. Write a function to retry API call 3 times  
60. Implement sleep() function using promises  

---

## ✨ Example Snippets (few highlights)

### Custom `bind()` Polyfill
```javascript
Function.prototype.myBind = function(context, ...args) {
  const fn = this;
  return function(...newArgs) {
    return fn.apply(context, [...args, ...newArgs]);
  };
};

function greet(msg) {
  console.log(`${msg}, ${this.name}`);
}

const person = { name: "Deepak" };
const bound = greet.myBind(person, "Hello");
bound(); // "Hello, Deepak"
```

---

### Fibonacci (Recursive)
```javascript
function fibonacci(n) {
  if (n <= 1) return n;
  return fibonacci(n - 1) + fibonacci(n - 2);
}

console.log(fibonacci(6)); // 8
```

---

### Debounce
```javascript
function debounce(fn, delay) {
  let timer;
  return function(...args) {
    clearTimeout(timer);
    timer = setTimeout(() => fn.apply(this, args), delay);
  };
}
```

---
