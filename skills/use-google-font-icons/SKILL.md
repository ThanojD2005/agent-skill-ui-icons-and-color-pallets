---
name: use-google-font-icons
description: When have requirment to add/use icons in the project, use google font icons.
---

### Overview
Whenever a project requires icons, always use **Google Font Icons** (specifically **Google Material Symbols**). Follow the standard workflow below to discover, integrate, customize, and handle edge cases for icons.

---

### Step-by-Step Instructions

#### 1. Import Google Font Icons into the Project

Ensure the Material Symbols stylesheet is loaded in your project before using any icons:
- **HTML `<head>` link:**
  ```html
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
  ```
- **Or CSS `@import`:**
  ```css
  @import url('https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200');
  ```

#### 2. Search & Select the Required Icon
- Visit [Google Fonts Icons](https://fonts.google.com/icons).
- Search using descriptive keywords and common synonyms (e.g., search for "trash" to find `delete`, "cog" or "gear" to find `settings`, "heart" to find `favorite`).
- Choose the icon and note its exact lowercase snake_case name (e.g., `account_circle`, `check_circle`, `shopping_cart`).

#### 3. Standard Implementation
- Insert the icon using a `<span>` element with the `material-symbols-outlined` class:
  ```html
  <span class="material-symbols-outlined">icon_name</span>
  ```
- For accessibility:
  - If the icon is decorative or next to visible text, add `aria-hidden="true"`.
  - If the icon functions as a standalone button/link without visible text, provide an `aria-label` on the parent button or include visually hidden screen-reader text.

#### 4. Handling Missing or Unavailable Icons
If the exact icon needed does not exist on Google Fonts:
1. **Find a Closely Related Icon**: Pick an existing icon with similar geometry or concept (e.g., use `arrow_forward` for diagonal arrows, `undo` for redo, `visibility` for inspection).
2. **Modify with CSS**: Adapt the icon to the desired look using CSS properties such as `transform` (`rotate`, `scaleX`, `scaleY`), `filter`, `clip-path`, or pseudo-elements.
3. **Mandatory Documentation Comment**: You **MUST** add a comment above the HTML element stating that the icon was adapted with CSS:
   ```html
   <!-- This icon is not available on Google Fonts; I have used the available icon by modifying it with the help of CSS properties. -->
   ```

#### 5. Styling & Variable Font Settings
- **Size & Alignment**: Set `font-size` and `display: inline-flex; align-items: center; vertical-align: middle;` for clean alignment with text.
- **Color**: Icons inherit the current text `color` by default (`currentColor`), or can be styled with explicit hex/hsl values.
- **Variable Font Axes**: Customize icon appearance using `font-variation-settings`:
  - `'FILL'`: `0` for outlined, `1` for filled.
  - `'wght'`: `100` to `700` (e.g., `400` normal, `600` bold).
  - `'GRAD'`: `-25` to `200` (grade/emphasis).
  - `'opsz'`: Optical size, typically matching the font size (`20` to `48`).

---

Example:

### 1. Include Google Fonts Icons in HTML `<head>`
```html
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
```

### 2. Standard Icon Usage
```html
<!-- Standard icons -->
<span class="material-symbols-outlined">search</span>
<span class="material-symbols-outlined">home</span>
<span class="material-symbols-outlined">settings</span>
```

### 3. Modified Icon with CSS (When Exact Icon Is Not Available)
When an exact icon isn't available in Google Fonts, adapt an existing icon using CSS transforms/filters and include the required comment:

```html
<!-- This icon is not available on Google Fonts; I have used the available icon by modifying it with the help of CSS properties. -->
<span class="material-symbols-outlined icon-arrow-diagonal">arrow_forward</span>

<!-- This icon is not available on Google Fonts; I have used the available icon by modifying it with the help of CSS properties. -->
<span class="material-symbols-outlined icon-undo-flipped">undo</span>
```

```css
/* Rotated to create an arrow_outward / diagonal arrow */
.icon-arrow-diagonal {
  display: inline-block;
  transform: rotate(-45deg);
  color: #1a73e8;
  font-size: 24px;
}

/* Flipped horizontally to serve as a redo variant */
.icon-undo-flipped {
  display: inline-block;
  transform: scaleX(-1);
  color: #5f6368;
}
```
