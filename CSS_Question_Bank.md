# CSS Question Bank

# 1. What is CSS? Why CSS?

### **What is CSS?**

CSS stands for **Cascading Style Sheets**. It is a stylesheet language that is used to describe the visual presentation of a web page written in **HTML (Hypertext Markup Language)**. HTML **creates the structure** of the page, while **CSS adds styling to that structure**.

### **Why the Term "Cascading"?**

The term "cascading" refers to the way CSS prioritises and applies styles when multiple rules target the same HTML element. This process considers specificity (how specific a rule is) and inheritance (styles passed from parent to child elements), ensuring the most relevant and recent rules take effect.

### **Why use CSS?**

CSS is essential for creating visually appealing and responsive websites. Here are some key reasons to use CSS:

- Enhances Visual Appeal: Transforms plain HTML into vibrant, professional-looking web pages.
- Improves User Experience: Makes websites intuitive and easy to navigate.
- Enables Responsive Design: Adapts layouts for various devices, from mobile phones to desktops.
- Supports Interactivity: Adds dynamic effects like hover states, transitions, and animations.
- Promotes Reusability: Allows the same styles to be applied across multiple pages, saving time and effort.

### **Key Features of CSS:**

CSS offers a wide range of capabilities that make it indispensable for web development:

- Styles and layouts of web pages.
- Works alongside HTML and XML documents.
- Enables responsive design for different screen sizes.
- Supports interactive effects like hover states and animations.
- CSS is now modularized, with ongoing updates rather than version numbers.
- Allows reusability of the same rules across multiple HTML documents.

---

# 2. How Does CSS Work?

CSS transforms a webpage by interacting with the DOM through a series of steps.

1. The user types the URL and clicks enter.
2. The browser makes a fetch request to the server.
3. HTML is fetched from the server.
4. HTML is converted into a DOM. In the DOM, each tag is considered a **node**.
5. The browser fetches all the related files and assets that are linked to that HTML, such as external CSS, fonts, images, etc.
6. The browser then parses the CSS and groups it based on the selectors, which can be tags.
7. Each CSS is attached to its respective node. In this phase, CSS gets attached to its respective node. This is called a **render tree**.
8. The render tree is the well-structured, well-arranged **DOM** node that will appear on the screen.
9. The well-structured, custom-designed website is presented on the screen. This is called **painting**.

### **What is a DOM?**

A DOM is like a tree-structure representation of all the tags and elements on the page. Each part of a web page, like headings, paragraphs, images, buttons, etc., will be part of the tree.

You can think of it as a blueprint for a web page that web browsers use to understand and display web content.

The tags are converted into nodes. Each node establishes a parent-child relationship with the others. To be precise, **Document Object Model (DOM)** is a sort of API that represents and interacts with HTML documents.

---

# **3. CSS Selectors**

**CSS Selectors** are patterns used to **select HTML elements** on which CSS styles should be applied. They tell the browser **which HTML elements should receive the specified styles**.

There are different types of CSS selectors, each used for selecting elements differently.

### **1. Universal Selector ()**

The **Universal Selector** selects **all the elements** present on a webpage.

**Example:**

```css
* {
    margin: 0;
    padding: 0;
}
```

### **2. Element Selector**

The **Element Selector** selects all elements of a particular HTML tag.

**Example:**

```css
p {
    color: blue;
}
```

This applies the blue color to all `<p>` elements.

### **3. ID Selector (`#`)**

The **ID Selector** selects an element using its unique **id** attribute. Since an ID should be unique within a webpage, it is generally used to style a single element.

**Example:**

```css
#title {
    color: red;
}
```

```html
<h1 id="title">Welcome</h1>
```

### **4. Class Selector (`.`)**

The **Class Selector** selects one or more elements having the same **class** attribute. Multiple elements can share the same class.

**Example:**

```css
.highlight {
    background-color: yellow;
}
```

```html
<p class="highlight">HTML</p>
<p class="highlight">CSS</p>
```

### **5. Group Selector (`,`)**

The **Group Selector** applies the same style to multiple elements by separating them with commas.

**Example:**

```css
h1, h2, p {
    color: green;
}
```

### **6. Descendant Selector (Space)**

The **Descendant Selector** selects elements that are inside another element, regardless of how deeply they are nested.

