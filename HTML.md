| **Tag** | **Purpose** | **Common Attributes** | **Self-closing** |
| --- | --- | --- | --- |
| ``<!DOCTYPE ``html>`` | Declares HTML5 document type | — | No |
| ``<html>`` | Root element of an HTML document | **lang** | No |
| ``<head>`` | Metadata container | — | No |
| ``<meta>`` | Metadata (charset, viewport) | **charset; name; content** | Yes |
| ``<title>`` | Document title shown in browser tab | — | No |
| ``<link>`` | Link external resources (CSS, icons) | **rel; href; type** | Yes |
| ``<script>`` | JavaScript inclusion | **src; async; defer; type** | No |
| ``<style>`` | Internal CSS | **type** | No |
| ``<body>`` | Visible page content | **class; id** | No |
| ``<header>`` | Introductory content or nav | **class; id** | No |
| ``<nav>`` | Navigation links | **aria-label; class** | No |
| ``<main>`` | Main page content | **id; class** | No |
| ``<section>`` | Thematic grouping of content | **id; class** | No |
| ``<article>`` | Self-contained composition | **id; class** | No |
| ``<aside>`` | Sidebar or tangential content | **id; class** | No |
| ``<footer>`` | Footer content | **id; class** | No |
| ``<h1>…<h6>`` | Headings, h1 highest level | **id; class** | No |
| ``<p>`` | Paragraph | **class; id** | No |
| ``<a>`` | Hyperlink | **href; target; rel; download** | No |
| ``<img>`` | Image | **src; alt; width; height; loading** | Yes |
| ``<ul>`` | Unordered list | **class; id** | No |
| ``<ol>`` | Ordered list | **start; type; reversed** | No |
| ``<li>`` | List item | **value; class** | No |
| ``<table>`` | Tabular data container | **border; summary** | No |
| ``<tr>`` | Table row | **class; id** | No |
| ``<th>`` | Table header cell | **scope; colspan; rowspan** | No |
| ``<td>`` | Table data cell | **colspan; rowspan** | No |
| ``<form>`` | Form container | **action; method; enctype** | No |
| ``<input>`` | Input control | **type; name; value; placeholder; required; disabled** | Yes |
| ``<textarea>`` | Multi-line text input | **name; rows; cols; placeholder** | No |
| ``<button>`` | Clickable button | **type; disabled; name; value** | No |
| ``<select>`` | Dropdown list | **name; multiple; size** | No |
| ``<option>`` | Option in select | **value; selected; disabled** | No |
| ``<label>`` | Label for form control | **for** | No |
| ``<figure>`` | Self-contained media with caption | **class; id** | No |
| ``<figcaption>`` | Caption for figure | — | No |
| ``<audio>`` | Audio player | **src; controls; autoplay; loop** | No |
| ``<video>`` | Video player | **src; controls; autoplay; muted; poster** | No |
| ``<source>`` | Media source for audio/video | **src; type** | Yes |
| ``<iframe>`` | Embedded browsing context | **src; title; width; height; sandbox** | No |
| ``<canvas>`` | Drawing surface for graphics | **width; height** | No |
| ``<svg>`` | Scalable vector graphics | **viewBox; xmlns** | No |
| ``<meta ``http-equiv="refresh">`` | Page redirect/refresh | **content** | Yes |



### What is HTML
**HTML** (HyperText Markup Language) is the standard markup language used to create and structure content on the web. It defines **elements (tags)** that tell the browser how to display text, images, links, forms, and other content. HTML is semantic: tags convey meaning (e.g., headings, paragraphs, navigation), which helps browsers, search engines, and assistive technologies.

---

