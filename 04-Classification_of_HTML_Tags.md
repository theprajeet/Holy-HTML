# Classification of HTML Tags

## **HTML Tags**

HTML tags are used to define the structure and content of a web page. Based on whether they require a closing tag or not, HTML tags are classified into **two types**:

1. **Paired Tags (Container Tags)**
2. **Unpaired Tags (Empty Tags)**

```jsx
HTML TAGS
│
├── 1. Paired Tags (Opening Tag & Closing Tag)
│   │
│   ├── A. Heading Tags
│   │   ├── <h1></h1>
│   │   ├── <h2></h2>
│   │   ├── <h3></h3>
│   │   ├── <h4></h4>
│   │   ├── <h5></h5>
│   │   └── <h6></h6>
│   │
│   ├── B. Formatting Tags
│   │   ├── <b></b>            (Bold)
│   │   ├── <strong></strong>  (Strong)
│   │   ├── <i></i>            (Italic)
│   │   ├── <em></em>          (Emphasis)
│   │   ├── <u></u>            (Underline)
│   │   ├── <strike></strike>  (Strike)
│   │   ├── <sup></sup>        (Superscript)
│   │   ├── <sub></sub>        (Subscript)
│   │   └── <mark></mark>      (Highlight)
│   │
│   └── C. Other Tags
│       ├── <p></p>            (Paragraph)
│       ├── <pre></pre>        (Preformatted Text)
│       ├── <div></div>        (Division)
│       ├── <span></span>      (Inline Container)
│       ├── <a></a>            (Anchor/Hyperlink)
│       ├── <table></table>    (Table)
│       ├── <tr></tr>          (Table Row)
│       ├── <th></th>          (Table Heading)
│       ├── <td></td>          (Table Data)
│       ├── <ol></ol>          (Ordered List)
│       ├── <ul></ul>          (Unordered List)
│       ├── <li></li>          (List Item)
│       ├── <dl></dl>          (Description List)
│       ├── <dt></dt>          (Description Term)
│       ├── <dd></dd>          (Description Description)
│       ├── <form></form>      (Form)
│       ├── <label></label>    (Label)
│       ├── <textarea></textarea>
│       ├── <button></button>
│       ├── <select></select>
│       ├── <option></option>
│       ├── <audio></audio>
│       ├── <video></video>
│       ├── <iframe></iframe>
│       ├── <header></header>
│       ├── <nav></nav>
│       ├── <main></main>
│       ├── <section></section>
│       ├── <article></article>
│       ├── <aside></aside>
│       └── <footer></footer>
│
└── 2. Unpaired Tags (Self-Closing Tags)
    ├── <br>      (Line Break)
    ├── <hr>      (Horizontal Rule)
    ├── <img>     (Image)
    ├── <input>   (Input Field)
    ├── <meta>    (Metadata)
    ├── <link>    (External Resource)
    ├── <source>  (Media Source)
    └── <base>    (Base URL)
```

---

### **1. Paired Tags (Container Tags)**

Paired tags consist of an **opening tag** and a **closing tag**. The content is placed between these two tags.

**Syntax:**

```html
<tagname>
    Content
</tagname>
```

Example:

```html
<p>This is a paragraph.</p>
```

Paired tags can be further classified into:

- Heading Tags
- Formatting Tags
- Other Tags

---

### **A. Heading Tags**

Heading tags are used to define headings and subheadings on a webpage. HTML provides six levels of headings, from `<h1>` to `<h6>`.

- `<h1>` – Largest and most important heading.
- `<h2>` – Second largest heading.
- `<h3>` – Third largest heading.
- `<h4>` – Fourth largest heading.
- `<h5>` – Fifth largest heading.
- `<h6>` – Smallest heading.

**Example:**

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Section Heading</h3>
<h4>Topic Heading</h4>
<h5>Small Heading</h5>
<h6>Smallest Heading</h6>
```

---

### **B. Formatting Tags**

Formatting tags are used to format or emphasise text. Most formatting tags are **inline elements**, meaning they appear side by side and do not start on a new line.

#### **`<b>` (Bold)**

Displays text in bold.

**Example:**

```html
<b>Bold Text</b>
```

#### **`<strong>` (Strong)**

Displays text in bold and indicates that the text is important.

`<strong>` is considered the semantic alternative to `<b>`.

**Example:**

```html
<strong>Important Text</strong>
```

#### **`<i>` (Italic)**

Displays text in italic.

**Example:**

```html
<i>Italic Text</i>
```

#### **`<em>` (Emphasis)**

Displays emphasized text, which is usually shown in italics.

`<em>` is the semantic alternative to `<i>`.

**Example:**

```html
<em>Emphasized Text</em>
```

#### **`<u>` (Underline)**

Underlines the text.

**Example:**

```html
<u>Underlined Text</u>
```

#### **`<strike>` (Strike)**

Displays text with a line through it.

**Example:**

```html
<strike>Old Price</strike>
```

Output: ~~Old Price~~

#### **`<sup>` (Superscript)**

Displays text slightly above the normal line.

**Example:**

```html
A<sup>+</sup>
```

#### **`<sub>` (Subscript)**

Displays text slightly below the normal line.

**Example:**

```html
H<sub>2</sub>O
```

#### **`<mark>` (Mark)**

Highlights the text.

**Example:**

```html
<mark>Highlighted Text</mark>
```

---

### **C. Other Tags**

These tags are commonly used to organise and display content on a webpage.

#### **`<p>` (Paragraph Tag)**

The paragraph tag is used to create paragraphs. It automatically removes extra spaces and line breaks, displaying the text as a normal paragraph.

**Example:**

```html
<p>
This is the first line.
This is the second line.
</p>
```

**Output:**

This is the first line. This is the second line.

#### **`<pre>` (Preformatted Tag)**

The preformatted tag displays text exactly as it is written in the HTML source code. It preserves spaces, tabs, and line breaks.

**Example:**

```html
<pre>
This is the first line.
    This line has spaces.
        This line is indented.
</pre>
```

**Output:**

```
This is the first line.
    This line has spaces.
        This line is indented.
```

#### **`<div>` (Division Tag)**

The `<div>` tag is a block-level container used to group HTML elements together. It is commonly used for creating sections of a webpage and applying CSS styles.

**Example:**

```html
<div>
    <h2>About Us</h2>
    <p>Welcome to our website.</p>
</div>
```

---

### **2. Unpaired Tags (Empty Tags)**

Unpaired tags contain only an opening tag and do not require a closing tag.

### **`<br>` (Line Break Tag)**

The `<br>` tag inserts a line break and moves the following content to the next line.

**Example:**

```html
Hello<br>
Welcome to HTML.
```

**Output:**

```
Hello
Welcome to HTML.
```

### **`<hr>` (Horizontal Rule Tag)**

The `<hr>` tag inserts a horizontal line, which is commonly used to separate sections of content.

**Example:**

```html
<p>Chapter 1</p>
<hr>
<p>Chapter 2</p>
```

### **`<img>` (Image Tag)**

The `<img>` tag is used to display images on a webpage. It is an empty tag and requires the `src` attribute to specify the image path and the `alt` attribute to provide alternative text.

**Syntax:**

```html
<img src="image.jpg" alt="Image Description">
```

**Example:**

```html
<img src="nature.jpg" alt="Nature Image" width="300" height="200">
```

---