**Example:**

```css
div p {
    color: blue;
}
```

This selects all `<p>` elements that are inside a `<div>`.

### **7. Child Selector (`>`)**

The **Child Selector** selects only the **direct child** of a parent element.

**Example:**

```css
div > p {
    color: red;
}
```

Only the `<p>` elements that are immediate children of `<div>` will be selected.

### **8. Adjacent Sibling Selector (`+`)**

The **Adjacent Sibling Selector** selects the element that comes **immediately after** another element at the same level.

**Example:**

```css
h1 + p {
    color: blue;
}
```

This selects the first `<p>` that comes immediately after an `<h1>`.

### **9. General Sibling Selector (`~`)**

The **General Sibling Selector** selects all sibling elements that come **after** a specified element and share the same parent.

**Example:**

```css
h1 ~ p {
    color: green;
}
```

This selects all `<p>` elements that appear after an `<h1>` within the same parent.

---

# 4. Flex Property

**Flexbox (Flexible Box Layout)** is a CSS layout model used to arrange, align, and distribute elements efficiently within a container. It makes it easy to create responsive layouts without using floats or complex positioning.

Flexbox allows elements to automatically adjust their size and position based on the available space, making web page layouts more flexible and responsive.

### **Why Do We Use Flexbox?**

Before Flexbox, developers used methods like **float**, **inline-block**, and **positioning** to create layouts. These methods were difficult to manage, especially when aligning elements vertically or distributing space evenly.

Flexbox solves these problems by providing an easy way to:

- Arrange elements in rows or columns.
- Align items horizontally and vertically.
- Distribute space evenly between elements.
- Create responsive layouts.
- Reorder elements without changing the HTML.
- Allow items to grow or shrink based on available space.

### **Important Flexbox Properties**

Flexbox properties are divided into two categories:

- **Container Properties** – Applied to the parent (flex container).
- **Item Properties** – Applied to the child elements (flex items).

### **1. `display: flex`**

The `display: flex` property converts a normal HTML element into a **flex container**, making all its direct child elements **flex items**.

**Example:**

```css
.container {
    display: flex;
}
```

### **Container Properties**

### **2. `flex-direction`**

Defines the direction in which flex items are placed.

**Values:** `row`, `row-reverse`, `column`, `column-reverse`

**Example:**

```css
.container {
    display: flex;
    flex-direction: row;
}
```

### **3. `justify-content`**

Aligns flex items along the **main axis** (horizontal by default).

**Values:** `flex-start`, `center`, `flex-end`, `space-between`, `space-around`, `space-evenly`

**Example:**

```css
.container {
    display: flex;
    justify-content: space-between;
}
```

### **4. `align-items`**

Aligns flex items along the **cross axis** (vertical by default).

**Values:** `stretch`, `flex-start`, `center`, `flex-end`, `baseline`

**Example:**

```css
.container {
    display: flex;
    align-items: center;
}
```

### **5. `flex-wrap`**

Determines whether items should wrap onto the next line when there isn’t enough space.

**Values:** `nowrap`, `wrap`, `wrap-reverse`

**Example:**

```css
.container {
    display: flex;
    flex-wrap: wrap;
}
```

### **6. `gap`**

Adds space between flex items without using margins.

**Example:**

```css
.container {
    display: flex;
    gap: 20px;
}
```

### **Item Properties**

### **7. `flex-grow`**

Specifies how much a flex item should grow relative to the other items when extra space is available.

**Example:**

```css
.item {
    flex-grow: 1;
}
```

### **8. `flex-shrink`**

Specifies how much a flex item should shrink when there isn’t enough space.

**Example:**

```css
.item {
    flex-shrink: 1;
}
```

### **9. `flex-basis`**

Defines the initial size of a flex item before the remaining space is distributed.

**Example:**

```css
.item {
    flex-basis: 200px;
}
```

### **10. `flex`**

A shorthand property for `flex-grow`, `flex-shrink`, and `flex-basis`.

**Syntax:**

```css
flex: flex-grow flex-shrink flex-basis;
```

**Example:**

```css
.item {
    flex: 1 1 200px;
}
```

### **11. `align-self`**

Allows an individual flex item to override the `align-items` property of the container.

