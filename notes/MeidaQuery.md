# Media queries

- Media queries — these are used to make your website responsive for different screen sizes 📱💻

### ✅ What are Media Queries?

#### Media queries let you apply CSS based on:

- Screen width
- Device type
- Resolution
- Orientation (portrait/landscape)

✅ Basic Syntax

```
@media (condition) {
  /* CSS rules */
}
```

## 📱 Common Examples
#### 1. For mobile screens

```
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

👉 Applies when screen width is 600px or less

## 2. For tablets

```
@media (min-width: 601px) and (max-width: 1024px) {
  body {
    background-color: lightgreen;
  }
}
```

### 3. For desktops
```
@media (min-width: 1025px) {
  body {
    background-color: white;
  }
}
```

## 💡 Mobile-first approach (best practice)

- Start with mobile styles, then scale up:

/* Default (mobile) */

```
.container {
  padding: 10px;
}
```
/* Tablet */
```
@media (min-width: 768px) {
  .container {
    padding: 20px;
  }
}
```

/* Desktop */

```
@media (min-width: 1200px) {
  .container {
    padding: 40px;
  }
}
```

## 🔄 Orientation example
#### 1. portrait
```
@media (orientation: portrait) {
  body {
    background-color: lightblue;
  }
}
```
#### 2. landscape
```
@media (orientation: landscape) {
  body {
    background-color: yellow;
  }
}
```
# 🎯 Real-world example (responsive layout)
```
.box {
  width: 100%;
}

@media (min-width: 768px) {
  .box {
    width: 50%;
  }
}
```

```
@media (min-width: 1200px) {
  .box {
    width: 25%;
  }
}
```