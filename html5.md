
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

