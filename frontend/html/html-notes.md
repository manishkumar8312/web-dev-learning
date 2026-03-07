# HTML (HyperText Markup Language)

## What is HTML

HTML (**HyperText Markup Language**) is the **standard markup language used to create and structure web pages**.

Web browsers read and interpret HTML code to render web pages visually.

HTML is used for:

* Structuring web page content
* Displaying text and media
* Creating forms to collect user input
* Embedding images, videos, and other media

> Important:
> HTML is **not a programming language**. It is a **markup language used to structure content** on the web.

---

# Basic HTML Document Structure

<p align="center">
  <img src="https://scaler.com/topics/images/paired-and-empty-tags.webp" width="250">
  <img src="https://www.enterrom.com/data/images/item/18200_img_9._Learning_Web_Design_Using_human_body_structure_to_explain_HTML.jpg" width="250">
  <img src="https://blog.rheinwerk-computing.com/hs-fs/hubfs/2422_02_010.png?height=292&name=2422_02_010.png&width=362" width="250">
</p>

Every HTML document follows a **standard structure**.

```html
<!DOCTYPE html>
<html>

<head>
    <title>My Web Page</title>
</head>

<body>

<h1>Hello World</h1>
<p>This is my first webpage</p>

</body>

</html>
```

## Explanation

### DOCTYPE Declaration

```html
<!DOCTYPE html>
```

This declaration tells the browser that the document uses **HTML5**.

---

### `<html>` Tag

```html
<html></html>
```

This is the **root element** that contains the entire HTML document.

---

### `<head>` Section

The head section contains **metadata about the webpage**, such as:

* Page title
* Meta tags
* Links to CSS files
* Scripts

---

### `<body>` Section

The body section contains the **visible content of the webpage**, such as:

* Headings
* Paragraphs
* Images
* Forms
* Tables

---

# HTML Elements

An **HTML element** consists of:

* Opening tag
* Content
* Closing tag

Example:

```html
<p>Hello Manish</p>
```

| Part         | Description |
| ------------ | ----------- |
| `<p>`        | Opening tag |
| Hello Manish | Content     |
| `</p>`       | Closing tag |

---

# HTML Attributes

Attributes provide **additional information about HTML elements**.

Example:

```html
<a href="https://google.com">Visit Google</a>
```

Here, `href` specifies the **destination URL** of the link.

Example:

```html
<img src="image.jpg" alt="sample image">
```

Common HTML attributes:

* `id`
* `class`
* `href`
* `src`
* `alt`
* `style`

---

# Headings

<p align="center">
  <img src="https://www.seobility.net/en/wiki/images/7/7d/H1-H6-headings.png" width="250">
  <img src="https://i.pinimg.com/736x/6a/18/c9/6a18c9959850146f8bf27aa1d652df3a.jpg" width="250">
  <img src="https://images.shiksha.com/mediadata/ugcDocuments/images/wordpressImages/2022_04_HTML-Heading-and-Paragraph-Tags.jpg" width="250">
</p>

HTML provides **six levels of headings**.

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Section Heading</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

Important points:

* `<h1>` is the **most important heading**
* Typically, a page should contain **only one `<h1>` for SEO purposes**

---

# Paragraph and Text Formatting

Paragraph:

```html
<p>This is a paragraph</p>
```

Line break:

```html
<br>
```

Horizontal rule:

```html
<hr>
```

Text formatting tags:

```html
<b>Bold</b>
<strong>Important text</strong>
<i>Italic</i>
<em>Emphasized</em>
<u>Underline</u>
```

---

# Links (Anchor Tag)

Links are created using the `<a>` tag.

```html
<a href="https://google.com">Visit Google</a>
```

To open a link in a new tab:

```html
<a href="https://google.com" target="_blank">
Open Google
</a>
```

---

# Images

<p align="center">
  <img src="https://images.postaffiliatepro.com/images/faq/0xf6e88737b03b8f9.webp" width="250">
  <img src="https://res.cloudinary.com/cloudinary-marketing/images/f_auto%2Cq_auto/v1649719999/Web_Assets/blog/picture-element_224214efe3/picture-element_224214efe3.png?_i=AA" width="250">
  <img src="https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/HTML_images/size.png" width="250">
</p>

Images are displayed using the `<img>` tag.

Example:

```html
<img src="photo.jpg" alt="sample image">
```

Important attributes:

