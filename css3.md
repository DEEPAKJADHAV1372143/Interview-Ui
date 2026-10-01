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