**Example:**

```css
.item {
    align-self: flex-end;
}
```

### **Example**

```html
<!DOCTYPE html>
<html>
<head>
<style>
.container {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    gap: 20px;
    height: 200px;
    border: 2px solid black;
}

.box {
    width: 80px;
    height: 80px;
    background-color: lightblue;
    text-align: center;
    line-height: 80px;
}
</style>
</head>

<body>

<div class="container">
    <div class="box">1</div>
    <div class="box">2</div>
    <div class="box">3</div>
</div>

</body>
</html>
```

### **Output**

```
+------------------------------------------------------+
|                                                      |
|     [ 1 ]         [ 2 ]         [ 3 ]                |
|                                                      |
+------------------------------------------------------+
```

The three boxes are arranged in a row, centered vertically, and evenly spaced horizontally.

---

# 5. Background Properties in CSS

Background properties in CSS are used to control the appearance of an element’s background. They allow you to set background colors, images, image positions, repetition, size, and attachment. These properties help make web pages visually appealing and improve the overall design.

### **1. `background-color`**

The `background-color` property is used to set the background color of an element.

**Syntax:**

```css
selector {
    background-color: color;
}
```

**Example:**

```css
body {
    background-color: lightblue;
}
```

### **2. `background-image`**

The `background-image` property is used to set an image as the background of an element.

**Syntax:**

```css
selector {
    background-image: url("image.jpg");
}
```

**Example:**

```css
body {
    background-image: url("nature.jpg");
}
```

### **3. `background-repeat`**

The `background-repeat` property specifies whether a background image should repeat.

**Values:** `repeat`, `repeat-x`, `repeat-y`, `no-repeat`

**Example:**

```css
body {
    background-image: url("logo.png");
    background-repeat: no-repeat;
}
```

### **4. `background-position`**

The `background-position` property specifies the position of the background image.

**Common Values:** `left`, `right`, `top`, `bottom`, `center`, `left top`, `right bottom`

**Example:**

```css
body {
    background-image: url("logo.png");
    background-position: center;
}
```

### **5. `background-size`**

The `background-size` property specifies the size of the background image.

**Values:** `auto`, `cover`, `contain`, or custom values like `300px 200px`

**Example:**

```css
body {
    background-image: url("nature.jpg");
    background-size: cover;
}
```

- `cover` – The image covers the entire element while maintaining its aspect ratio.
- `contain` – The entire image is visible within the element while maintaining its aspect ratio.

### **6. `background-attachment`**

The `background-attachment` property specifies whether the background image scrolls with the page or remains fixed.

**Values:** `scroll`, `fixed`, `local`

**Example:**

```css
body {
    background-image: url("nature.jpg");
    background-attachment: fixed;
}
```

### **7. `background-origin`**

The `background-origin` property specifies the area from which the background image starts.

**Values:** `padding-box`, `border-box`, `content-box`

**Example:**

```css
div {
    background-origin: content-box;
}
```

### **8. `background-clip`**

The `background-clip` property specifies how far the background extends within an element.

**Values:** `border-box`, `padding-box`, `content-box`

**Example:**

```css
div {
    background-clip: padding-box;
}
```

### **9. `background` (Shorthand Property)**

The `background` property is a shorthand property that combines multiple background properties into a single declaration.

**Syntax:**

```css
selector {
    background: color image repeat attachment position / size;
}
```

**Example:**

```css
body {
    background: lightblue url("nature.jpg") no-repeat fixed center/cover;
}
```

### **Example**

```html
<!DOCTYPE html>
<html>
<head>
    <style>
        body {
            background-color: lightgray;
            background-image: url("nature.jpg");
            background-repeat: no-repeat;
            background-position: center;
            background-size: cover;
            background-attachment: fixed;
        }

        h1 {
            color: white;
            text-align: center;
        }
    </style>
</head>
<body>

    <h1>Welcome to CSS Background Properties</h1>

</body>
</html>
```

---

# 6. CSS Box Model

The **CSS Box Model** is a layout model that defines how every HTML element is displayed on a web page. According to the Box Model, every element is treated as a **rectangular box** consisting of four parts: **Content**, **Padding**, **Border**, and **Margin**.

Understanding the Box Model is essential because it determines the total space occupied by an element and helps in designing proper layouts.

