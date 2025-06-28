# Today's Topics

## Display Properties

Display properties in CSS determine how elements are rendered on the user interface (UI) and impact the user experience (UX).

### Block Elements

- **Definition:** Block-level elements consume the full available width of their parent container and always start on a new line.
- **Characteristics:**
  - Occupy the entire width by default.
  - Accept width, height, margin, and padding properties.
  - The next element appears on a new line.
- **Examples:**  
   `<div>`, `<p>`, headings (`<h1>`–`<h6>`), `<hr>`, `<br>`, `<ol>`, `<ul>`, `<li>`

### Inline Elements

- **Definition:** Inline elements only take up as much width as necessary and do not force the next element onto a new line.
- **Characteristics:**
  - Do not accept width and height properties.
  - Margins and paddings are only respected horizontally (left and right).
  - Next element appears on the same line, if space allows.
- **Examples:**  
   `<span>`, `<a>`, `<img>`, `<input>`, formatting tags like `<b>`, `<i>`

### Types of Display Properties

1. **block** – Renders as a block-level element.
2. **inline** – Renders as an inline element.
3. **inline-block** – Behaves like an inline element but accepts width and height.
4. **flex** – Enables flexbox layout for flexible and responsive designs.
5. **grid** – Enables grid layout for two-dimensional layouts.
6. **none** – Hides the element from the page.
7. **inline-flex** – Flex container that behaves like an inline element.
8. **inline-grid** – Grid container that behaves like an inline element.

---

## Box Model

The CSS box model describes how elements are structured and spaced on a web page.

- **Content:** The actual content of the element (text, image, etc.).
- **Padding:** Space between the content and the border.
- **Border:** The line surrounding the padding (and content).
- **Margin:** Space outside the border, separating the element from others.
- **Position:** Determines the element's placement if positioning is applied.

```
| Margin | Border | Padding | Content | Padding | Border | Margin |
```

---

## Margin

Margins create space outside the element's border.

- **margin-auto:** Centers an element horizontally within its container.
- **margin-top:** Sets the top margin.
- **margin-right:** Sets the right margin.
- **margin-bottom:** Sets the bottom margin.
- **margin-left:** Sets the left margin.
- **Shorthand:**
  - `margin: 10px 0;` (top & bottom: 10px, left & right: 0)
  - `margin: 0px 10px;` (top & bottom: 0, left & right: 10px)
  - `margin: 0px 10px 5px 2px;` (top: 0, right: 10px, bottom: 5px, left: 2px; order is clockwise)

---

## Padding

Padding creates space inside the element, between the content and the border.

- **padding-top:** Sets the top padding.
- **padding-right:** Sets the right padding.
- **padding-bottom:** Sets the bottom padding.
- **padding-left:** Sets the left padding.
- **Shorthand:**
  - `padding: 10px 0;` (top & bottom: 10px, left & right: 0)
  - `padding: 0px 10px;` (top & bottom: 0, left & right: 10px)
  - `padding: 0px 10px 5px 2px;` (top: 0, right: 10px, bottom: 5px, left: 2px; order is clockwise)

---

## Border

Borders are lines that wrap around the padding and content of an element. You can control their width, style, and color using CSS properties like `border`, `border-width`, `border-style`, and `border-color`.
