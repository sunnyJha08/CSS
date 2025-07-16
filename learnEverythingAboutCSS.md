# 🎨 Complete CSS Guide (Beginner → Advanced)

---

## 📗 Beginner CSS

### 1. What is CSS & How It Works
```css
/*
CSS (Cascading Style Sheets) is used to style HTML content.
It controls the layout, colors, fonts, spacing, etc.
It can be applied in 3 ways: Inline, Internal, External.
*/
```

### 2. CSS Syntax
```css
/*
A CSS rule has:
1. Selector: HTML element to style
2. Property: The aspect you want to change
3. Value: The setting you want to apply
*/

h1 {
  color: blue; /* selector: h1, property: color, value: blue */
}
```

### 3. Types of CSS
```html
<!-- Inline -->
<h1 style="color: red">Hello</h1>

<!-- Internal -->
<style>
  p { font-size: 18px; }
</style>

<!-- External -->
<link rel="stylesheet" href="style.css" />
```

### 4. CSS Selectors
```css
/* Selectors target elements */
h1 {}            /* Element Selector */
#title {}        /* ID Selector */
.container {}    /* Class Selector */
div p {}         /* Descendant Selector */
div > p {}       /* Child Selector */
a:hover {}       /* Pseudo-class */
```

### 5. Colors, Units, Comments
```css
/* Colors */
body { background-color: #f0f0f0; color: rgb(50, 50, 50); }

/* Units */
p { font-size: 16px; width: 80%; padding: 1em; }

/* Comments */
/* This is a comment */
```

### 6. Text & Font Styling
```css
h1 {
  font-family: Arial, sans-serif;
  font-size: 36px;
  font-weight: bold;
  text-align: center;
  text-transform: uppercase;
  color: navy;
}
```

### 7. Box Model
```css
/* Every element is a box: content + padding + border + margin */
div {
  width: 200px;
  padding: 10px;
  border: 2px solid black;
  margin: 20px;
}
```

### 8. Display & Visibility
```css
/* Controls layout behavior */
span { display: inline; }
div { display: block; }
nav { display: flex; }
.hidden { display: none; visibility: hidden; }
```

### 9. Positioning
```css
/* Positions: static (default), relative, absolute, fixed, sticky */
.relative-box {
  position: relative;
  top: 10px;
  left: 20px;
}

.absolute-box {
  position: absolute;
  top: 0;
  right: 0;
}
```

---

## 📘 Intermediate CSS

### 10. Flexbox
```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}
```

### 11. Grid
```css
.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}
```

### 12. Responsive Design & Media Queries
```css
@media (max-width: 768px) {
  body {
    font-size: 14px;
  }
}
```

### 13. Pseudo-classes & Pseudo-elements
```css
a:hover {
  color: red;
}

p::first-line {
  font-weight: bold;
}
```

### 14. Transitions & Animations
```css
button {
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: green;
}

@keyframes slide {
  from { left: 0; }
  to { left: 100px; }
}

.box {
  animation: slide 1s ease-in-out;
}
```

### 15. Z-index & Layering
```css
.box1 {
  position: absolute;
  z-index: 1;
}

.box2 {
  position: absolute;
  z-index: 2; /* Appears on top */
}
```

### 16. CSS Variables
```css
:root {
  --main-color: #3498db;
}

h1 {
  color: var(--main-color);
}
```

---

## 📙 Advanced CSS

### 17. Advanced Selectors
```css
/* Attribute Selector */
a[target="_blank"] {
  color: orange;
}

/* Not Selector */
input:not([type="submit"]) {
  border: 1px solid gray;
}
```

### 18. Transformations
```css
.box {
  transform: rotate(45deg);
  transform: scale(1.2);
}
```

### 19. Complex Animations (Keyframes)
```css
@keyframes bounce {
  0%   { transform: translateY(0); }
  50%  { transform: translateY(-50px); }
  100% { transform: translateY(0); }
}

.ball {
  animation: bounce 1s infinite;
}
```

### 20. Responsive Units
```css
.container {
  width: 80vw;  /* 80% of viewport width */
  height: 50vh; /* 50% of viewport height */
  font-size: 2rem; /* relative to root element */
}
```

### 21. Clipping, Masking, Filters
```css
.image {
  clip-path: circle(50%);
  filter: grayscale(80%);
}
```

### 22. CSS Functions
```css
.box {
  width: calc(100% - 50px);
  font-size: clamp(1rem, 2vw, 3rem); /* responsive scaling */
}
```

---

## ✅ What's Next?
- Start practicing with small projects.
- Use this file as a reference cheat sheet.
- Build and style your own layouts.

> 🎯 Tip: Combine CSS with HTML and JavaScript to unlock full power!

---

Happy Styling! 💅✨
