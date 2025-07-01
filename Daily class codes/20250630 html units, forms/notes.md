## What are units?

- Units are used for measurement.

1. distance--> meter, kilometer, centimeter
2. weight --> gram, kilogram, ton
3. energy --> watt, joules
4. liquid --> litre, milliliter, kilo-liter
5. web --> pixel, %age, vh, vw, rem, em

## Types of Units in Web Development

Web development uses various units to define sizes, spacing, and layout. Here’s a detailed explanation of the most common units, along with code examples:

### 1. `px` (Pixels)

- **Definition:** An absolute unit representing a single dot on the screen. 96px equals 1 inch on standard displays.
- **Usage:** Fixed-size elements.

#### 96 pixel === 1 inch

```css
.box {
  width: 200px;
  height: 100px;
  background: #4caf50;
}
```

### 2. `%` (Percentage)

- **Definition:** A relative unit based on the parent element’s size.
- **Usage:** Responsive layouts.

```css
.container {
  width: 80%;
  background: #2196f3;
}
```

### 3. `vw` (Viewport Width)

- **Definition:** 1vw equals 1% of the viewport’s width.
- **Usage:** Sizing elements relative to the browser window.

```css
.header {
  width: 100vw;
  height: 10vw;
  background: #ff9800;
}
```

### 4. `vh` (Viewport Height)

- **Definition:** 1vh equals 1% of the viewport’s height.
- **Usage:** Full-screen sections.

```css
.fullscreen {
  height: 100vh;
  background: #9c27b0;
}
```

### 5. `em` (Element)

- **Definition:** Relative to the font-size of the current element.
- **Usage:** Scalable spacing and font sizes.

```css
.text {
  font-size: 2em; /* 2 times the parent’s font size */
  margin: 1em; /* equal to the element’s font size */
}
```

### 6. `rem` (Root Element)

- **Definition:** Relative to the font-size of the root (`<html>`) element.
- **Usage:** Consistent sizing across the document.

```css
html {
  font-size: 16px;
}
.title {
  font-size: 2rem; /* 32px */
  padding: 1rem; /* 16px */
}
```

---

**Summary Table:**

| Unit | Relative To     | Example Value | Use Case                |
| ---- | --------------- | ------------- | ----------------------- |
| px   | Screen pixels   | 100px         | Fixed size              |
| %    | Parent element  | 50%           | Responsive width/height |
| vw   | Viewport width  | 10vw          | Full-width layouts      |
| vh   | Viewport height | 50vh          | Full-height sections    |
| em   | Current element | 2em           | Scalable spacing        |
| rem  | Root element    | 1.5rem        | Consistent sizing       |

## Color Types in CSS

CSS supports several ways to specify colors. Here are the most common types, with explanations and code examples:

### 1. Named Colors

- **Definition:** Use predefined color names recognized by CSS (e.g., `red`, `blue`, `green`).
- **Usage:** Quick and easy for common colors.

```css
.element {
  color: blue;
  background-color: lightgray;
}
```

### 2. Hexadecimal (`#RRGGBB` or `#RGB`)

- **Definition:** A hex code starts with `#` followed by 3 or 6 hexadecimal digits representing red, green, and blue.
- **Usage:** Precise color selection.

`Hexadecimal`

- 0
- 1
- 2
- 3
- 4
- 5
- 6
- 7
- 8
- 9
- A
- B
- C
- D
- E
- F

`# RR GG BB`
`# 0f 0f 0f`
`#000000` Black
`#ffffff` White

```css
.element {
  color: #ff5733; /* 6-digit hex */
  background: #0f0; /* 3-digit hex (same as #00ff00) */
}
```

### 3. RGB (`rgb()`)

- **Definition:** Specifies color using Red, Green, and Blue values (0–255).
- **Usage:** Useful for dynamic color generation.

- `Red --` background-color: rgb(255, 0, 0);
- `Green--` background-color: rgb(0, 255, 0);
- `Blue--` background-color: rgb(0, 0, 255);
- `White--` background-color: rgb(255, 255, 255);
- `--` background-color: rgb(0, 0, 0);

```css
.element {
  color: rgb(255, 99, 71); /* tomato */
  background: rgb(240, 240, 240); /* light gray */
}
```

### 4. RGBA (`rgba()`)

- **Definition:** Like `rgb()`, but with an Alpha (opacity) value (0–1).
- **Usage:** For transparent or semi-transparent colors.

```css
.element {
  background: rgba(0, 128, 255, 0.5); /* 50% transparent blue */
}
```

### 5. HSL (`hsl()`)

- **Definition:** Uses Hue (0–360), Saturation (0%–100%), and Lightness (0%–100%).
- **Usage:** Easier to adjust color variations.

```css
.element {
  color: hsl(120, 100%, 25%); /* dark green */
}
```

### 6. HSLA (`hsla()`)

- **Definition:** Like `hsl()`, but with Alpha (opacity).
- **Usage:** For transparent HSL colors.

