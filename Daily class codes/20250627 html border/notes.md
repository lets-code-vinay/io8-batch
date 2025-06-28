# CSS Revision Notes

## 1. Display: `inline`, `block`, `inline-block`

### create Grid of divs with p tag

- **block**: Takes full width, starts on a new line.  
   Example: `<div>`, `<p>`, `<h1>`
  ```css
  div {
    display: block;
  }
  ```
- **inline**: Takes only as much width as needed, does not start on a new line.  
   Example: `<span>`, `<a>`
  ```css
  span {
    display: inline;
  }
  ```
- **inline-block**: Behaves like inline but allows width/height.
  ```css
  .box {
    display: inline-block;
    width: 100px;
    height: 50px;
  }
  ```

---

## 2. External CSS

- CSS is written in a separate `.css` file and linked in HTML.
  ```html
  <link rel="stylesheet" href="styles.css" />
  ```

---

## 3. Global Margin/Padding Reset

- Remove default browser margin/padding for consistency.
  ```css
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  ```

---

## 4. Borders

### Basic Border

```css
div {
  border: 1px solid red;
}
```

### Border Properties

1. **border-style**:  
    `solid`, `dashed`, `dotted`, `double`, `inset`, `outset`, `ridge`, `groove`, `hidden`, `none`

   ```css
   border-style: dashed;
   ```

2. **border-width**:  
    Controls thickness.

   ```css
   border-width: 2px;
   ```

3. **Shorthand**:  
    Combine width, style, color.

   ```css
   border: 2px double blue;
   ```

4. **border-color**:

   ```css
   border-color: green;
   ```

5. **Border Side Styling**:

   ```css
   border-top: 1px double red;
   border-left: 1px dotted green;
   border-right: 1px double red;
   ```

6. **border-radius**:

   - Makes rounded corners.
   - To make a circle:
     - Height = Width
     - `border-radius: 50%;`
   - To make a capsule:
     - `border-radius: 150px;` (large px value)
   - To make an ellipse:
     - `border-radius: 50%;` (height ≠ width)

   ```css
   .circle {
     width: 100px;
     height: 100px;
     border-radius: 50%;
   }
   ```

7. **border-image**:
   - Use an image as a border.
   ```css
   div {
     border: 10px solid transparent;
     border-image: url("https://www.w3schools.com/cssref/border.png") 30 round;
   }
   ```
   - [Reference image](https://www.w3schools.com/cssref/border.png)

---

## 5. Background Image

1. **Add image as background**

   ```css
   .bg {
     background-image: url("image.jpg");
   }
   ```

2. **Image sources**

   - Local: `url('images/bg.jpg')`
   - Online: `url('https://example.com/bg.jpg')`

3. **Background Filters**

   ```css
   .bg {
     filter: blur(2px) brightness(0.8) grayscale(50%);
   }
   ```

4. **background-position**

   ```css
   background-position: center;
   background-position: 10% 50%;
   ```

5. **background-position-x / background-position-y**

   ```css
   background-position-x: right;
   background-position-y: bottom;
   ```

6. **background-repeat**

   ```css
   background-repeat: no-repeat;
   background-repeat: repeat-x;
   ```

7. **background-size**
   ```css
   background-size: cover;
   background-size: 100px 100px;
   ```

---

## 6. Types of Units in Web Development

| Unit | Description                                   |
| ---- | --------------------------------------------- |
| px   | Pixels (fixed size, 96px = 1 inch)            |
| %    | Percentage (relative to parent)               |
| vw   | Viewport width (1vw = 1% of viewport width)   |
| vh   | Viewport height (1vh = 1% of viewport height) |
| em   | Relative to element's font-size               |
| rem  | Relative to root (`html`) font-size           |

**Example:**

```css
.box {
  width: 50vw;
  height: 10vh;
  padding: 2em;
  margin: 1rem;
}
```

---
