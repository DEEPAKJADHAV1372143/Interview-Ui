### Angular Material Interview Questions and Answers

Below is a focused, practical set of **Angular Material** interview questions and concise, interview-ready answers. It covers core concepts, components, theming, accessibility, performance, and common implementation patterns you’re likely to face in frontend interviews.

---

### 1. What is Angular Material?
**Answer:**  
**Angular Material** is an official UI component library for Angular that implements Google’s Material Design. It provides pre-built, accessible, and themable UI components (buttons, forms, navigation, dialogs, tables, etc.) that integrate with Angular’s reactive patterns, change detection, and dependency injection.

---

### 2. How do you install and set up Angular Material in an Angular project?
**Answer:**  
Install via npm:  
```bash
ng add @angular/material
```
This runs a schematic that installs packages, adds BrowserAnimationsModule, and offers to set up a theme and typography. Alternatively, install `@angular/material`, `@angular/cdk`, and `@angular/animations` and import `BrowserAnimationsModule` and the Material modules you need.

---

### 3. What is Angular CDK and how does it relate to Angular Material?
**Answer:**  
**CDK (Component Dev Kit)** is a library of behavior primitives (overlay, accessibility, drag-drop, scrolling, portals, etc.) used by Angular Material. CDK provides low-level building blocks so you can build custom components without reimplementing common behaviors. Angular Material builds on CDK to provide styled, ready-to-use components.

---

### 4. How does Angular Material handle theming?
**Answer:**  
Angular Material uses **Sass-based theming**. You define a **palette** (primary, accent, warn) and a **theme** (light or dark) using Material’s Sass mixins. Then include `@include mat-core();` and `@include angular-material-theme($my-theme);`. You can create custom palettes, override component variables, and support multiple themes by switching CSS classes or using CSS variables (newer approaches).

---

### 5. Explain the difference between MatDialog and MatSnackBar.
**Answer:**  
- **MatDialog**: Modal dialog for complex interactions, supports custom components, data injection, and returns an `afterClosed()` observable with results.  
- **MatSnackBar**: Lightweight transient notification (toast) for brief messages and optional action; returns a `MatSnackBarRef` and `afterDismissed()` observable.

---

### 6. How do you open a dialog and pass data to it?
**Answer:**  
```ts
// Open dialog
const ref = this.dialog.open(MyDialogComponent, {
  width: '400px',
  data: { id: 1, name: 'Deepak' }
});

// In MyDialogComponent
constructor(@Inject(MAT_DIALOG_DATA) public data: any) {}
```
Use `MatDialog` service to open and `MAT_DIALOG_DATA` injection token to receive data. Use `dialogRef.close(result)` to return data.

---

### 7. What is MatTable and how do you implement sorting, pagination, and filtering?
**Answer:**  
**MatTable** is a Material data-table component. Use `MatTableDataSource` for simple data handling. For features:
- **Sorting**: Add `<mat-sort>` and `MatSort` directive; set `dataSource.sort = this.sort`.
- **Pagination**: Use `<mat-paginator>` and set `dataSource.paginator = this.paginator`.
- **Filtering**: Use `dataSource.filter = filterValue.trim().toLowerCase()` and optionally override `filterPredicate` for custom logic.

Example:
```ts
dataSource = new MatTableDataSource(ELEMENT_DATA);
@ViewChild(MatSort) sort: MatSort;
@ViewChild(MatPaginator) paginator: MatPaginator;

ngAfterViewInit() {
  this.dataSource.sort = this.sort;
  this.dataSource.paginator = this.paginator;
}
```

---

### 8. How do you lazy-load Angular Material modules to reduce bundle size?
**Answer:**  
Import only the Material modules you need rather than a single shared module with everything. Use **feature modules** and import Material modules inside them. For route-based lazy loading, include Material imports in the lazy-loaded module so they’re bundled separately. Also consider using Angular CLI’s differential loading and build optimizations.

---

### 9. What is MatFormField and how do you use it with form controls?
**Answer:**  
`<mat-form-field>` is a wrapper for form controls that provides Material styling, floating labels, hints, and error messages. Use with `matInput` directive:
```html
<mat-form-field>
  <input matInput placeholder="Name" [formControl]="nameControl" required>
  <mat-error *ngIf="nameControl.hasError('required')">Name required</mat-error>
</mat-form-field>
```
Works with reactive forms and template-driven forms.

---

### 10. How does Angular Material support accessibility (a11y)?
**Answer:**  
Angular Material components are built with accessibility in mind: proper ARIA attributes, keyboard navigation, focus management, and screen-reader support. CDK provides `A11yModule` utilities (FocusMonitor, LiveAnnouncer). Developers must still provide semantic markup, `aria-*` attributes where needed, and ensure color contrast and focus visibility.

---

### 11. Explain MatStepper and when to use it.
**Answer:**  
`MatStepper` provides a wizard-like stepper UI for multi-step workflows. It supports linear and non-linear modes, step validation, and custom step content. Use when you need guided, sequential user input (e.g., multi-page forms).

---

### 12. How do you customize Angular Material component styles?
**Answer:**  
Preferred ways:
- **Theming with Sass**: Override theme variables and include custom theme mixins.
- **Component-level styles**: Use `::ng-deep` (deprecated, avoid) or global styles to override deep component styles.
- **CSS variables**: Newer approach—use CSS variables in your theme and override them at runtime.
- **Encapsulation**: Use `ViewEncapsulation.None` carefully for global overrides.
Best practice: use theming APIs and Sass variables rather than brittle deep selectors.

---