### **Components of the CSS Box Model**

The CSS Box Model consists of the following four parts (from inside to outside):

1. Content
2. Padding
3. Border
4. Margin

```
        +---------------------------+
        |          Margin           |
        |  +---------------------+  |
        |  |       Border        |  |
        |  |  +---------------+  |  |
        |  |  |    Padding    |  |  |
        |  |  | +-----------+ |  |  |
        |  |  | |  Content  | |  |  |
        |  |  | +-----------+ |  |  |
        |  |  +---------------+  |  |
        |  +---------------------+  |
        +---------------------------+
```

### **1. Content**

The **Content** is the actual area where text, images, videos, or other HTML elements are displayed. By default, the `width` and `height` properties apply only to the content area.

**Example:**

```css
div {
    width: 300px;
    height: 150px;
}
```

### **2. Padding**

**Padding** is the space between the content and the border. It creates inner spacing, making the content appear away from the border.

Padding can be applied individually to each side.

**Properties:** `padding`, `padding-top`, `padding-right`, `padding-bottom`, `padding-left`

**Example:**

```css
div {
    padding: 20px;
}
```

### **3. Border**

The **Border** surrounds the padding and content. It provides an outline around the element and can have different widths, styles, and colors.

**Properties:** `border`, `border-width`, `border-style`, `border-color`

**Example:**

```css
div {
    border: 2px solid black;
}
```

### **4. Margin**

**Margin** is the space outside the border. It creates separation between one element and another.

Margins are transparent and do not have a background color.

**Properties:** `margin`, `margin-top`, `margin-right`, `margin-bottom`, `margin-left`

**Example:**

```css
div {
    margin: 30px;
}
```

### **Total Width of an Element**

The total width occupied by an element is calculated as:

```
Total Width = Margin (Left + Right)
            + Border (Left + Right)
            + Padding (Left + Right)
            + Content Width
```

### **Total Height of an Element**

The total height occupied by an element is calculated as:

```
Total Height = Margin (Top + Bottom)
             + Border (Top + Bottom)
             + Padding (Top + Bottom)
             + Content Height
```

### **Example**

```html
<!DOCTYPE html>
<html>
<head>
<style>
div {
    width: 250px;
    height: 100px;
    padding: 20px;
    border: 3px solid blue;
    margin: 30px;
    background-color: lightgray;
}
</style>
</head>

<body>

<div>
    This is a CSS Box Model Example.
</div>

</body>
</html>
```

### **Output**

```
           Margin
+--------------------------------------+
|              Border                  |
|  +--------------------------------+  |
|  |           Padding              |  |
|  |  +--------------------------+  |  |
|  |  |        Content           |  |  |
|  |  | This is a CSS Box Model  |  |  |
|  |  | Example.                 |  |  |
|  |  +--------------------------+  |  |
|  +--------------------------------+  |
+--------------------------------------+
```

### **`box-sizing` Property**

By default, CSS uses `box-sizing: content-box`, where the specified `width` and `height` apply only to the content.

Using `box-sizing: border-box`, the specified `width` and `height` include the content, padding, and border, making layout calculations easier.

**Example:**

```css
div {
    width: 300px;
    padding: 20px;
    border: 2px solid black;
    box-sizing: border-box;
}
```

---

# 7. CSS Color and Gradient.

CSS provides different ways to add colors and gradients to web pages. **Colors** are used to style text, backgrounds, and borders, while **Gradients** create a smooth transition between two or more colors without using images. They help make web pages more attractive and visually appealing.

### **CSS Colors**

CSS supports multiple ways of specifying colors.

#### **1. Color Name**

A color can be specified using predefined color names.

**Example:**

```css
h1 {
    color: red;
}
```

### **2. Hexadecimal (HEX) Color**

A hexadecimal color is represented using a `#` followed by six hexadecimal digits.

**Syntax:**

```css
color: #RRGGBB;
```

**Example:**

```css
p {
    color: #0000FF;
}
```

### **3. RGB Color**

The RGB color model specifies colors using **Red**, **Green**, and **Blue** values ranging from **0 to 255**.

**Syntax:**

```css
color: rgb(red, green, blue);
```

**Example:**

