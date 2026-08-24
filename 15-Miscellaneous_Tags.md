# Miscellaneous Tags

## HTML Code Tag

The **`<code>`** tag is a semantic HTML tag that's used for displaying code snippets. It can be used both inline and within a block-level element like **`<pre>`**.

- **Semantic Meaning**: Provides semantic value to the enclosed code.
- **Readability**: This makes it easier for both browsers and developers to understand that the text is code.
- **Styling**: Easier to style and highlight with CSS or JavaScript libraries like Prism.

The most straightforward way to use the **`<code>`** tag is inline for short code snippets:

```html
<code>Your code here</code>
```

#### **Using `<code>` with `<pre>`**

For multiline code snippets, it's common to combine the **`<code>`** tag with the **`<pre>`** tag:

```html
<pre><code>Your multiline code here</code></pre>
```

---

## HML Canvas Tag

The **`<canvas>`** element serves as a container for graphics, which can be rendered via scripting. Essentially, it offers a drawing area for visual content.

#### Characteristics

- **Graphics:** For drawing shapes, graphs, and other visual representations.
- **Dynamic Content:** To dynamically update visual elements.
- **Interactivity:** Though this involves JavaScript, the canvas element is the foundation for interactive graphical content.

Here's how you can define a simple **`<canvas>`** element:

```html
<canvas id="myCanvas" width="200" height="100"></canvas>
```

#### **Attributes of Canvas**

While the **`<canvas>`** element is simple, it does have a couple of important attributes:

- **width:** Specifies the width of the canvas.
- **height:** Specifies the height of the canvas.

#### **Styling with CSS**

You can also style the **`<canvas>`** element with CSS. For example, to add a border:

```html
canvas {
    border: 1px solid black;
}
```

---

## HTML Entities

HTML entities are used to represent special characters in a format that the browser can understand. They start with an ampersand (**`&`**) and end with a semicolon (**`;`**).

#### **Why Use HTML Entities?**

Here are some reasons:

- **Reserved Characters**: Characters like **`<`**, **`>`**, and **`&`** are reserved in HTML.
- **Special Symbols**: For symbols like **`©`**, **`®`**, or mathematical symbols.
- **Non-Breaking Spaces**: To create white spaces that won't break into a new line.

### **Common HTML Entities**

```jsx
&lt;  for *<*&gt;  for >&amp; for &&nbsp; for a non-breaking space&copy; for ©
```

### **How to Use HTML Entities**

Entities can be implemented easily within HTML code. Here are some examples:

```jsx
<p>The price is 10 &lt; 20.</p> <!-- Using Reserved Characters -->
<p>Copyright &copy; 2023.</p>  <!-- Displaying Special Symbols -->
<p>This is an example&nbsp;text.</p> <!-- Creating Non-Breaking Spaces -->
```

---

## HTML Quotation Tag

The **`<blockquote>`** and **`<q>`** tags serve to define quotations in HTML. While **`<blockquote>`** is used for longer, block-level quotes, **`<q>`** is used for shorter, inline quotes. They provide semantic meaning to your quotations, making it easier for search engines to understand the context and relevance of the content.

### **Basic Syntax**

#### **`<blockquote>` Tag**

```html
<blockquote cite="source-url">  Quotation text here.</blockquote>
```

#### **`<q>` Tag**

```html
<q cite="source-url">Quotation text here.</q>
```

### **Attributes**

Both **`<blockquote>`** and **`<q>`** tags support the **cite** attribute:

- **cite**: Specifies the URL of the quote's source.

### **Examples**

#### **Using `<blockquote>` for Long Quotes**

```html
<blockquote cite="https://example.com">  This is a long quote from an external source. This quote can span multiple lines and paragraphs.</blockquote>
```

#### **Using `<q>` for Short, Inline Quotes**

```html
The philosopher said, <q cite="https://example.com">The unexamined life is not worth living.</q>
```

---