```css
.element {
  background: hsla(340, 82%, 52%, 0.7); /* semi-transparent pink */
}
```

---

**Summary Table:**

| Type | Example Value              | Use Case                         |
| ---- | -------------------------- | -------------------------------- |
| Name | `red`, `blue`, `goldenrod` | Quick, common colors             |
| Hex  | `#ff5733`, `#0f0`          | Precise, web-safe colors         |
| RGB  | `rgb(255, 99, 71)`         | Dynamic, script-generated colors |
| RGBA | `rgba(0, 128, 255, 0.5)`   | Transparent backgrounds          |
| HSL  | `hsl(120, 100%, 25%)`      | Easy color adjustments           |
| HSLA | `hsla(340, 82%, 52%, 0.7)` | Transparent HSL colors           |

## Gradients in CSS

Gradients in CSS allow you to create smooth transitions between two or more colors. They can be used as backgrounds for elements and come in three main types: linear, radial, and conic gradients.

### 1. Linear Gradient

- **Definition:** A linear gradient transitions colors along a straight line (horizontal, vertical, or diagonal).
- **Syntax:** `linear-gradient(direction, color-stop1, color-stop2, ...)`
- **Direction:** Can be specified using angles (e.g., `90deg`) or keywords (`to right`, `to bottom`, etc.).

**Example: Horizontal Linear Gradient**

```css
.box-linear {
  background: linear-gradient(to right, #ff7e5f, #feb47b);
  width: 300px;
  height: 100px;
}
```

**Example: Diagonal Linear Gradient with Multiple Colors**

```css
.box-linear-multi {
  background: linear-gradient(45deg, #2193b0, #6dd5ed, #b2fefa);
  width: 300px;
  height: 100px;
}
```

#### Additional Options

- **Repeating Linear Gradient:**  
  Use `repeating-linear-gradient()` for repeating patterns.

  ```css
  .box-repeating-linear {
    background: repeating-linear-gradient(
      45deg,
      #606dbc,
      #606dbc 10px,
      #465298 10px,
      #465298 20px
    );
    width: 300px;
    height: 100px;
  }
  ```

---

### 2. Radial Gradient

- **Definition:** A radial gradient radiates from an origin (center by default) outward in a circular or elliptical shape.
- **Syntax:** `radial-gradient(shape size at position, color-stop1, color-stop2, ...)`
- **Shape:** Can be `circle` or `ellipse`.
- **Position:** Default is `center`, but can be set (e.g., `at top left`).

**Example: Circular Radial Gradient**

```css
.box-radial {
  background: radial-gradient(circle, #ffaf7b, #d76d77, #3a1c71);
  width: 300px;
  height: 100px;
}
```

**Example: Elliptical Radial Gradient Positioned**

```css
.box-radial-ellipse {
  background: radial-gradient(ellipse at left, #43cea2, #185a9d);
  width: 300px;
  height: 100px;
}
```

#### Additional Options

- **Repeating Radial Gradient:**  
  Use `repeating-radial-gradient()` for repeating patterns.

  ```css
  .box-repeating-radial {
    background: repeating-radial-gradient(
      circle,
      #f7971e,
      #ffd200 20px,
      #f7971e 40px
    );
    width: 300px;
    height: 100px;
  }
  ```

---

### 3. Conic Gradient

- **Definition:** A conic gradient transitions colors around a central point, like the colors on a pie chart.
- **Syntax:** `conic-gradient(from angle at position, color-stop1, color-stop2, ...)`
- **Starting Angle:** Optional, default is `0deg`.
- **Position:** Default is `center`.

**Example: Basic Conic Gradient**

```css
.box-conic {
  background: conic-gradient(#fcb045, #fd1d1d, #833ab4, #fcb045);
  width: 300px;
  height: 100px;
}
```

**Example: Conic Gradient with Segments**

```css
.box-conic-segments {
  background: conic-gradient(
    red 0% 25%,
    yellow 25% 50%,
    green 50% 75%,
    blue 75% 100%
  );
  width: 300px;
  height: 100px;
}
```

#### Additional Options

- **Repeating Conic Gradient:**  
  Use `repeating-conic-gradient()` for repeating patterns.

  ```css
  .box-repeating-conic {
    background: repeating-conic-gradient(
      from 0deg,
      #e66465 0deg 30deg,
      #9198e5 30deg 60deg
    );
    width: 300px;
    height: 100px;
  }
  ```

---

### Summary Table

| Gradient Type | Syntax Example                         | Use Case                          |
| ------------- | -------------------------------------- | --------------------------------- |
| Linear        | `linear-gradient(to right, red, blue)` | Backgrounds, buttons, borders     |
| Radial        | `radial-gradient(circle, red, blue)`   | Circular highlights, overlays     |
| Conic         | `conic-gradient(red, yellow, green)`   | Pie charts, color wheels, effects |

## gradients in css
