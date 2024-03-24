# CSS NOTES

![CSS logo](https://github.com/itsme-rash522/frontend-freaks/assets/127365805/a38212aa-5f78-4b0a-a7fd-314cba7d6cb2)

## [CSS Basic](#css-basic)

## [CSS Flexbox](#css-flexbox)

## [CSS Grid](#css-grid)

---

<h1 id="css-basic">CSS Basic</h1>

## Adding CSS to HTML (3 Methods & Precedence)

```html
<!-- Inline CSS -->
  <h1 style="color: red;">Hello World</h1>

<!-- Internal CSS -->
<head>
    <style>
        h1 {
            color: red;
        }
    </style>
</head>

<!-- External CSS -->
<head>
    <link rel="stylesheet" href="style.css">
</head>
```

## Understanding CSS Syntax

```css
selector {
    property: value;
}
```

## CSS Selectors and Specificity

```css
/* Element selector */
h1 {
    color: red;
}

/* Class selector */
.heading {
    color: blue;
}

/* Id selector */
#title {
    color: green;
}

/* Specificity example */
.heading#title {
    color: yellow;
}
```

## Working with CSS Fonts

```css
/* Font family */
body {
    font-family: Arial, sans-serif;
}

/* Font size */
h1 {
    font-size: 3rem;
}

/* Font weight */
h2 {
    font-weight: bold;
}
```

## Using CSS Color Effectively

```css
/* Hex code */
h1 {
    color: #ff0000;
}

/* RGB */
.heading {
    color: rgb(0, 255, 0);
}

/* HSL */
#title {
    color: hsl(240, 100%, 50%);
}
```

## CSS Backgrounds and Gradients

```css
/* Background color */
body {
    background-color: #fff;
}

/* Background image */
.container {
    background-image: url(bg.jpg);
}

/* Linear gradient */
.heading {
    background: linear-gradient(to bottom, #ff0000, #0000ff);
}

/* Radial gradient */
.title {
    background: radial-gradient(circle, #ff0000, #0000ff);
}
```

## Creating CSS Borders and Shapes

```css
/* Border */
.container {
    border: 1px solid black;
}

/* Border radius */
.box {
    border-radius: 10px;
}

/* Box shadow */
.heading {
    box-shadow: 5px 5px 10px #888888;
}

/* Triangle */
.triangle {
    width: 0;
    height: 0;
    border-top: 50px solid red;
    border-right: 50px solid transparent;
}

/* Circle */
.circle {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background-color: red;
}
```

## Understanding the CSS Box Model

```css
/* Content box */
.container {
    width: 300px;
    height: 200px;
}

/* Padding box */
.container {
    padding: 10px;
}

/* Border box */
.container {
    border: 1px solid black;
}

/* Margin box */
.container {
    margin: 10px;
}
```

## Formatting CSS Text

```css
/* Text alignment */
h1 {
    text-align: center;
}

/* Text decoration */
a {
    text-decoration: none;
}

/* Text transformation */
.heading {
    text-transform: uppercase;
}

/* Letter spacing */
.title {
    letter-spacing: 2px;
}

/* Line height */
p {
    line-height: 1.5;
}
```

## Creating CSS Links

```css
/* unvisited link */
a:link {
    color: blue;
}

/* visited link */
a:visited {
    color: purple;
}

/* mouse over link */
a:hover {
    color: red;
}

/* selected link */
a:active {
    color: green;
}
```

## Using CSS Display Property

```css
/* block-level element */
div {
    display: block;
}

/* inline-level element */
span {
    display: inline;
}

/* inline-block element */
img {
    display: inline-block;
}
```

## Positioning Elements with CSS

```css
/* static positioning (default) */
div {
    position: static;
}

/* relative positioning */
div {
    position: relative;
    top: 10px;
    left: 20px;
}

/* absolute positioning */
div {
    position: absolute;
    top: 10px;
    left: 20px;
}

/* fixed positioning */
div {
    position: fixed;
    top: 10px;
    left: 20px;
}

/* sticky */
div {
    position: sticky;
}
```

## CSS Media Queries

```css
/* Small screens (mobile devices) */
@media only screen and (max-width: 767px) {
    /* Styles go here */
}

/* Medium screens (tablets) */
@media only screen and (min-width: 768px) and (max-width: 1023px) {
    /* Styles go here */
}

/* Large screens (desktops) */
@media only screen and (min-width: 1024px) and (max-width: 1279px) {
    /* Styles go here */
}

/* Extra large screens (large desktops) */
@media only screen and (min-width: 1280px) {
    /* Styles go here */
}
```

<br>

---

<h1 id="css-flexbox">CSS Flexbox</h1>

## Display Property

```css
/* Set the container to a flexbox */
.container {
    display: flex;
}
```

## Flex Direction Property

```css
/* Set the main axis direction */
.container {
    flex-direction: row | row-reverse | column | column-reverse;
}
```

## Flex Wrap Property

```css
/* Allow items to wrap */
.container {
    flex-wrap: nowrap | wrap | wrap-reverse;
}
```

## Flex Flow Property

```css
/* Combine flex-direction and flex-wrap */
.container {
    flex-flow: row wrap;
}
```

## Justify Content Property

```css
/* Align items along the main axis */
.container {
    justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
}
```

## Align Items Property

```css
/* Align items along the cross axis */
.container {
    align-items: stretch | flex-start | flex-end | center | baseline;
}
```

## Align Content Property

```css
/* Align wrapped lines along the cross axis */
.container {
    align-content: flex-start | flex-end | center | space-between | space-around | stretch;
}
```

## Gap Property

```css
/* Set the gap between flex items */
.container {
    gap: 10px;
}
```

## Order Property

```css
/* Change the order of flex items */
.item {
    order: 2;
}
```

## Flex Grow Property

```css
.item {
    flex-grow: 1;
}
```

## Flex Shrink Property

```css
/* Allow an item to shrink to fit available space */
.item {
    flex-shrink: 1;
}
```

## Flex Basis Property

```css
/* Set the initial main size of an item */
.item {
    flex-basis: auto | 0 | 50%;
}
```

## Flex Property

```css
.item {
     flex: 3 5 500px; /* shorthand for flex-grow flex shrink flex-basis */
}
```

## Align Self Property

```css
.item {
    align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```

---

<h1 id="css-grid">CSS Grid</h1>

## Grid Template Columns

```css
/* Defines the columns of the grid */
.container {
    gird-template-columns: 100px 100px 100px;
}
```

## Grid Template Rows

```css
/* Defines the rows of the grid */
.container {
    grid-template-rows: 100px 100px 100px;
}
```

## Grid Template Areas

```css
/* Defines the areas of the grid */
.container {
    grid-template-areas:
      "header header header"
      "content content sidebar"
      "footer footer footer"
}
```

## Gap

```css
/* Specifies the size of the gap between grid items */
.container {
    gap:10px;
}
```

## Justify Items

```css
/* Aligns items along the inline (row) axis */
.container {
    justify-items: center;
}
```

## Align Items

```css
/* Align items along the block (column) axis */
.container {
    align-items: center;
}
```

## Justify Content

```css
/* Aligns the grid along the inline (row) axis */
.container {
    justify-content: center;
}
```

## Align Content

```css
/* Aligns the grid along the block (column) axis */
.container {
    align-content: center;
}
```

## Grid Column Start

```css
/* Specifies the start position of a grid item along the inline (row) axis */
.item {
    grid-column-start: 1;
}
```

## Grid Column End

```css
/* Specifies the end position of a grid item along the inline (row) axis */
.item {
    grid-column-end: 3;
}
```

## Grid Row Start

```css
/* Specifies the start position of a grid item along the block (column) axis */
.item {
    grid-row-start: 1;
}
```

## Grid Row End

```css
/* Specifies the end position of a grid item along the block (column) axis */
.item {
    grid-row-end: 1;
}
```

## Grid Area

```css
/* Specifies both the start and end positions of a grid item */
.item {
    grid-area: 1 / 1 / 3 / 3; /* start-row / start-column / end-row / end-column */
}
```

## Justify Self

```css
/* Aligns a grid item along the inline (row) axis. */
  .item {
    justify-self: center;
  }
```

## Align Self

```css
/* Aligns a grid item along the block (column) axis. */
  .item {
    align-self: center;
  }
```
