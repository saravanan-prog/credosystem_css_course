# 1. Display Property
 The display property controls how an element is shown on the page.
####  Common values:
- block
- inline
- inline-block
- none


# 📦 2. Block Elements (display: block)

Block elements take up the full width and start on a new line.

✅ Features:

- Always starts on a new line
- Takes full width (100% by default)
- Can set width, height, margin, padding

📌 Examples:

```
<div>
<p>
<h1> to <h6>
```

# 🧵 3. Inline Elements (display: inline)

Inline elements only take as much width as needed and stay in the same line.

✅ Features:

- No line break
- Width/height cannot be set properly
- Only horizontal margin/padding works well

📌 Examples:

```
<span>
<a>
<strong>
```

# 🔲 4. Inline-Block (display: inline-block)

This is a hybrid of inline and block.

✅ Features:

- Stays in the same line (like inline)
- You can set width & height (like block)

📌 Use case:

Perfect for buttons, cards, navbar items.

# 👁️ 5. Visibility

Controls whether an element is visible or hidden.

#### Values:

- visible → normal
- hidden → hidden but space is still reserved
- visibility: hidden;

### ⚠️ Difference from display: none:
```
visibility: hidden → keeps space
display: none → removes element completely
```

# 🌊 6. Overflow

Controls what happens when content overflows its container.

#### Values:


- visible   → default (content spills out)
- hidden    → hides extra content
- scroll    → always shows scrollbars
- auto      → scrollbars only if needed
- overflow:  auto;