```css
h2 {
    color: rgb(255, 0, 0);
}
```

### **4. RGBA Color**

RGBA is similar to RGB but includes an **Alpha (opacity)** value ranging from **0.0 to 1.0**.

**Syntax:**

```css
color: rgba(red, green, blue, alpha);
```

**Example:**

```css
div {
    background-color: rgba(0, 0, 255, 0.5);
}
```

### **5. HSL Color**

HSL stands for **Hue, Saturation, and Lightness**.

- **Hue:** 0°–360°
- **Saturation:** 0%–100%
- **Lightness:** 0%–100%

**Syntax:**

```css
color: hsl(hue, saturation, lightness);
```

**Example:**

```css
h3 {
    color: hsl(120, 100%, 50%);
}
```

### **6. HSLA Color**

HSLA is the HSL color model with an additional **Alpha (opacity)** value.

**Syntax:**

```css
color: hsla(hue, saturation, lightness, alpha);
```

**Example:**

```css
div {
    background-color: hsla(200, 80%, 50%, 0.6);
}
```

### **CSS Gradients**

A **CSS Gradient** is a gradual transition between two or more colors. Gradients are commonly used as backgrounds and do not require image files.

There are three main types of gradients in CSS.

### **1. Linear Gradient**

A **Linear Gradient** changes colors in a straight line.

**Syntax:**

```css
background: linear-gradient(direction, color1, color2);
```

**Example:**

```css
div {
    background: linear-gradient(to right, red, yellow);
}
```

### **2. Radial Gradient**

A **Radial Gradient** changes colors outward from the center in a circular or elliptical shape.

**Syntax:**

```css
background: radial-gradient(color1, color2);
```

**Example:**

```css
div {
    background: radial-gradient(red, yellow);
}
```

### **3. Conic Gradient**

A **Conic Gradient** changes colors around a center point, similar to the slices of a pie chart.

**Syntax:**

```css
background: conic-gradient(color1, color2, color3);
```

**Example:**

```css
div {
    background: conic-gradient(red, yellow, green);
}
```

### **Example**

```html
<!DOCTYPE html>
<html>
<head>
<style>
body {
    background: linear-gradient(to right, lightblue, white);
    font-family: Arial, sans-serif;
}

h1 {
    color: #003366;
}

.box {
    width: 300px;
    height: 150px;
    margin: 20px;
    color: white;
    text-align: center;
    line-height: 150px;
    background: radial-gradient(blue, purple);
}
</style>
</head>

<body>

<h1>CSS Colors and Gradients</h1>

<div class="box">
    Gradient Background
</div>

</body>
</html>
```

---

# **8. CSS Positions**

     The **`position`** property in CSS is used to control how an HTML element is positioned on a web page. It determines whether an element follows the normal document flow or is positioned relative to its parent, the viewport, or its original location.

The position of an element can be adjusted using the following properties:

- `top`
- `right`
- `bottom`
- `left`

CSS provides five main positioning values:

- `static`
- `relative`
- `absolute`
- `fixed`
- `sticky`

### **1. `position: static`**

The **static** position is the default position for all HTML elements. An element with `position: static` follows the normal flow of the document, and the `top`, `right`, `bottom`, and `left` properties have no effect.

**Example:**

```css
.box {
    position: static;
}
```

### **2. `position: relative`**

An element with `position: relative` remains in the normal document flow but can be moved from its original position using the `top`, `right`, `bottom`, and `left` properties.

The space originally occupied by the element is still preserved.

**Example:**

```css
.box {
    position: relative;
    top: 20px;
    left: 30px;
}
```

### **3. `position: absolute`**

An element with `position: absolute` is removed from the normal document flow and is positioned relative to its **nearest positioned ancestor** (an ancestor with `position: relative`, `absolute`, `fixed`, or `sticky`). If no positioned ancestor exists, it is positioned relative to the entire webpage.

**Example:**

```css
.parent {
    position: relative;
}

.child {
    position: absolute;
    top: 20px;
    right: 10px;
}
```

### **4. `position: fixed`**

An element with `position: fixed` is positioned relative to the browser’s viewport. It remains in the same position even when the user scrolls the page.

This is commonly used for navigation bars, chat buttons, and floating action buttons.

**Example:**

