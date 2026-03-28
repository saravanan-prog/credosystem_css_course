# CSS animation  👇

## 🎯 1. Transition Property

Used to create smooth changes between two states (like hover).

### ✅ Syntax

- transition: property duration timing-function delay;

🔹 Example

```
.box {
  width: 100px;
  background: blue;
  transition: width 0.5s ease;
}

.box:hover {
  width: 200px;
}
```

👉 When you hover, width changes smoothly instead of instantly.

### 🔄 2. Transform

Used to move, rotate, scale, or skew elements.

#### 🔹 Common functions

   ```
    translate()  →  move
    scale()      →  resize
    rotate()     →  rotate
    skew()       →  tilt
   ```

🔹 Example
```
.box {
  transform: rotate(45deg);
}

.box:hover {
  transform: scale(1.2) rotate(10deg);  /* combined Example */
}
```

### 🎬 3. Keyframes

Defines steps of an animation.

✅ Syntax

```
@keyframes animationName {
  from { }
  to { }
}
```
OR

```
@keyframes animationName {
  0%   { }
  50%  { }
  100% { }
}
```


🔹 Example

```
@keyframes slide {
  0% { transform: translateX(0); }
  100% { transform: translateX(200px); }
}
```

## 🚀 4. Animation

- Applies the keyframes to an element.

✅ Syntax
- animation: name duration timing-function delay iteration-count direction;

🔹 Example
```
.box {
  animation: slide 2s ease infinite;
}
```

👉 This runs the slide animation continuously.

### 🔥 Full Example (All Combined)
```
.box {
  width: 100px;
  height: 100px;
  background: red;

  /* Transition */
  transition: transform 0.3s;

  /* Animation */
  animation: move 2s infinite;
}

.box:hover {
  transform: scale(1.3);
}

/* Keyframes */
@keyframes move {
  0%   { transform: translateX(0); }
  50%  { transform: translateX(150px); }
  100% { transform: translateX(0); }
}
```