| Attribute | Purpose                            |
| --------- | ---------------------------------- |
| src       | Image file path                    |
| alt       | Alternative text for accessibility |
| width     | Sets image width                   |
| height    | Sets image height                  |

Example:

```html
<img src="image.jpg" width="300">
```

---

# Lists

Lists help organize items in a structured format.

## Ordered List

A numbered list.

```html
<ol>
<li>HTML</li>
<li>CSS</li>
<li>JavaScript</li>
</ol>
```

---

## Unordered List

A bullet-point list.

```html
<ul>
<li>React</li>
<li>Node</li>
<li>MongoDB</li>
</ul>
```

---

# Tables

<p align="center">
  <img src="https://www.ourtutorials.in/html/img/table1.JPG" width="250">
  <img src="https://scaler.com/topics/images/html-tables-with-rowspan.webp" width="250">
  <img src="https://www.tutorialspoint.com/html/images/html_tables.jpg" width="250">
</p>

Tables are used to display data in **rows and columns**.

Example:

```html
<table border="1">

<tr>
<th>Name</th>
<th>Age</th>
</tr>

<tr>
<td>Manish</td>
<td>21</td>
</tr>

</table>
```

Important tags:

| Tag   | Purpose         |
| ----- | --------------- |
| table | Creates a table |
| tr    | Table row       |
| th    | Table header    |
| td    | Table data      |

---

# Forms

<p align="center">
  <img src="https://myschoolhouse.in/admin-panel/assets/upload-images/HTML-Form2521-D-20-12-2024-T-04-37-05am.jpg" width="250">
  <img src="https://img.brainkart.com/imagebk37/R1MVwxg.jpg" width="250">
  <img src="https://www.learntosap.com/html81.jpg" width="250">
</p>

Forms are used to **collect user input**.

Example:

```html
<form>

<label>Name</label>
<input type="text">

<label>Password</label>
<input type="password">

<input type="submit">

</form>
```

Common input types:

* text
* password
* email
* number
* radio
* checkbox
* submit

---

# Semantic HTML

<p align="center">
  <img src="https://www.w3schools.com/html/img_sem_elements.gif" width="250">
</p>

Semantic HTML elements describe the **meaning of the content**.

Examples:

```html
<header></header>
<nav></nav>
<section></section>
<article></article>
<footer></footer>
```

Benefits:

* Improves SEO
* Enhances accessibility
* Makes code easier to read and maintain

---

# Block vs Inline Elements

## Block Elements

Block elements start on a **new line**.

Examples:

* div
* p
* h1
* section

Example:

```html
<div>This is a block element</div>
```

---

## Inline Elements

Inline elements remain **within the same line**.

Examples:

* span
* a
* img
* strong

Example:

```html
<span>Hello</span>
```

---

# div vs span

| div                          | span                                    |
| ---------------------------- | --------------------------------------- |
| Block element                | Inline element                          |
| Used for layout and grouping | Used for styling small portions of text |

Example:

```html
<div>
<p>Hello</p>
</div>
```

```html
<span>Important text</span>
```

---

# HTML5 Features

HTML5 introduced several modern web features.

Examples:

* Semantic elements
* Audio and video support
* Canvas for graphics
* Local storage
* Geolocation APIs

Example:

```html
<video controls>
<source src="video.mp4">
</video>
```

---

# Important HTML Interview Questions

### What is HTML?

HTML is a markup language used to structure and display content on web pages.

---

### What is the difference between HTML and HTML5?

HTML5 introduced several new features, including:

* Semantic elements
* Audio and video support
* Canvas API
* Local storage

---

### What are semantic tags?

Semantic tags clearly describe the **purpose of the content**.

Examples:

* header
* nav
* article
* section
* footer

---

### Difference between id and class

| id                        | class                      |
| ------------------------- | -------------------------- |
| Unique identifier         | Can be reused              |
| Used for a single element | Used for multiple elements |

Example:

```html
<div id="header"></div>

<div class="box"></div>
```
--- 
# Useful Resources

**MDN Web Docs**
[https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

**W3Schools HTML Tutorial**
[https://www.w3schools.com/html/](https://www.w3schools.com/html/)

**HTML Validator**
[https://validator.w3.org](https://validator.w3.org)

**Can I Use (Browser Compatibility)**
[https://caniuse.com](https://caniuse.com)

**ARIA Authoring Practices**
[https://www.w3.org/WAI/ARIA/apg/](https://www.w3.org/WAI/ARIA/apg/)
