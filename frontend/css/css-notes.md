# CSS (Cascading Style Sheets)

## Introduction

CSS (**Cascading Style Sheets**) is a stylesheet language used to describe the presentation and layout of HTML documents. It controls how elements are displayed on screen, paper, or other media.

CSS allows developers to separate **content (HTML)** from **presentation (design)**, making web pages more maintainable, reusable, and visually appealing.

CSS can control:

* Layout
* Colors
* Fonts
* Spacing
* Animations
* Responsive design

---

# Ways to Add CSS

There are three main ways to apply CSS to HTML.

## 1. Inline CSS

Inline CSS is written directly inside an HTML element using the `style` attribute.

```html
<p style="color: blue; font-size: 18px;">Hello World</p>
```

Advantages:

* Quick styling
* Useful for testing

Disadvantages:

* Not reusable
* Hard to maintain
* Poor practice for large projects

---

## 2. Internal CSS

Internal CSS is defined inside the `<style>` tag within the `<head>` section of an HTML document.

```html
<head>
    <style>
        p {
            color: red;
            font-size: 20px;
        }
    </style>
</head>
```

Advantages:

* Useful for styling a single page
* Better organization than inline CSS

Disadvantages:

* Not reusable across multiple pages

---

## 3. External CSS

External CSS is written in a separate `.css` file and linked to the HTML file.

```html
<link rel="stylesheet" href="styles.css">
```

Example CSS file:

```css
p {
    color: green;
    font-size: 18px;
}
```

Advantages:

* Reusable across multiple pages
* Cleaner HTML
* Best practice for real projects

---

# CSS Syntax

CSS consists of selectors and declaration blocks.

```css
selector {
    property: value;
}
```

Example:

```css
h1 {
    color: blue;
    font-size: 32px;
}
```

Components:

* **Selector** → HTML element to style
* **Property** → Style attribute
* **Value** → Property value

---

# CSS Selectors

Selectors are used to target HTML elements.

## Element Selector

Targets all elements of a specific type.

```css
p {
    color: black;
}
```

---

## Class Selector

Targets elements with a specific class.

```css
.note {
    color: blue;
}
```

HTML:

```html
<p class="note">Important text</p>
```

---

## ID Selector

Targets a specific element using an ID.

```css
#header {
    background-color: gray;
}
```

HTML:

```html
<div id="header"></div>
```

IDs should be unique in a page.

---

## Universal Selector

Targets all elements.

```css
* {
    margin: 0;
    padding: 0;
}
```

---

## Group Selector

Applies the same styles to multiple elements.

```css
h1, h2, h3 {
    font-family: Arial;
}
```

---

## Descendant Selector

Targets elements inside another element.

```css
div p {
    color: red;
}
```

---

## Child Selector

Targets direct children only.

```css
div > p {
    color: blue;
}
```

---

# CSS Colors

CSS supports multiple ways to define colors.

## Named Colors

```css
color: red;
```

---

## HEX

```css
color: #ff0000;
```

---

## RGB

```css
color: rgb(255, 0, 0);
```

---

## RGBA

```css
color: rgba(255, 0, 0, 0.5);
```

---

# CSS Box Model

Every HTML element is treated as a rectangular box.

The box model consists of:

1. Content
2. Padding
3. Border
4. Margin

```
Margin
  Border
    Padding
      Content
```

Example:

```css
div {
    width: 200px;
    padding: 20px;
    border: 5px solid black;
    margin: 10px;
}
```

---

# Margin

Controls the outer spacing of an element.

```css
margin: 20px;
```

Individual sides:

```css
margin-top: 10px;
margin-right: 20px;
margin-bottom: 10px;
margin-left: 20px;
```

---

# Padding

Controls spacing inside the element between content and border.

```css
padding: 15px;
```

---

# Borders

Defines the border around elements.

```css
border: 2px solid black;
```

Properties:

* `border-width`
* `border-style`
* `border-color`

Example:

```css
border: 1px dashed red;
```

---

# CSS Display Property

Controls how elements are displayed.

Common values:

### Block

```css
display: block;
```

Examples:

* div
* p
* h1

Block elements take the full width.

---

### Inline

```css
display: inline;
```

Examples:

* span
* a
* strong

Inline elements do not start on a new line.

---

### Inline-block

```css
display: inline-block;
```

Allows width and height while staying inline.

---

### None

```css
display: none;
```

Element becomes invisible and takes no space.

---

# Positioning

Controls element placement.

## Static

Default positioning.

```css
position: static;
```

---

## Relative

Position relative to itself.

```css
position: relative;
top: 10px;
left: 20px;
```

---

## Absolute

Position relative to the nearest positioned ancestor.

```css
position: absolute;
top: 0;
right: 0;
```

---

## Fixed

Position relative to the viewport.

```css
position: fixed;
bottom: 0;
right: 0;
```

---

# Flexbox

Flexbox is a layout module for designing flexible layouts.

Container:

```css
.container {
    display: flex;
}
```

Important properties:

```
flex-direction
justify-content
align-items
flex-wrap
gap
```

Example:

```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
}
```

---

# CSS Grid

CSS Grid is used for two-dimensional layouts.

```css
.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
}
```

Example:

```css
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}
```

---

# Responsive Design

Responsive design ensures that websites work across all screen sizes.

## Media Queries

```css
@media (max-width: 768px) {
    body {
        background-color: lightgray;
    }
}
```

Example:

```css
@media (max-width: 600px) {
    .container {
        flex-direction: column;
    }
}
```

---

# CSS Units

Common units used in CSS.

## Absolute Units

* px
* cm
* mm

Example:

```css
font-size: 16px;
```

---

## Relative Units

* %
* em
* rem
* vw
* vh

Example:

```css
font-size: 2rem;
width: 50%;
```

---

# CSS Transitions

Transitions allow smooth changes between CSS property values.

```css
button {
    transition: background 0.3s;
}

button:hover {
    background: blue;
}
```

---

# CSS Animations

Animations allow complex visual effects.

```css
@keyframes slide {
    from {
        transform: translateX(0);
    }
    to {
        transform: translateX(200px);
    }
}

.box {
    animation: slide 2s infinite;
}
```

---

# Best Practices

* Use **external CSS files**
* Use **class selectors instead of IDs**
* Maintain **consistent naming conventions**
* Keep CSS **modular and reusable**
* Avoid excessive nesting
* Use **Flexbox and Grid** for layouts
* Write **responsive styles**

---

# Conclusion

CSS is a fundamental technology of web development that controls the visual presentation of web pages. By mastering selectors, layout systems like Flexbox and Grid, and responsive design techniques, developers can create modern and responsive web interfaces.
