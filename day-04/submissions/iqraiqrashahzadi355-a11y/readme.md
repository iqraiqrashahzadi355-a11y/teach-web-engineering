# Assignment 01 – CSS Box Model & Display Property

## Objective

The objective of this assignment is to practice using the **CSS Box Model**, understand the **display property**, and apply **multiple CSS classes using the BEM (Block Element Modifier) naming convention** to create a structured layout.

---

## Project Structure

```
assignment-01
│
├── index.html
└── style.css
```

---

## HTML Structure

The HTML file contains **four paragraph (`<p>`) elements**.
Each paragraph contains **three span (`<span>`) elements**.

Each paragraph uses:

* A **base class:** `box`
* A **modifier class** to define the width.

### Paragraph Classes

| Paragraph | Classes                |
| --------- | ---------------------- |
| First     | `box box--small`       |
| Second    | `box box--medium`      |
| Third     | `box box--large`       |
| Fourth    | `box box--extra-large` |

Each paragraph contains three spans:

```
<span>Span 1</span>
<span>Span 2</span>
<span>Span 3</span>
```

---

## CSS Styling

### Paragraph Styling

The paragraph elements are styled using the **CSS Box Model** and the **display property**.

* Border: `2px solid black`
* Display: `inline-block`
* Alignment: side-by-side horizontally

### Width Modifiers

The modifier classes control the width of each box.

| Class               | Width |
| ------------------- | ----- |
| `.box--small`       | 100px |
| `.box--medium`      | 200px |
| `.box--large`       | 300px |
| `.box--extra-large` | 400px |

---

### Span Styling

The span elements are styled to behave like block elements.

Properties applied:

* Border: `1px solid red`
* Display: `block`
* Margin: `5px`
* Padding: `5px`

Because of `display: block`, the spans **stack vertically inside each paragraph**.

---

## Expected Output

The page displays:

* **Four black bordered boxes** arranged horizontally.
* Each box has **different widths** (100px, 200px, 300px, 400px).
* Inside each box are **three red bordered spans** stacked vertically.

Visual structure:

```
[ Box 100px ]   [ Box 200px ]   [ Box 300px ]   [ Box 400px ]

Span 1          Span 1          Span 1          Span 1
Span 2          Span 2          Span 2          Span 2
Span 3          Span 3          Span 3          Span 3
```

---

## Concepts Practiced

* CSS Box Model
* `display` property
* Inline vs Block elements
* `inline-block`
* BEM naming convention
* Margin and Padding

---

## Author

Iqra Shahzadi