### 13. What is MatAutocomplete and how do you implement it?
**Answer:**  
`MatAutocomplete` provides suggestions as the user types. Use `matAutocomplete` directive with an input and a panel of `mat-option` elements. Typically combined with `FormControl` and `valueChanges` to filter options.
```html
<input type="text" [formControl]="ctrl" [matAutocomplete]="auto">
<mat-autocomplete #auto="matAutocomplete">
  <mat-option *ngFor="let opt of filteredOptions" [value]="opt">{{opt}}</mat-option>
</mat-autocomplete>
```

---

### 14. How do you implement responsive layouts with Angular Material?
**Answer:**  
Use **Angular Flex-Layout** (optional) or CSS Flexbox/Grid. Material provides responsive components (sidenav modes, breakpoints). Combine `@angular/flex-layout` directives (`fxLayout`, `fxFlex`) or CSS media queries and Material’s layout utilities to adapt to screen sizes.

---

### 15. Explain MatSidenav and its modes.
**Answer:**  
`MatSidenav` is a side navigation container. Modes:
- **over**: Sidenav overlays content (mobile-friendly).
- **push**: Sidenav pushes content aside.
- **side**: Sidenav is always visible and part of layout (desktop).
Control with `opened`, `mode`, and `fixedInViewport` properties.

---

### 16. How do you handle server-side pagination and sorting with MatTable?
**Answer:**  
Listen to `MatPaginator` and `MatSort` events and request data from the server with current page, pageSize, sortField, and sortDirection. Update the table’s `dataSource` with server response and set `length` to total items for paginator. Avoid using `MatTableDataSource` for large datasets; use a custom data source that fetches pages.

---

### 17. What is MatTooltip and how do you customize its position and delay?
**Answer:**  
`MatTooltip` shows brief hover text. Use `matTooltip`, `matTooltipPosition` (`above`, `below`, `left`, `right`), `matTooltipShowDelay`, and `matTooltipHideDelay` to control timing. For styling, override tooltip CSS classes or use theming.

---

### 18. How do you create a custom Angular Material component or extend an existing one?
**Answer:**  
Use CDK primitives (Overlay, Portal, A11y) to build custom components. To extend Material components, you can wrap them in your own component, reuse their templates, or extend classes (careful with private APIs). Prefer composition over inheritance and use CDK for behavior.

---

### 19. How do you test Angular Material components in unit tests?
**Answer:**  
Import required Material modules and `NoopAnimationsModule` (or `BrowserAnimationsModule`) in the TestBed. Use `fixture.detectChanges()` and query elements with `By.css`. For dialogs/snackbars, inject `MatDialog`/`MatSnackBar` and use spies or `MatDialogHarness` for harness-based testing.

---

### 20. What are Component Harnesses and why use them?
**Answer:**  
**Component Harnesses** (part of Angular CDK testing) are a stable, API-driven way to interact with Material components in tests. They abstract DOM details, making tests resilient to markup changes. Use `MatButtonHarness`, `MatDialogHarness`, `MatTableHarness`, etc., with `TestbedHarnessEnvironment`.

---

### 21. How do you implement dark mode with Angular Material?
**Answer:**  
Create a dark theme Sass palette and theme object. Apply the dark theme class to a top-level element (e.g., `<body class="dark-theme">`) and scope theme styles. Alternatively, use CSS variables to switch colors at runtime and toggle a class to switch themes.

---

### 22. How do you optimize performance when using many Material components?
**Answer:**  
- Import only needed modules.  
- Use `OnPush` change detection where possible.  
- Avoid heavy DOM trees; virtualize long lists (`cdk-virtual-scroll-viewport`).  
- Use lazy-loaded feature modules.  
- Use harnesses and `NoopAnimationsModule` in tests to speed them up.

---

### 23. Explain how overlays work in Angular Material.
**Answer:**  
Overlays (CDK Overlay) create floating panels (dialogs, menus, tooltips). They manage positioning, scroll strategies, and backdrop. Use `Overlay` service to create overlay refs, attach portals, and configure position strategies and scroll behavior.

---

### 24. How do you internationalize (i18n) Angular Material components?
**Answer:**  
Material components use Angular’s i18n for static text; for dynamic labels (e.g., paginator), provide `MatPaginatorIntl` service with translated strings. Replace or extend `MatPaginatorIntl` and provide it in your module.

---

### 25. Common pitfalls with Angular Material
**Answer:**  
- Importing entire Material library instead of specific modules (bundle bloat).  
- Overriding styles with `::ng-deep` leading to brittle CSS.  
- Not using `NoopAnimationsModule` in tests causing flakiness.  
- Relying on `MatTableDataSource` for server-side pagination of large datasets.  
- Forgetting accessibility considerations (labels, ARIA).

---

## Quick Practical Examples

**Open a dialog and get result**
```ts
const ref = this.dialog.open(EditDialogComponent, { data: item });
ref.afterClosed().subscribe(result => {
  if (result) this.save(result);
});
```

**MatTable with server-side paging (concept)**
```ts
paginator.page.subscribe(() => this.loadData());
sort.sortChange.subscribe(() => { this.paginator.pageIndex = 0; this.loadData(); });

loadData() {
  const params = {
    page: this.paginator.pageIndex,
    size: this.paginator.pageSize,
    sort: this.sort.active,
    dir: this.sort.direction
  };
  this.service.getData(params).subscribe(res => {
    this.data = res.items;
    this.paginator.length = res.total;
  });
}
```

**Theming (Sass snippet)**
```scss
@use '@angular/material' as mat;

$my-primary: mat.define-palette(mat.$indigo-palette);
$my-accent: mat.define-palette(mat.$pink-palette, A200, A100, A400);
$my-theme: mat.define-light-theme((color: (primary: $my-primary, accent: $my-accent)));

@include mat.core();
@include mat.all-component-themes($my-theme);
```

---
