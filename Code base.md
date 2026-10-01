

## 🔹 Code-Level JavaScript Interview Q&A

### 1. Reverse a String
**Question:** Write a function to reverse a string without using built-in `reverse()`.

```javascript
function reverseString(str) {
  let reversed = "";
  for (let i = str.length - 1; i >= 0; i--) {
    reversed += str[i];
  }
  return reversed;
}

console.log(reverseString("Deepak")); // "kapeeD"
```

---

### 2. Remove Duplicates from an Array
**Question:** How do you remove duplicates from an array?

```javascript
function removeDuplicates(arr) {
  return [...new Set(arr)];
}

console.log(removeDuplicates([1, 2, 2, 3, 4, 4])); // [1, 2, 3, 4]
```

---

### 3. Check for Palindrome
**Question:** Write a function to check if a string is a palindrome.

```javascript
function isPalindrome(str) {
  const reversed = str.split("").reverse().join("");
  return str === reversed;
}

console.log(isPalindrome("madam")); // true
console.log(isPalindrome("deepak")); // false
```

---

### 4. Flatten a Nested Array
**Question:** Flatten `[1, [2, [3, 4]], 5]` into `[1, 2, 3, 4, 5]`.

```javascript
function flattenArray(arr) {
  return arr.flat(Infinity);
}

console.log(flattenArray([1, [2, [3, 4]], 5])); // [1, 2, 3, 4, 5]
```

---

### 5. Debounce Function
**Question:** Implement a debounce function.

```javascript
function debounce(fn, delay) {
  let timer;
  return function (...args) {
    clearTimeout(timer);
    timer = setTimeout(() => fn.apply(this, args), delay);
  };
}

const logMessage = debounce(() => console.log("Hello!"), 1000);
logMessage(); // Executes after 1s if not called again
```

---

### 6. Deep Clone an Object
**Question:** How do you deep clone an object in JavaScript?

```javascript
function deepClone(obj) {
  return JSON.parse(JSON.stringify(obj));
}

const original = { a: 1, b: { c: 2 } };
const copy = deepClone(original);
copy.b.c = 99;

console.log(original.b.c); // 2 (not affected)
```

---
