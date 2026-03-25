## CSS Grid — simple explanation

 - CSS Grid is a layout system that lets you design web pages in rows and columns
 - (like a table, but way more powerful).

#### 🔹 Basic idea

You have:

- Grid container → parent element
- Grid items → children inside it

🔹 Step 1: Create a grid
```
    .container {
        display: grid;
    }
```
🔹 Step 2: Define columns & rows
```   
.container {
    display: grid; 
    grid-template-columns: 1fr 1fr 1fr;  /* 3 equal columns and fr means fraction of unit */
    grid-template-rows: auto auto;      /* 2 rows */
}
```

👉 fr = fraction of available space

#### 🔹 Example

```
<div class="container">
  <div>1</div>
  <div>2</div>
  <div>3</div>
  <div>4</div>
</div>
```

```
.container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 10px;
}
```
```        
👉 Output:

1   2
3   4

```


##  Important properties
#### 1. Columns
```
    grid-template-columns: 200px 1fr 2fr;
```
#### 2. Rows
```
    grid-template-rows: 100px auto;
```
#### 3. Gap (spacing)
```
    gap: 10px;
```
#### 4. Position items
```
.item {
  grid-column: 1 / 3; /* spans 2 columns */
}
```
🔹 Real-world use

### CSS Grid is great for:

- Page layouts (header, sidebar, content)
- Dashboards
- Image galleries

### Flexbox vs Grid
```
Flexbox  → 1D (row or column)
Grid     → 2D (row and column)
```