### Core HTML tags and common attributes
| **Tag** | **Purpose** | **Common Attributes** | **Self-closing** |
|---|---:|---|---:|
| **`<!DOCTYPE html>`** | Declares HTML5 document type | — | No |
| **`<html>`** | Root element of an HTML document | **lang** | No |
| **`<head>`** | Metadata container | — | No |
| **`<meta>`** | Metadata (charset, viewport) | **charset; name; content** | Yes |
| **`<title>`** | Document title shown in browser tab | — | No |
| **`<link>`** | Link external resources (CSS, icons) | **rel; href; type** | Yes |
| **`<script>`** | JavaScript inclusion | **src; async; defer; type** | No |
| **`<style>`** | Internal CSS | **type** | No |
| **`<body>`** | Visible page content | **class; id** | No |
| **`<header>`** | Introductory content or nav | **class; id** | No |
| **`<nav>`** | Navigation links | **aria-label; class** | No |
| **`<main>`** | Main page content | **id; class** | No |
| **`<section>`** | Thematic grouping of content | **id; class** | No |
| **`<article>`** | Self-contained composition | **id; class** | No |
| **`<aside>`** | Sidebar or tangential content | **id; class** | No |
| **`<footer>`** | Footer content | **id; class** | No |
| **`<h1>…<h6>`** | Headings, h1 highest level | **id; class** | No |
| **`<p>`** | Paragraph | **class; id** | No |
| **`<a>`** | Hyperlink | **href; target; rel; download** | No |
| **`<img>`** | Image | **src; alt; width; height; loading** | Yes |
| **`<ul>`** | Unordered list | **class; id** | No |
| **`<ol>`** | Ordered list | **start; type; reversed** | No |
| **`<li>`** | List item | **value; class** | No |
| **`<table>`** | Tabular data container | **border; summary** | No |
| **`<tr>`** | Table row | **class; id** | No |
| **`<th>`** | Table header cell | **scope; colspan; rowspan** | No |
| **`<td>`** | Table data cell | **colspan; rowspan** | No |
| **`<form>`** | Form container | **action; method; enctype** | No |
| **`<input>`** | Input control | **type; name; value; placeholder; required; disabled** | Yes |
| **`<textarea>`** | Multi-line text input | **name; rows; cols; placeholder** | No |
| **`<button>`** | Clickable button | **type; disabled; name; value** | No |
| **`<select>`** | Dropdown list | **name; multiple; size** | No |
| **`<option>`** | Option in select | **value; selected; disabled** | No |
| **`<label>`** | Label for form control | **for** | No |
| **`<figure>`** | Self-contained media with caption | **class; id** | No |
| **`<figcaption>`** | Caption for figure | — | No |
| **`<audio>`** | Audio player | **src; controls; autoplay; loop** | No |
| **`<video>`** | Video player | **src; controls; autoplay; muted; poster** | No |
| **`<source>`** | Media source for audio/video | **src; type** | Yes |
| **`<iframe>`** | Embedded browsing context | **src; title; width; height; sandbox** | No |
| **`<canvas>`** | Drawing surface for graphics | **width; height** | No |
| **`<svg>`** | Scalable vector graphics | **viewBox; xmlns** | No |
| **`<meta http-equiv="refresh">`** | Page redirect/refresh | **content** | Yes |

---

### Global attributes used on most elements
- **`id`** — unique identifier for the element.  
- **`class`** — one or more class names for styling and selection.  
- **`style`** — inline CSS styles.  
- **`title`** — advisory tooltip text.  
- **`data-*`** — custom data attributes (e.g., `data-user-id="123"`).  
- **`hidden`** — boolean to hide element.  
- **`tabindex`** — keyboard navigation order.  
- **`aria-*`** — accessibility attributes (e.g., `aria-label`, `aria-hidden`).  

---

### Form and media attributes to know
- **Form**: **`action`**, **`method`** (`GET`/`POST`), **`enctype`** (`multipart/form-data`), **`novalidate`**, **`autocomplete`**.  
- **Input types**: `text`, `password`, `email`, `number`, `tel`, `url`, `checkbox`, `radio`, `file`, `date`, `datetime-local`, `range`, `search`, `color`, `hidden`.  
- **Validation attributes**: **`required`**, **`min`**, **`max`**, **`minlength`**, **`maxlength`**, **`pattern`**, **`step`**.  
- **Media**: **`controls`**, **`autoplay`**, **`muted`**, **`loop`**, **`preload`**, **`poster`**, **`loading="lazy"`** for images.

---

### HTML Roadmap for learning and mastery
1. **Basics** — Learn document structure, tags listed above, attributes, and how browsers render HTML.  
2. **Semantics and Accessibility** — Use semantic tags (`header`, `main`, `nav`, `article`, `section`, `footer`) and **ARIA** attributes for screen readers.  
3. **Forms and Validation** — Build forms, understand input types, client-side validation, and form submission.  
4. **Media and Graphics** — Work with `<img>`, `<picture>`, `<audio>`, `<video>`, `<canvas>`, and `<svg>`.  
5. **Responsive HTML** — Combine HTML with CSS (flexbox, grid) and meta viewport for mobile-first design.  
6. **Performance and Best Practices** — Use lazy loading, optimize images, minimize DOM size, prefer semantic markup.  
7. **Progressive Enhancement** — Ensure content works without JavaScript; add JS for richer behavior.  
8. **Modern APIs** — Learn Fetch, Web Storage, Service Workers, and how HTML integrates with them.  
9. **SEO and Metadata** — Use proper headings, meta tags, structured data, and accessible links.  
10. **Testing and Validation** — Validate HTML (W3C), test with screen readers, and run performance audits.

---

If you want, I can:
- **Expand any table** into more tags and attributes.  
- Provide **code examples** for semantic layout, forms, or responsive patterns.  
- Create a **compact printable cheat sheet** of tags and attributes. Which would you like next?

### HTML Cheat Sheet — Compact Printable Reference

---

### Document skeleton
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <title>Page Title</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <!-- content -->
  </body>
