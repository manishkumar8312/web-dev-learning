# HTML (HyperText Markup Language)

## What is HTML

HTML (**HyperText Markup Language**) ek **standard markup language** hai jo web pages ka **structure define** karti hai.

Browser HTML ko parse karke webpage render karta hai.

HTML ka use hota hai:

* Web page structure banane ke liye
* Content display karne ke liye
* Forms create karne ke liye
* Images aur media embed karne ke liye

Important point:

> HTML **programming language nahi hai**, balki **markup language** hai.

---

## Basic HTML Document Structure

<p align="center">
  <img src="https://scaler.com/topics/images/paired-and-empty-tags.webp" width="250">
  <img src="https://www.enterrom.com/data/images/item/18200_img_9._Learning_Web_Design_Using_human_body_structure_to_explain_HTML.jpg" width="250">
  <img src="https://blog.rheinwerk-computing.com/hs-fs/hubfs/2422_02_010.png?height=292&name=2422_02_010.png&width=362" width="250">
</p>
Every HTML page ek **standard structure follow karta hai**.

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

### Explanation

**DOCTYPE**

```html
<!DOCTYPE html>
```

Browser ko batata hai ki document **HTML5 standard** follow karta hai.

---

**html tag**

```html
<html></html>
```

Yeh **root element** hai jo poore document ko wrap karta hai.

---

**head section**

Head section me **metadata** hota hai.

Examples:

* title
* meta tags
* CSS
* scripts

---

**body section**

Body me **visible content** hota hai.

Examples:

* headings
* text
* images
* forms
* tables

---

# HTML Elements

HTML element = **start tag + content + end tag**

Example:

```html
<p>Hello Manish</p>
```

| Part         | Description |
| ------------ | ----------- |
| `<p>`        | start tag   |
| Hello Manish | content     |
| `</p>`       | end tag     |

---

# HTML Attributes

Attributes **additional information** provide karte hain.

Example:

```html
<a href="https://google.com">Visit Google</a>
```

`href` attribute link destination define karta hai.

Example:

```html
<img src="image.jpg" alt="sample image">
```

Common attributes:

* id
* class
* href
* src
* alt
* style

---

# Headings

<p align="center">
  <img src="https://www.seobility.net/en/wiki/images/7/7d/H1-H6-headings.png" width="250">
  <img src="https://i.pinimg.com/736x/6a/18/c9/6a18c9959850146f8bf27aa1d652df3a.jpg" width="250">
  <img src="https://images.shiksha.com/mediadata/ugcDocuments/images/wordpressImages/2022_04_HTML-Heading-and-Paragraph-Tags.jpg" width="250">
</p>

HTML me **6 levels ke headings** hote hain.

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Section Heading</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

Important:

* **h1 sabse important heading hoti hai**
* SEO ke liye **page me usually ek hi h1 hota hai**

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

Horizontal line:

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

Links create karne ke liye `<a>` tag use hota hai.

```html
<a href="https://google.com">Visit Google</a>
```

New tab me open karne ke liye:

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

Images display karne ke liye `<img>` tag use hota hai.

Example:

```html
<img src="photo.jpg" alt="sample image">
```

Important attributes:

| Attribute | Purpose              |
| --------- | -------------------- |
| src       | image path           |
| alt       | alternative text     |
| width     | width set karta hai  |
| height    | height set karta hai |

Example:

```html
<img src="image.jpg" width="300">
```

---

# Lists

Lists items ko structured format me show karti hain.

## Ordered List

Numbered list.

```html
<ol>
<li>HTML</li>
<li>CSS</li>
<li>JavaScript</li>
</ol>
```

---

## Unordered List

Bullet list.

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
Tables data ko **rows aur columns** me display karti hain.

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

| Tag   | Purpose                |
| ----- | ---------------------- |
| table | table create karta hai |
| tr    | table row              |
| th    | table header           |
| td    | table data             |

---

# Forms
<p align="center">
  <img src="https://myschoolhouse.in/admin-panel/assets/upload-images/HTML-Form2521-D-20-12-2024-T-04-37-05am.jpg" width="250">
  <img src="https://img.brainkart.com/imagebk37/R1MVwxg.jpg" width="250">
  <img src="https://www.learntosap.com/html81.jpg" width="250">
</p>

Forms user se **data collect karne** ke liye use hote hain.

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


Semantic tags **content ka meaning define karte hain**.

Examples:

```html
<header></header>
<nav></nav>
<section></section>
<article></article>
<footer></footer>
```

Benefits:

* SEO improve hota hai
* Accessibility improve hoti hai
* Code readable hota hai

---

# Block vs Inline Elements

## Block Elements

New line se start hote hain.

Examples:

* div
* p
* h1
* section

Example:

```html
<div>This is block element</div>
```

---

## Inline Elements

Same line me rehte hain.

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

| div            | span                 |
| -------------- | -------------------- |
| block element  | inline element       |
| layout ke liye | text styling ke liye |

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

HTML5 ne modern web development ke liye naye features introduce kiye.

Examples:

* semantic elements
* audio
* video
* canvas
* local storage
* geolocation

Example:

```html
<video controls>
<source src="video.mp4">
</video>
```

---

# Most Important HTML Interview Questions

### What is HTML?

HTML ek markup language hai jo web pages ka structure define karti hai.

---

### What is the difference between HTML and HTML5?

HTML5 me naye features add hue:

* semantic tags
* audio/video support
* canvas
* local storage

---

### What are semantic tags?

Semantic tags elements ka **meaning describe karte hain**.

Examples:

* header
* nav
* article
* section
* footer

---

### Difference between id and class

| id         | class             |
| ---------- | ----------------- |
| unique     | multiple elements |
| ek element | multiple elements |

Example:

```html
<div id="header"></div>

<div class="box"></div>
```

---

# Most Important HTML Tags

Common tags:

* html
* head
* body
* h1-h6
* p
* a
* img
* ul
* ol
* table
* form
* input
* div
* span

Useful Resources

MDN Web Docs: https://developer.mozilla.org/en-US/docs/Web/HTMLW3Schools 
HTML: https://www.w3schools.com/html/HTML 
Validator: https://validator.w3.org
Can I Use: https://caniuse.comARIA 
Authoring Practices: https://www.w3.org/WAI/ARIA/apg/