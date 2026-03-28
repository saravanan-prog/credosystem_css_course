# CSS Grid 

- CSS Grid is a powerful layout system used to create rows and columns easily—perfect for building responsive layouts 🔥

### 🎯 What is CSS Grid?

It lets you design layouts in 2 dimensions:

```
Rows     ➝ horizontal
Columns  ➝ vertical
```

#### 🧱 1. Basic Grid Setup

```
.container {
  display: grid;
}
```

👉 This turns the element into a grid container

### 📏 2. Define Columns

```
.container {
  display: grid;
  grid-template-columns: 100px 100px 100px;
}
```

👉 Creates 3 columns

### 📏 3. Using fr (flexible units)
```
.container {
  grid-template-columns: 1fr 1fr 1fr;
}
```
👉 Equal width columns

### 📦 Example Layout

HTML

```
<div class="container">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
</div>
```
CSS
```
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 10px;
}

.box {
  background: blue;
  color: white;
  padding: 20px;
}
```
### 🔲 4. Rows

```
.container {
  grid-template-rows: 100px 200px;
}
```

### 🔀 5. Span (merge cells)

```
.box1 {
  grid-column: span 2;
}
👉 Box takes 2 columns
```

### 📱 6. Responsive Grid

```
.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
}
👉 Automatically adjusts columns based on screen size
```




# 🧠 Key Properties


| Property                | Purpose             |
| ----------------------- | ------------------- |
| `display: grid`         | Enable grid         |
| `grid-template-columns` | Set columns         |
| `grid-template-rows`    | Set rows            |
| `gap`                   | Space between items |
| `grid-column`           | Span columns        |
| `grid-row`              | Span rows           |
