# Assignment 02 – Layout with Viewport, em, rem & calc()

## Objective

The purpose of this assignment is to practice **CSS layout concepts** using different CSS units such as **em, rem, %, and vh**, and to dynamically calculate sizes using the **calc() function**.
It also demonstrates how different CSS units behave when the viewport size or root font size changes.

---

## Project Structure

```
assignment-02
│
├── index.html
├── style.css
└── README.md
```

---

## Layout Description

The layout contains:

* A **Header section**
* A **Body section**
* Two **columns inside the body**
* Multiple **rows inside each column**

### Header

* Uses `#header` ID
* Height: **10vh**
* Background: **lightgray**
* Border: **1px solid black**
* Positioned at the top of the page

### Body

* Uses `#body` ID
* Background: **lightblue**
* Border: **1px solid black**
* Height dynamically calculated using:

```
min-height: calc(100vh - 10vh - 10px);
```

This ensures the body fills the **remaining viewport height after the header**.

---

## Columns

Two columns are placed **next to each other on the same line** using `display: inline-block`.

### Column 1

* ID: `#col-1`
* Width: **30%**
* Contains **4 rows**

### Column 2

* ID: `#col-2`
* Width: **70%**
* Contains **6 rows**

Both columns have:

* Border: **1px solid red**
* Background: **antiquewhite**

---

## Rows

Each row has:

* Border: **1px solid blue**
* Padding: **1em**
* Margin: **0**
* Display: **block**

Rows take the **full width of their parent column**.

---

## CSS Concepts Practiced

This assignment demonstrates:

* **Viewport units (`vh`)**
* **Relative units (`em`)**
* **Percentage widths (`%`)**
* **Dynamic calculations using `calc()`**
* **Inline-block layout**
* **Box sizing**

---

## Experimentation

Try modifying the root font size:

```
html {
  font-size: 16px;
}
```

Then change it to:

```
html {
  font-size: 20px;
}
```

You will observe:

* `em` values scale with the parent font size
* `vh` values change with the browser height
* `calc()` recomputes dimensions dynamically

---

## Preview

Add your assignment screenshot here:

```
![Assignment Preview](./assignment-02.png)
```

---

## Author

**Iqra Shahzadi**
