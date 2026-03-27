# Media Query

A media query in CSS is used to make your website responsive—meaning it adjusts its layout and design based on the screen size, device type, or conditions like width, height, orientation, etc.

### 🔹 Basic Syntax
```
@media (condition) {
  /* CSS rules */
}
```
### 🔹 Example: Change background for smaller screens
```
body {
  background-color: blue;
}

@media (max-width: 768px) {
  body {
    background-color: red;
  }
}
```
👉 When screen width is 768px or less, background turns red.

### 🔹 Common Media Query Breakpoints

#### /* Mobile */
```
@media (max-width: 480px) { }
```
#### /* Tablets */
```
@media (max-width: 768px) { }
```
#### /* Small laptops */
```
@media (max-width: 1024px) { }
```

#### /* Large screens */

```
 @media (min-width: 1200px) { }

🔹 Using Multiple Conditions

@media (min-width: 600px) and (max-width: 900px) {
  body {
    background-color: green;
  }
}

```
🔹 Orientation Example
```
@media (orientation: landscape) {
  body {
    font-size: 18px;
  }
}
```
### 🔹 Responsive Navbar Example
```
.nav {
  display: flex;
}

@media (max-width: 600px) {
  .nav {
    flex-direction: column;
  }
}
```