```css
.box {
    position: fixed;
    bottom: 20px;
    right: 20px;
}
```

### **5. `position: sticky`**

An element with `position: sticky` behaves like a `relative` element until a specified scroll position is reached. After that, it behaves like a `fixed` element and remains visible until its parent container ends.

This is commonly used for sticky navigation bars and table headers.

**Example:**

```css
.header {
    position: sticky;
    top: 0;
}
```

### **Example**

```html
<!DOCTYPE html>
<html>
<head>
<style>
.container {
    position: relative;
    width: 400px;
    height: 250px;
    border: 2px solid black;
}

.relative-box {
    position: relative;
    top: 10px;
    left: 20px;
    background-color: lightblue;
    padding: 10px;
}

.absolute-box {
    position: absolute;
    top: 20px;
    right: 20px;
    background-color: lightgreen;
    padding: 10px;
}

.fixed-box {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: orange;
    padding: 10px;
}

.sticky-box {
    position: sticky;
    top: 0;
    background-color: yellow;
    padding: 10px;
}
</style>
</head>

<body>

<div class="sticky-box">
    Sticky Header
</div>

<div class="container">
    <div class="relative-box">Relative</div>
    <div class="absolute-box">Absolute</div>
</div>

<div class="fixed-box">
    Fixed Button
</div>

</body>
</html>
```

### **Output**

```
-----------------------------------------------
| Sticky Header                               |
-----------------------------------------------

+-----------------------------------------+
|                                         |
|   Relative                              |
|                               Absolute  |
|                                         |
+-----------------------------------------+

                             Fixed Button
```

### **Difference Between CSS Positions**

| **Position** | **Follows Normal Flow** | **Can Use top/right/bottom/left** | **Scrolls with Page** | **Reference Point** |
| --- | --- | --- | --- | --- |
| `static` | Yes | No | Yes | Normal document flow |
| `relative` | Yes | Yes | Yes | Its original position |
| `absolute` | No | Yes | Yes | Nearest positioned ancestor |
| `fixed` | No | Yes | No | Browser viewport |
| `sticky` | Yes (initially) | Yes | Sticks while scrolling | Scroll position within its parent |

---

# 9. Transition, Transform and Animation in CSS.

**Transition**, **Transform**, and **Animation** are CSS features used to create interactive and visually appealing web pages. They allow elements to move, change size, rotate, scale, fade, and animate without using JavaScript.

### **CSS Transition**

A **Transition** allows a CSS property to change **smoothly** from one value to another over a specified period of time. It is commonly used with pseudo-classes like `:hover`, `:focus`, or when a property value changes.

A transition requires at least two states:

- Initial state
- Final state

#### **Transition Properties**

- `transition-property` – Specifies the CSS property to animate.
- `transition-duration` – Specifies how long the transition takes.
- `transition-timing-function` – Specifies the speed curve of the transition.
- `transition-delay` – Specifies the delay before the transition starts.

#### **Shorthand Syntax**

```css
selector {
    transition: property duration timing-function delay;
}
```

#### **Example**

```css
.button {
    width: 150px;
    background-color: blue;
    color: white;
    transition: background-color 0.5s ease;
}

.button:hover {
    background-color: green;
}
```

When the mouse pointer is placed over the button, the background color changes smoothly from blue to green in **0.5 seconds**.

### **CSS Transform**

The **Transform** property is used to change the shape, size, position, or orientation of an element without affecting the layout of surrounding elements.

Common transform functions include:

- `translate()`
- `rotate()`
- `scale()`
- `skew()`

#### **1. `translate()`**

Moves an element horizontally and/or vertically.

**Example:**

```css
.box {
    transform: translate(50px, 20px);
}
```

#### **2. `rotate()`**

Rotates an element by a specified angle.

**Example:**

```css
.box {
    transform: rotate(45deg);
}
```

#### **3. `scale()`**

Increases or decreases the size of an element.

**Example:**

```css
.box {
    transform: scale(1.5);
}
```

#### **4. `skew()`**

Tilts an element along the X-axis, Y-axis, or both.

**Example:**

```css
.box {
    transform: skew(20deg, 10deg);
}
```

### **CSS Animation**

A **CSS Animation** allows an element to change its appearance or position automatically over time. Unlike transitions, animations do not require user interaction and can repeat continuously.

