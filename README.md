# 📦 CSS — Box Sizing

The `box-sizing` property in CSS defines how the width and height of an element are calculated.

## 🛠️ Types of Box Sizing

### 1. `content-box`
- Width and height apply **only** to the content.
- Padding and borders are **added outside** the content box, which increases the total size of the element.

### 2. `border-box`
- Width and height include **content, padding, and border**.
- Makes it easier to size elements **predictably and consistently**.

## 💡 Example

```css
/* Content-box example (default) */
.box1 {
  box-sizing: content-box;
  width: 200px;
  padding: 20px;
  border: 5px solid black;
}
/* Total width = 200 + 40 (padding) + 10 (border) = 250px */

/* Border-box example */
.box2 {
  box-sizing: border-box;
  width: 200px;
  padding: 20px;
  border: 5px solid black;
}
/* Total width = 200px (everything included) */