</html>
```

---

### Essential tags and one-line purpose
| **Tag** | **Purpose** | **Common attributes** |
|---|---:|---|
| **`<html>`** | Root element | **lang** |
| **`<head>`** | Metadata container | — |
| **`<meta>`** | Charset, viewport, SEO | **charset; name; content** |
| **`<title>`** | Browser tab title | — |
| **`<link>`** | External resources (CSS, icons) | **rel; href; type** |
| **`<script>`** | JS inclusion | **src; async; defer; type** |
| **`<body>`** | Visible content | **class; id** |
| **`<header>`** | Intro/navigation | **class; id** |
| **`<nav>`** | Navigation links | **aria-label; class** |
| **`<main>`** | Main page content | **id; class** |
| **`<section>`** | Thematic grouping | **id; class** |
| **`<article>`** | Self-contained content | **id; class** |
| **`<aside>`** | Sidebar/tangential content | **id; class** |
| **`<footer>`** | Footer content | **id; class** |
| **`<h1>…<h6>`** | Headings | **id; class** |
| **`<p>`** | Paragraph | **class; id** |
| **`<a>`** | Link | **href; target; rel; download** |
| **`<img>`** | Image | **src; alt; width; height; loading** |
| **`<ul>` / `<ol>` / `<li>`** | Lists | **start; type; value** |
| **`<table>` / `<tr>` / `<th>` / `<td>`** | Tabular data | **colspan; rowspan; scope** |
| **`<form>`** | Form container | **action; method; enctype** |
| **`<input>`** | Input control | **type; name; value; placeholder; required** |
| **`<textarea>`** | Multi-line input | **name; rows; cols; placeholder** |
| **`<button>`** | Clickable button | **type; disabled; name; value** |
| **`<select>` / `<option>`** | Dropdown | **multiple; selected; value** |
| **`<figure>` / `<figcaption>`** | Media + caption | — |
| **`<audio>` / `<video>`** | Media players | **src; controls; autoplay; loop; muted** |
| **`<iframe>`** | Embedded content | **src; title; sandbox; width; height** |
| **`<canvas>` / `<svg>`** | Graphics | **width; height; viewBox** |

---

### Global attributes (use on most elements)
- **`id`** — unique identifier.  
- **`class`** — CSS/JS hooks.  
- **`style`** — inline CSS.  
- **`title`** — tooltip text.  
- **`data-*`** — custom data attributes.  
- **`hidden`** — hide element.  
- **`tabindex`** — keyboard order.  
- **`aria-*`** — accessibility (e.g., `aria-label`, `aria-hidden`).

---

### Common input types & validation
| **Type** | **Use** | **Validation attrs** |
|---|---:|---|
| **text** | Free text | **required; minlength; maxlength; pattern** |
| **email** | Email address | **required; pattern** |
| **password** | Password | **minlength; required** |
| **number** | Numeric input | **min; max; step** |
| **date / datetime-local** | Dates | **min; max** |
| **checkbox / radio** | Options | **checked; required** |
| **file** | Uploads | **accept; multiple** |
| **range** | Slider | **min; max; step** |
| **hidden** | Hidden value | — |

---

### Semantic layout example
```html
<body>
  <header>
    <nav aria-label="Main navigation">
      <a href="/">Home</a>
      <a href="/about">About</a>
    </nav>
  </header>

  <main>
    <article>
      <h1>Article Title</h1>
      <p>Intro paragraph…</p>
    </article>

    <aside aria-label="Related">
      <h2>Related</h2>
    </aside>
  </main>

  <footer>
    <p>&copy; 2026</p>
  </footer>
</body>
```

---

### Form example (accessible)
```html
<form action="/submit" method="post" novalidate>
  <label for="name">Full name</label>
  <input id="name" name="name" type="text" required />

  <label for="email">Email</label>
  <input id="email" name="email" type="email" required />

  <label for="message">Message</label>
  <textarea id="message" name="message" rows="5"></textarea>

  <button type="submit">Send</button>
</form>
```

---

### Responsive & performance tips
- Include `<meta name="viewport" content="width=device-width,initial-scale=1">`.  
- Use **`loading="lazy"`** on images for deferred loading.  
- Prefer **semantic tags** for SEO and accessibility.  
- Use **`srcset`** and `<picture>` for responsive images.  
- Minimize DOM depth and avoid excessive inline styles.  

---

### Accessibility quick rules
- Always provide **`alt`** for images; empty `alt=""` for decorative images.  
- Use **labels** for form controls (`<label for="id">`).  
- Use **landmark roles** (`<nav>`, `<main>`, `<header>`, `<footer>`).  
- Add **`aria-*`** only when semantic HTML is insufficient.  
- Ensure **keyboard focus** order and visible focus styles.

---

### Useful snippets
**Responsive image**
```html
<picture>
  <source srcset="image-large.webp" type="image/webp" media="(min-width:800px)">
  <img src="image.jpg" alt="Description" loading="lazy">
</picture>
```

**Prefetch CSS**
```html
<link rel="preload" href="styles.css" as="style" onload="this.rel='stylesheet'">
<noscript><link rel="stylesheet" href="styles.css"></noscript>
```

---

If you want, I can now:
- **Generate a printable one-page PDF-style layout** (formatted cheat sheet) you can copy and save.  
- **Expand any section** into more tags, attributes, and examples (forms, media, ARIA patterns).  
- **Create a short quiz** to test HTML knowledge based on this sheet.  

Tell me which of those you want and I’ll prepare it.
