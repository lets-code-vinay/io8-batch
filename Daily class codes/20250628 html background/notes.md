# Revision of border

# CSS Font Properties

CSS font properties allow you to control the appearance of text on your web pages. Here are the main properties:

## 1. `font-family`

Specifies the typeface for text.

```css
p {
  font-family: "Arial", "Helvetica", sans-serif;
}
```

### `google fonts` [https://fonts.google.com/]

## 2. `font-size`

Sets the size of the font.

```css
h1 {
  font-size: 2em;
}
```

**Common units:** `px`, `em`, `rem`, `%`

## 3. `font-weight`

Controls the thickness (boldness) of the text.

```css
strong {
  font-weight: bold;
}
```

**Common values:** `normal`, `bold`, `bolder`, `lighter`, `100`–`900`

## 4. `font-style`

Sets the style of the font (normal, italic, or oblique).

```css
em {
  font-style: italic;
}
```

## 5. `font-variant`

Controls the use of small-caps.

```css
span {
  font-variant: small-caps;
}
```

## 6. `font-stretch`

Adjusts the width of the text.

```css
p {
  font-stretch: expanded;
}
```

**Common values:** `normal`, `condensed`, `expanded`

## 7. `font`

A shorthand property for setting all font properties in one line.

```css
p {
  font: italic small-caps bold 16px/1.5 "Arial", sans-serif;
}
```

---

**Tip:** Always provide fallback fonts in `font-family` for better compatibility.

# CSS Background Properties

CSS background properties allow you to control the background effects of elements. Here are the main properties:

## 1. `background-color`

Sets the background color of an element.

```css
div {
  background-color: lightblue;
}
```

## 2. `background-image`

Sets one or more background images on an element.

```css
div {
  background-image: url("image.jpg");
}
```

## 3. `background-repeat`

Controls if/how a background image repeats.
**Common `background-repeat` values:**

1. `repeat` (default, repeats both horizontally and vertically)
2. `repeat-x` (repeats horizontally only)
3. `repeat-y` (repeats vertically only)
4. `no-repeat` (does not repeat)
5. `space` (repeats as many times as possible without clipping, spaces out the images)
6. `round` (repeats and scales the image so it fits exactly)

```css
div {
  background-repeat: no-repeat;
}
```

## 4. `background-position`

Sets the starting position of a background image.
**Common `background-position` values:**

- `top`
- `center`
- `left`
- `right`
- `bottom`
- `center top`
- `left bottom`
- `right top`
- `50% 50%` (center using percentage)
- `10px 20px` (specific pixel values)

### `background-position-x`

Specifies the horizontal position of a background image.

**Common values:**

- `left`
- `center`
- `right`
- Length values (e.g., `20px`, `50%`)

```css
div {
  background-position-x: right;
}
```

### `background-position-y`

Specifies the vertical position of a background image.

**Common values:**

- `top`
- `center`
- `bottom`
- Length values (e.g., `10px`, `75%`)

```css
div {
  background-position-y: bottom;
}
```

## 5. `background-size`

Specifies the size of the background image.
**Common `background-size` values:**

- `auto` (default, original image size)
- `cover` (scales the image to cover the element)
- `contain` (scales the image to fit inside the element)
- `100px 50px`
- `50% 100%`

```css
div {
  background-size: cover;
}
```

## 6. `background-attachment`

Sets whether a background image scrolls with the page or is fixed.
**Common `background-attachment` values:**

- `scroll` (default, background scrolls with the page)
- `fixed` (background is fixed relative to the viewport)
- `local` (background scrolls with the element's content)

```css
div {
  background-attachment: fixed;
}
```

## 7. `background`

A shorthand for setting all background properties in one line.

```css
div {
  background: #f0f0f0 url("image.jpg") no-repeat right top / cover;
}
```

---

# CSS Filter Properties

CSS filter properties allow you to apply visual effects to elements, such as blurring, changing colors, or adjusting opacity.

## Common Filter Functions

### 1. `blur()`

- **Description:** Applies a Gaussian blur to the element, making it appear out of focus.
- **Example:**
  ```css
  img {
    filter: blur(5px);
  }
  ```

### 2. `grayscale()`

- **Description:** Converts the element's colors to shades of gray, removing color saturation.
- **Example:**
  ```css
  img {
    filter: grayscale(100%);
  }
  ```

### 3. `sepia()`

- **Description:** Applies a sepia tone, giving the element a warm, brownish color (vintage effect).
- **Example:**
  ```css
  img {
    filter: sepia(100%);
  }
  ```

### 4. `saturate()`

- **Description:** Adjusts the intensity of the colors. Values above 100% increase saturation, below 100% decrease it.
- **Example:**
  ```css
  img {
    filter: saturate(200%);
  }
  ```

### 5. `brightness()`

- **Description:** Adjusts the brightness of the element. Values above 100% make it brighter, below 100% make it darker.
- **Example:**
  ```css
  img {
    filter: brightness(150%);
  }
  ```

### 6. `contrast()`

- **Description:** Adjusts the contrast of the element. Values above 100% increase contrast, below 100% decrease it.
- **Example:**
  ```css
  img {
    filter: contrast(120%);
  }
  ```

### 7. `invert()`

- **Description:** Inverts the colors of the element, producing a negative image effect.
- **Example:**
  ```css
  img {
    filter: invert(100%);
  }
  ```

### 8. `opacity()`

- **Description:** Adjusts the transparency of the element. Lower values make the element more transparent.
- **Example:**
  ```css
  img {
    filter: opacity(50%);
  }
  ```

### 9. `drop-shadow()`

- **Description:** Applies a shadow effect to the element, similar to `box-shadow` but as a filter.
- **Example:**
  ```css
  img {
    filter: drop-shadow(4px 4px 10px rgba(0, 0, 0, 0.5));
  }
  ```

## Combining Filters

You can combine multiple filters for complex effects:

```css
img {
  filter: grayscale(80%) blur(2px) opacity(70%) brightness(120%) contrast(110%);
}
```

> **Note:** The `filter` property works on most elements, especially images and backgrounds, to create various visual effects.

---

# CSS Gradients

Gradients are images generated by CSS, used as backgrounds.

## 1. Linear Gradient

Creates a gradient along a straight line.

```css
div {
  background: linear-gradient(to right, red, yellow, green);
}
```

**Explanation:**

- `to right` means the gradient goes from left to right.
- Colors transition from red to yellow to green.

## 2. Radial Gradient

Creates a gradient radiating from an origin (center by default).

```css
div {
  background: radial-gradient(circle, orange, white, blue);
}
```

**Explanation:**

- `circle` makes the gradient circular.
- Colors spread from orange at the center to white, then blue at the edges.

## 3. Conic Gradient

Creates a gradient rotated around a center point (like a pie chart).

```css
div {
  background: conic-gradient(from 0deg, red, yellow, green, red);
}
```

**Explanation:**

- `from 0deg` starts the gradient at the top.
- Colors transition in a circle: red → yellow → green → red.

---

**Tip:** Gradients can be used as `background-image` values and combined with other background properties for advanced effects.
