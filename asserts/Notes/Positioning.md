## Positioning in CSS

The `position property` controls `how an element is placed` on the `page`.

### 📌 1. Static (default)
- `Default` for `all elements`
- Not affected by `top`, `left`, `right`, `bottom`
- Follows normal `document flow`

```
  position: static;
```

### 📌 2. Relative
- `Moves` relative to its `original position`
- Space is still preserved

```
  position: relative;
  top: 10px;
  left: 20px;
```

### 📌 3. Absolute


- `Positioned` relative to the `nearest positioned parent`
- If no parent → relative to `<body>`
- `Removed` from `normal flow` (no space reserved)

##### 💡 Example:

```
  .parent {
    position: relative;
  }
  .child {
    position: absolute;
    top: 0;
    right: 0;
  }
```

👉 Common use:

- Badges
- Tooltips
- Icons inside inputs

### 📌 4. Fixed

```
  position: fixed;
  top: 0;
```

#### ✅ Features:

- `Fixed relative` to the `viewport (screen)`
- `Stays in the same place` even` when scrolling`
- Removed from normal flow

👉 Common use:

 - Navbar
 - Floating buttons
 - Chat widgets

### 📌 5. Sticky

```
  position: sticky;
  top: 0;
```
#### ✅ Features:

-` Acts like relative` until scroll `reaches a point`
- Then behaves `like fixed`
- Requires top, left, etc.

👉 Common use:

- Sticky headers
- Section titles

### 🧠 6. Z-Index (Layering)

```
  z-index: 10;
```
#### ✅ Features:

- Controls stack order (which element is on top)
- Works only on positioned elements (relative, absolute, fixed, sticky)

🔥 Rule:

- Higher value → comes on top
- Lower value → goes behind

```
  .box1 { z-index: 1; }
  .box2 { z-index: 10; } /* appears above */

```

### 🚀 Real-World Summary

| Position   | Key Behavior             |
| ---------- | ------------------------ |
| `static`   | Default flow             |
| `relative` | Move from original spot  |
| `absolute` | Positioned inside parent |
| `fixed`    | Sticks to screen         |
| `sticky`   | Scroll → then sticks     |
| `z-index`  | Controls layers          |
