# HTML Attributes

**Attributes** provide additional information about an HTML element. They modify the behavior or appearance of an element and are always written inside the opening tag.

### **Characteristics of Attributes**

1. Attributes provide additional information about HTML tags.
2. Almost all HTML tags can have attributes.
3. A tag can have multiple attributes.
4. Attributes are always written in the opening tag.
5. Attributes are written as **key-value pairs**.
6. The syntax of an attribute is: `attribute="value"`

**Example:**

```html
<img src="nature.jpg" width="300" height="200" alt="Nature">
```

In the above example:

- `src` → Key
- `"nature.jpg"` → Value
- `width`, `height`, and `alt` are also attributes.

---

## **Types of HTML Attributes**

There are three main types of HTML attributes:

1. **Core Attributes**: These are basic attributes that can be applied to most HTML elements. Examples include **`id`**, **`class`**, and **`style`**.
2. **Internationalization Attributes**: These attributes help adapt the document to different languages and regions. Examples include **`lang`** and **`dir`**.
3. **Generic Attributes**: These attributes provide additional information about the element but don't necessarily affect its appearance or behavior. Examples include **`data-*`** attributes for storing custom data private to the page or application.

Core attributes are some of the most widely used attributes in HTML. There are four main types:

- **`id`**
- **`class`**
- **`title`**
- **`style`**

### **ID Attribute**

The ID attribute is used to assign a unique identifier to an HTML element. Each element with an ID has its own unique identity, similar to how each individual has a unique identity. Multiple elements cannot have the same ID.

Example:

```jsx
<p id="html">This is an HTML tutorial</p>
<p id="python">This is a Python tutorial</p>
```

In this example, the ID attribute helps to distinguish between two paragraphs by having different values: "html" and "python".

### **Class Attribute**

The class attribute is used to associate an HTML element with a particular class, typically for styling or JavaScript manipulation. Unlike the ID attribute, the class attribute is not unique, and multiple elements can share the same class.

Example:

```jsx
<p class="tutorial">This is an HTML tutorial</p>
<p class="tutorial">This is a CSS tutorial</p>
<p class="tutorial">This is a JavaScript tutorial</p>
```

### **Title Attribute**

The title attribute provides additional information about an element and is often displayed as a tooltip when the mouse hovers over it.

Example:

```jsx
<h4 title="hello, motto">Title attribute</h4>
```

### **Style Attribute**

The style attribute allows for inline styling of HTML elements. It is used in conjunction with CSS properties to directly style individual elements within the HTML code.

Example:

```jsx
<p style="color: red; font-size: 20px;">
    This text is red and 20px in size.
</p>
```

## **Case Sensitivity**

The HTML standard is flexible about the case of attribute names, allowing them to be written in either uppercase or lowercase, such as "title" or "TITLE." However, for best practices and compatibility with stricter document types like XHTML, the W3C recommends using lowercase attributes.

Example:

```jsx
<p TITLE="Hello">You can write attribute like this</p>
<p title="Hello">But this is the recommended way</p>
```

Both are treated the same way in normal HTML because HTML attribute names are **case-insensitive**. However, the recommended convention is to always use lowercase.

---