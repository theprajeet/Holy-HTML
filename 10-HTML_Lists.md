# HTML Lists

Our day-to-day lives often involve the use of lists. For example, when we go shopping, the bill we receive includes a list of all the items we've purchased. In a similar manner, web developers use lists to neatly display data on websites.

**HTML lists** are **used to group a set of related items in a structured, organised format**. HTML provides three types of lists to display data in various forms. Each list contains one or more list items.

- **Unordered List:** Displays items using bullets.
- **Ordered List:** Displays items in a numerical sequence, and supports various numbering styles like Arabic numerals, Roman numerals, and so on.
- **Definition List:** Organizes items in a format similar to a dictionary, with terms and their corresponding definitions.

## **1. Unordered List**

An unordered list is a list of items that are not arranged in any specific, sequential order. Unlike ordered lists, the items in an unordered list are typically marked with bullet points, dashes, or other symbols to indicate list membership, but these markers do not imply any particular order.

### Characteristics

- No specific sequence is required.
- Typically displayed as bullet points.
- Defined using the **`<ul>`** tag.
- Individual items use the **`<li>`** tag.

```html
<ul>
  <li>Pen</li>
  <li>Pencil</li>
  <li>Eraser</li>
</ul>
```

### **Output:**

- Pen
- Pencil
- Eraser

### **Customizing Bullet Points with 'type' Attribute**

You can specify the style of bullet points using the **`type`** attribute. It supports three values:

- **`disc`** - default bullet style
- **`square`**
- **`circle`**

**Example Using Square Bullets:**

```html
<ul type="square">
  <li>Notebook</li>
  <li>Marker</li>
</ul>
```

---

## **2. Ordered List**

An ordered list is a list of items that are arranged in a specific, sequential order. Each item in the list is usually numbered to indicate its position in the sequence. Ordered lists are commonly used when the sequence of the items is important, such as in step-by-step instructions or rankings.

### Characteristics

- Ordered lists are used for items that follow a sequence.
- They are created using the **`<ol>`** (Ordered List) tag.
- List items are enclosed within **`<li>`** (List Item) tags.

### **Basic Example**

```html
<ol>
  <li>Mango</li>
  <li>Orange</li>
  <li>Litchi</li>
</ol>
```

### **Output:**

1. Mango
2. Orange
3. Litchi

### **Setting the 'type' Attribute**

The **`type`** attribute specifies the style of numbering. You have several options:

1. **Uppercase Roman Numerals**: Use **`type="I"`**
2. **Lowercase Roman Numerals**: Use **`type="i"`**
3. **Arabic Numerals**: Use **`type="1"`** (This is the default if the **`type`** attribute is not specified)
4. **Lowercase Alphabetical Letters**: Use **`type="a"`**
5. **Uppercase Alphabetical Letters**: Use **`type="A"`**

### **Setting the 'start' Attribute**

The **`start`** attribute specifies the starting number for the list.

```html
<ol type="A" start="3">
  <li>Pen</li>
  <li>Pencil</li>
</ol>
```

### **Output:**

1. Pen

 4.  Pencil

---

### **3. Definition List**

A Definition List in HTML is used to represent a list of terms along with their corresponding descriptions or definitions. The Definition List is created using the **`<dl>`** (Definition List) element, which wraps around one or more pairs of **`<dt>`** (Definition Term) and **`<dd>`** (Definition Description) elements.

Here's a simple example to illustrate:

```html
<h1>HTML Definition List</h1>
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language: The standard language for creating web pages.</dd>

  <dt>CSS</dt>
  <dd>Cascading Style Sheets: A stylesheet language used for describing the look and formatting of a document written in HTML.</dd>

  <dt>JavaScript</dt>
  <dd>A programming language commonly used in web development to add interactive features.</dd>
</dl>
```

### **Understanding the example**

In this example:

- **`<dl>`** is the container for the list.
- **`<dt>`** defines the terms that you want to explain.
- **`<dd>`** contains the definitions or explanations for the terms.

---

### Example

```jsx
<!DOCTYPE html>
<html>
<head>
    <title>HTML Lists</title>
</head>
<body>

    <h2>Ordered List</h2>
    <ol type="1">
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
        <li>React</li>
    </ol>

    <h2>Unordered List</h2>
    <ul type="square">
        <li>Apple</li>
        <li>Mango</li>
        <li>Orange</li>
        <li>Banana</li>
    </ul>

    <h2>Description List</h2>
    <dl>
        <dt>HTML</dt>
        <dd>HyperText Markup Language used to create web pages.</dd>

        <dt>CSS</dt>
        <dd>Cascading Style Sheets used to style web pages.</dd>

        <dt>JavaScript</dt>
        <dd>A programming language used to add interactivity to web pages.</dd>
    </dl>

</body>
</html>
```

### Output

```jsx
OUTPUT

Ordered List

1. HTML
2. CSS
3. JavaScript
4. React

Unordered List

■ Apple
■ Mango
■ Orange
■ Banana

Description List

HTML
    HyperText Markup Language used to create web pages.

CSS
    Cascading Style Sheets used to style web pages.

JavaScript
    A programming language used to add interactivity to web pages.
```

---