Animations are created using the `@keyframes` rule.

#### **Animation Properties**

- `animation-name` – Specifies the name of the animation.
- `animation-duration` – Specifies how long the animation takes.
- `animation-timing-function` – Specifies the speed curve.
- `animation-delay` – Specifies the delay before the animation starts.
- `animation-iteration-count` – Specifies the number of times the animation repeats.
- `animation-direction` – Specifies the direction of the animation.
- `animation-fill-mode` – Specifies the styles before or after the animation.
- `animation-play-state` – Specifies whether the animation is running or paused.

#### **Shorthand Syntax**

```css
selector {
    animation: name duration timing-function delay iteration-count direction;
}
```

#### **Example**

```css
@keyframes moveBox {
    from {
        transform: translateX(0);
    }

    to {
        transform: translateX(200px);
    }
}

.box {
    width: 100px;
    height: 100px;
    background-color: red;
    animation: moveBox 3s linear infinite;
}
```

The box moves from left to right continuously, taking **3 seconds** to complete one cycle.

### **Example**

```html
<!DOCTYPE html>
<html>
<head>
<style>

.button {
    padding: 10px 20px;
    background-color: blue;
    color: white;
    border: none;
    transition: background-color 0.5s ease;
}

.button:hover {
    background-color: green;
}

.box {
    width: 100px;
    height: 100px;
    background-color: orange;
    margin-top: 20px;
    transition: transform 0.5s;
}

.box:hover {
    transform: rotate(45deg) scale(1.2);
}

.circle {
    width: 80px;
    height: 80px;
    background-color: red;
    border-radius: 50%;
    margin-top: 20px;
    animation: bounce 2s infinite;
}

@keyframes bounce {
    0%   { transform: translateY(0); }
    50%  { transform: translateY(-80px); }
    100% { transform: translateY(0); }
}

</style>
</head>

<body>

<button class="button">Hover Me</button>

<div class="box"></div>

<div class="circle"></div>

</body>
</html>
```

### **Output**

```
[ Hover Me ]

□  ← Rotates and enlarges when hovered.

●  ← Continuously moves up and down automatically.
```

### **Difference Between Transition, Transform, and Animation**

| **Feature** | **Transition** | **Transform** | **Animation** |
| --- | --- | --- | --- |
| Purpose | Creates a smooth change between two states. | Changes the shape, size, position, or orientation of an element. | Creates continuous or multi-step animations. |
| Trigger | Requires a property change (e.g., `:hover`). | Applied immediately when used. | Runs automatically or when triggered. |
| Uses `@keyframes` | No | No | Yes |
| Repeats Automatically | No | No | Yes (using `animation-iteration-count`) |
| Common Uses | Hover effects, button color changes. | Rotate, scale, move, skew elements. | Loading spinners, bouncing balls, sliding objects, fading effects. |

---

# 10. CSS Media Queries

**Media Queries** are a feature of CSS used to apply different styles to a webpage based on the characteristics of the user’s device, such as screen width, screen height, orientation, or resolution.

Media queries are mainly used to create **responsive web designs**, allowing a website to look good on desktops, laptops, tablets, and mobile phones without changing the HTML.

### **Why Do We Use Media Queries?**

Different devices have different screen sizes. A webpage designed only for a desktop may not display properly on a mobile phone. Media queries solve this problem by applying different CSS rules for different devices.

Some common uses of media queries are:

- Creating responsive websites.
- Adjusting layouts for different screen sizes.
- Changing font sizes for better readability.
- Showing or hiding elements on specific devices.
- Rearranging navigation menus for mobile devices.
- Optimizing images and spacing for different screens.

### **Syntax of Media Query**

```css
@media media-type and (condition) {
    /* CSS Rules */
}
```

The **media-type** is optional and is usually `screen`.

The **condition** specifies when the CSS rules should be applied.

### **Common Media Features**

- `max-width`
- `min-width`
- `max-height`
- `min-height`
- `orientation`
- `resolution`

### **1. `max-width`**

The CSS rules are applied when the screen width is **less than or equal to** the specified value.

**Example:**

```css
@media (max-width: 768px) {
    body {
        background-color: lightblue;
    }
}
```

If the screen width is **768px or smaller**, the background color becomes light blue.

### **2. `min-width`**

The CSS rules are applied when the screen width is **greater than or equal to** the specified value.

**Example:**

```css
@media (min-width: 992px) {
    body {
        background-color: lightgreen;
    }
}
```

If the screen width is **992px or larger**, the background color becomes light green.

### **3. `orientation`**

The `orientation` media feature checks whether the device is in **portrait** or **landscape** mode.

**Example:**

```css
@media (orientation: landscape) {
    body {
        background-color: lightyellow;
    }
}
```

The background color changes when the device is in landscape mode.

### **4. Combining Conditions**

Multiple conditions can be combined using the `and` keyword.

**Example:**

```css
@media screen and (min-width: 600px) and (max-width: 900px) {
    body {
        background-color: lightpink;
    }
}
```

The CSS rules apply only when the screen width is between **600px and 900px**.

### **Complete Example**

```html
<!DOCTYPE html>
<html>
<head>
<style>

body {
    background-color: white;
    font-size: 20px;
}

@media (max-width: 768px) {
    body {
        background-color: lightblue;
        font-size: 16px;
    }
}

@media (max-width: 480px) {
    body {
        background-color: lightgreen;
        font-size: 14px;
    }
}

</style>
</head>

<body>

<h1>CSS Media Queries</h1>
<p>Resize the browser window to see the changes.</p>

</body>
</html>
```

### **Output**

- **Desktop (Width > 768px):**
    - White background
    - Font size: 20px
- **Tablet (Width ≤ 768px):**
    - Light blue background
    - Font size: 16px
- **Mobile (Width ≤ 480px):**
    - Light green background
    - Font size: 14px

---

# 11. Bootstrap and Tailwind CSS

**Bootstrap** and **Tailwind CSS** are popular CSS frameworks used to design responsive and modern websites quickly. They provide pre-written CSS that reduces the amount of custom styling developers need to write.

Although both frameworks help in building attractive user interfaces, they follow different approaches.

### **Bootstrap**

**Bootstrap** is a front-end CSS framework developed by Twitter. It provides a collection of **pre-designed components** such as buttons, forms, cards, navigation bars, alerts, and modals. Developers can quickly build responsive websites by using Bootstrap’s ready-made classes.

Bootstrap follows a **component-based approach**, where you use predefined components with built-in styles.

### **Features of Bootstrap**

- Ready-made UI components.
- Responsive grid system.
- Mobile-first design.
- Built-in utility classes.
- Easy to learn and use.
- Large community and documentation.
- Supports JavaScript components like modals, carousels, and dropdowns.

### **Example**

```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet"
          href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css">
</head>

<body>

<button class="btn btn-primary">
    Click Me
</button>

</body>
</html>
```

In this example, the classes `btn` and `btn-primary` create a blue Bootstrap button without writing custom CSS.

### **Tailwind CSS**

**Tailwind CSS** is a utility-first CSS framework that provides small utility classes for styling HTML elements. Instead of using pre-designed components, developers build their own designs by combining utility classes directly in the HTML.

Tailwind CSS offers greater flexibility and customization compared to Bootstrap.

### **Features of Tailwind CSS**

- Utility-first approach.
- Highly customizable.
- Responsive design utilities.
- Smaller production CSS after optimization.
- Easy to create unique designs.
- No predefined components.
- Supports dark mode and modern CSS features.

### **Example**

```html
<!DOCTYPE html>
<html>
<head>
    <script src="https://cdn.tailwindcss.com"></script>
</head>

<body>

<button class="bg-blue-600 text-white px-4 py-2 rounded">
    Click Me
</button>

</body>
</html>
```

In this example:

- `bg-blue-600` sets the background color.
- `text-white` sets the text color.
- `px-4` adds horizontal padding.
- `py-2` adds vertical padding.
- `rounded` gives rounded corners.

### **When to Use Bootstrap**

- Rapid application development.
- Admin dashboards.
- Business websites.
- Projects requiring ready-made UI components.
- Beginners learning web development.

### **When to Use Tailwind CSS**

- Custom website designs.
- Modern web applications.
- React, Vue, and Angular projects.
- Projects requiring complete design flexibility.
- Applications where optimized CSS size is important.

---