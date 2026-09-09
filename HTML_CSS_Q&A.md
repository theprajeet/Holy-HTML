# HTML CSS Questions & Answers

# HTML Questions & Answers

### 1. What is HTML, and is it a programming language?

HTML stands for **HyperText Markup Language**. It is used to define the
structure and content of a webpage.

HTML is **not a programming language** because it does not contain
programming logic such as conditions, loops, or functions. It is a
**markup language**.

---

### 2. What is the basic structure of an HTML document, and why is `<!DOCTYPE html>` used?

A basic HTML document contains:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>
    Page content
</body>
</html>
```

`<!DOCTYPE html>` tells the browser that the document uses **HTML5** and
makes the browser render the page in standards mode.

---

### 3. What is the difference between an HTML tag, element, and attribute?

- **Tag** → The markup itself, such as `<p>` or `</p>`.
- **Element** → The complete structure, such as `<p>Hello</p>`.
- **Attribute** → Additional information provided to an element, such
as `id="name"`.

Example:

```html
<p id="intro">Hello</p>
```

Here `<p>` is the tag, `<p id="intro">Hello</p>` is the element, and
`id="intro"` is the attribute.

---

### 4. What is the difference between paired and unpaired/void elements?

**Paired elements** have an opening and closing tag:

```html
<p>Hello</p>
```

**Void elements** do not have a closing tag:

```html
<img src="photo.jpg" alt="Photo">
```

Examples of void elements include `<img>`, `<input>`, and `<br>`.

---

### 5. What is the difference between block-level and inline elements?

A **block-level element** normally starts on a new line and takes up the
available width.

Examples: `<div>`, `<p>`, `<h1>`.

An **inline element** normally occupies only the space required by its
content.

Examples: `<span>`, `<a>`, `<strong>`.

---

### 6. What is the difference between `<div>` and `<span>`?

`<div>` is generally a **block-level container**, while `<span>` is
generally an **inline container**.

```html
<div>This is a block</div>
<span>This is inline</span>
```

Both are non-semantic containers; the main difference is their default
display behavior.

---

### 7. What is the difference between `<b>` and `<strong>`?

Both commonly appear bold, but their meaning is different.

`<b>` is mainly used to draw attention stylistically.

`<strong>` indicates that the content has **strong importance**.

Semantic HTML is preferred when the meaning of the content matters.

---

### 8. What is the difference between `<i>` and `<em>`?

Both commonly appear italic by default.

`<i>` represents text that is stylistically offset from normal text.

`<em>` represents **emphasis** and carries semantic meaning.

---

### 9. What is the difference between `<p>` and `<pre>`?

`<p>` represents a paragraph and normal HTML whitespace is generally
collapsed.

`<pre>` preserves whitespace and line breaks, making it useful when the
exact formatting of text matters.

---

### 10. What is the purpose of the `alt` attribute in an `<img>` tag?

`alt` provides alternative text describing an image.

It is useful when the image cannot be displayed and is important for
**accessibility**, because screen readers can use the alternative text.

```html
<img src="cat.jpg" alt="A cat sitting on a chair">
```

---

### 11. What is the difference between an absolute path and a relative path?

An **absolute path** specifies the complete location of a resource.

```html
<a href="https://example.com/about.html">About</a>
```

A **relative path** specifies the location relative to the current
document.

```html
<a href="about.html">About</a>
```

Relative paths are commonly used when linking files within the same
project.

---

### 12. What does `target="_blank"` do?

It tells the browser to open the linked document in a new browsing
context, commonly a new tab.

```html
<a href="https://example.com" target="_blank">Visit</a>
```

---

### 13. How would you make an image clickable?

Place the `<img>` inside an `<a>` element.

```html
<a href="https://example.com">
    <img src="logo.png" alt="Logo">
</a>
```

---

### 14. What is the difference between `<th>` and `<td>`?

`<th>` represents a **table header cell**.

`<td>` represents a **table data cell**.

```html
<tr>
    <th>Name</th>
    <th>Age</th>
</tr>
<tr>
    <td>John</td>
    <td>22</td>
</tr>
```

---

### 15. What is the difference between `rowspan` and `colspan`?

`rowspan` makes a cell span multiple **rows**.

`colspan` makes a cell span multiple **columns**.

```html
<td rowspan="2">A</td>
<td colspan="2">B</td>
```

---

### 16. What is the difference between `cellpadding` and `cellspacing`?

`cellpadding` refers to the space **inside a table cell**, between the
cell content and its border.

`cellspacing` refers to the space **between table cells**.

In modern development, CSS is generally preferred for controlling table
spacing.

---

### 17. How would you merge two rows or two columns in a table?

Use `rowspan` to merge rows:

```html
<td rowspan="2">Merged</td>
```

Use `colspan` to merge columns:

```html
<td colspan="2">Merged</td>
```

---

### 18. What is the difference between `<ol>`, `<ul>`, and `<dl>`?

- `<ol>` → Ordered list, where order matters.
- `<ul>` → Unordered list.
- `<dl>` → Description list containing terms and descriptions.

Example:

```html
<ol>
    <li>First</li>
    <li>Second</li>
</ol>

<ul>
    <li>Apple</li>
    <li>Orange</li>
</ul>

<dl>
    <dt>HTML</dt>
    <dd>Markup language for webpages.</dd>
</dl>
```

---

### 19. How do you create a nested list in HTML?

Place another list inside an `<li>` element.

```html
<ul>
    <li>Frontend
        <ul>
            <li>HTML</li>
            <li>CSS</li>
        </ul>
    </li>
</ul>
```

---

### 20. What is the difference between radio buttons and checkboxes?

**Radio buttons** are generally used when the user should select **one
option from a group**.

**Checkboxes** allow the user to select **multiple independent
options**.

```html
<input type="radio" name="gender" value="male">
<input type="radio" name="gender" value="female">

<input type="checkbox" name="skills" value="html">
<input type="checkbox" name="skills" value="css">
```

Radio buttons with the same `name` form a group.

---

### 21. What is the purpose of the `<label>` element, and how do you associate it with an input?

`<label>` provides a text label for a form control and improves
usability and accessibility.

Associate it using the input’s `id`:

```html
<label for="username">Username</label>
<input type="text" id="username">
```

The `for` value matches the input’s `id`.

---

### 22. What is the difference between the `id` and `name` attributes of a form input?

`id` uniquely identifies an element in the HTML document and is commonly
used with labels and CSS/JavaScript.

`name` identifies the form field when its value is submitted as form
data.

```html
<label for="username">Username</label>
<input id="username" name="username">
```

They can have the same value, but they serve different purposes.

---

### 23. What is the difference between GET and POST?

**GET** sends form data as part of the URL. It is commonly used for
retrieving data.

**POST** sends data in the request body and is commonly used when
submitting or creating data.

Sensitive data should not be treated as secure merely because POST is
used; HTTPS is what protects data in transit.

---

### 24. What is the purpose of the `action` attribute in a form?

`action` specifies the URL/resource to which the form data should be
submitted.

```html
<form action="/login" method="post">
```

Here, the form data is submitted to `/login`.

---

### 25. What is the difference between `<input>`, `<select>`, and `<textarea>`?

- `<input>` → Single-line input and supports many types such as text,
email, number, date, radio, checkbox, etc.
- `<select>` → Provides a dropdown selection.
- `<textarea>` → Provides a multi-line text input.

---

### 26. What is the difference between `<select>` and `<datalist>`?

`<select>` provides a predefined set of options from which the user
selects.

`<datalist>` provides suggestions for an input, while still allowing the
user to enter a value.

---

### 27. What do `required`, `maxlength`, `pattern`, and `placeholder` do?

- `required` → Makes the field mandatory.
- `maxlength` → Limits the maximum number of characters.
- `pattern` → Requires the value to match a specified regular
expression.
- `placeholder` → Displays a temporary hint inside the input.

Example:

```html
<input
    type="text"
    placeholder="Enter username"
    maxlength="20"
    pattern="[A-Za-z0-9]+"
    required
>
```

---

### 28. What is the purpose of the `pattern` attribute? Give an example.

`pattern` allows you to specify a regular expression that the input
value must match.

```html
<input type="text" pattern="[A-Za-z]+" required>
```

This example requires alphabetic characters only.

---

### 29. What are semantic HTML elements, and why should we use them?

Semantic elements clearly describe the meaning or role of their content.

Examples:

```html
<header>
<nav>
<main>
<section>
<article>
<aside>
<footer>
```

They make the structure easier for developers, assistive technologies,
and search engines to understand.

---

### 30. What is the difference between semantic and non-semantic elements?

Semantic elements describe **what the content means**.

For example:

```html
<article>...</article>
```

Non-semantic elements do not describe the meaning of their content.

For example:

```html
<div>...</div>
```

---

### 31. What is the difference between `<section>` and `<article>`?

`<section>` represents a thematic section of a document.

`<article>` represents a self-contained piece of content that could
potentially stand on its own, such as an article, blog post, or news
item.

---

### 32. What is the purpose of `<header>`, `<nav>`, `<main>`, `<aside>`, and `<footer>`?

- `<header>` → Introductory/header content.
- `<nav>` → Navigation links.
- `<main>` → Main content of the document.
- `<aside>` → Related/sidebar content.
- `<footer>` → Footer information.

---

### 33. How does semantic HTML improve accessibility and SEO?

Semantic elements give browsers and assistive technologies meaningful
information about page structure.

They also provide search engines with clearer information about the
organization and meaning of page content.

---

### 34. Given a webpage structure, which semantic HTML elements would you choose and why?

Use elements according to their meaning rather than simply using `<div>`
everywhere.

For example:

```html
<header>...</header>
<nav>...</nav>

<main>
    <article>
        ...
    </article>

    <aside>
        ...
    </aside>
</main>

<footer>...</footer>
```

The choice should be based on the role of each section.

---

### 35. Given a piece of HTML, identify which elements are block-level, inline, semantic, or void elements.

Look at the element’s normal HTML behavior and purpose.

For example:

- `<div>` → block-level, non-semantic
- `<p>` → block-level, semantic
- `<span>` → inline, non-semantic
- `<a>` → inline
- `<img>` → void element
- `<header>` → block-level semantic element

---

# CSS Questions & Answers

### 1. What is CSS, and why is it used?

CSS stands for **Cascading Style Sheets**.

It is used to control the presentation and layout of HTML elements,
including colors, spacing, fonts, positioning, backgrounds, and
responsive layouts.

---

### 2. What are the different ways of applying CSS?

There are three common ways:

1. **Inline CSS**
2. **Internal CSS**
3. **External CSS**

Example of inline CSS:

```html
<p style="color: red;">Hello</p>
```

Internal CSS is written inside `<style>`.

External CSS is written in a separate `.css` file and linked to HTML.

---

### 3. What is the difference between inline, internal, and external CSS?

**Inline CSS** is written directly on an HTML element.

**Internal CSS** is written inside a `<style>` element in the HTML
document.

**External CSS** is written in a separate CSS file.

External CSS is generally preferred for larger projects because it
separates styling from HTML and allows styles to be reused.

---

### 4. If multiple CSS rules target the same element, how does the browser decide which rule gets applied?

**CSS Priority**

**Inline CSS > Internal CSS > External CSS**

---

### 5. What is CSS specificity?

Specificity is the mechanism used by CSS to determine which competing
selector has greater priority.

A simplified priority order is:

**ID > class/attribute/pseudo-class > element/pseudo-element**

Inline styles have higher normal author specificity than these
selectors.

---

### 6. Which has higher specificity: ID, class, or element selector?

The order is:

**ID > class > element**

Example:

```css
#box { color: red; }
.box { color: blue; }
p { color: green; }
```

If all three target the same `<p id="box" class="box">`, the ID rule
wins.

---

### 7. What happens when two selectors have the same specificity?

The rule that appears **later in the CSS** generally wins.

```css
p {
    color: red;
}

p {
    color: blue;
}
```

The paragraph becomes blue.

---

### 8. What is the difference between a class selector and an ID selector?

A **class** is intended to be reusable across multiple elements.

An **ID** identifies a particular element and should be unique within
the document.

```css
.box { }
#header { }
```

Class selectors are commonly preferred for reusable styling.

---

### 9. What are CSS combinators?

Combinators describe relationships between elements.

Common combinators include:

- Descendant: space
- Child: `>`
- Adjacent sibling: `+`
- General sibling: `~`

---

### 10. What is the difference between a descendant selector 
(``) and child selector (`>`)

```css
div p
```

selects `<p>` elements that are descendants of a `<div>`, at any nesting
level.

```css
div > p
```

selects only `<p>` elements that are **direct children** of the `<div>`.

---

### 11. What is the difference between adjacent sibling (`+`) and general sibling (`~`)?

`+` selects the **immediately following sibling**.

```css
h1 + p
```

`~` selects **all following siblings** that match.

```css
h1 ~ p
```

---

### 12. What is the difference between a pseudo-class and pseudo-element?

A **pseudo-class** targets a particular state or condition of an
element.

```css
button:hover { }
```

A **pseudo-element** targets a specific part of an element or creates
generated content.

```css
p::first-letter { }
```

---

### 13. What are `:hover`, `:focus`, `:active`, and `:visited` used for?

- `:hover` → Element is being hovered over.
- `:focus` → Element has focus.
- `:active` → Element is being activated.
- `:visited` → Link has previously been visited.

---

### 14. How does `:nth-child()` work?

It selects an element based on its position among its parent’s children.

```css
li:nth-child(2) {
    color: red;
}
```

This targets the second child if it is an `<li>`.

It can also use patterns such as:

```css
li:nth-child(odd) { }
li:nth-child(even) { }
```

---

### 15. What are `::before` and `::after`, and why is the `content` property commonly used with them?

`::before` and `::after` create generated pseudo-elements associated
with an element.

They commonly use `content` to specify what should be generated.

```css
.box::before {
    content: "★";
}
```

---

### 16. What is an attribute selector? Give an example.

An attribute selector selects elements based on their attributes.

```css
input[type="text"] {
    border: 1px solid black;
}
```

This targets `<input>` elements whose `type` attribute is `"text"`.

---

### 17. What are the different ways of specifying colors in CSS?

Common formats include:

- Color names
- HEX
- RGB
- RGBA
- HSL
- HSLA

Example:

```css
color: red;
color: #ff0000;
color: rgb(255, 0, 0);
```

---

### 18. What is the difference between RGB, RGBA, HEX, HSL, and HSLA?

- **RGB** → Red, Green, Blue.
- **RGBA** → RGB plus alpha/transparency.
- **HEX** → Hexadecimal representation of color.
- **HSL** → Hue, Saturation, Lightness.
- **HSLA** → HSL plus alpha.

---

### 19. What does the alpha value represent?

The alpha value controls the **opacity/transparency** of a color.

For example:

```css
background-color: rgba(255, 0, 0, 0.5);
```

The `0.5` represents 50% opacity.

---

### 20. What is the difference between `background-size: cover` and `contain`?

`cover` scales the background image so the entire container is covered,
potentially cropping part of the image.

`contain` scales the image so the entire image fits inside the
container, potentially leaving empty space.

---

### 21. What is the difference between `background-repeat`, `background-position`, and `background-size`?

- `background-repeat` → Controls whether/how the image repeats.
- `background-position` → Controls where the image is positioned.
- `background-size` → Controls the size of the image.

---

### 22. What is a CSS gradient? What is the difference between linear, radial, and conic gradients?

A gradient creates a smooth transition between colors.

- **Linear gradient** → Transition along a line.
- **Radial gradient** → Transition outward from a central point.
- **Conic gradient** → Transition around a center point.

They are commonly used through `background-image`.

---

### 23. What is the CSS box model?

Every HTML element is represented as a rectangular box consisting of:

**Content → Padding → Border → Margin**

The box model determines how the element’s dimensions and surrounding
space are calculated.

---

### 24. Explain the difference between content, padding, border, and margin.

- **Content** → Actual text/image/etc.
- **Padding** → Space between content and border.
- **Border** → Line surrounding padding/content.
- **Margin** → Space outside the border.

---

### 25. What is the difference between padding and margin?

**Padding** creates space **inside** the element, between its content
and border.

**Margin** creates space **outside** the element, beyond its border.

---

### 26. What is `box-sizing`, and what is its default value?

`box-sizing` controls how an element’s declared width and height are
calculated.

The default is:

```css
box-sizing: content-box;
```

With `content-box`, declared `width` and `height` apply to the content
area, while padding and border are added outside those dimensions.

With:

```css
box-sizing: border-box;
```

the declared width/height includes content, padding, and border.

---

### 27. How do you calculate the actual size of an element under the default box model?

With `box-sizing: content-box`:

**Total width = content width + left/right padding + left/right border**

For example:

```css
width: 200px;
padding: 20px;
border: 5px solid;
```

Total width:

`200 + 20 + 20 + 5 + 5 = 250px`

Margin is outside the element and is not included in this box width.

---

### 28. What is the difference between border and outline?

A **border** is part of the element’s box model.

An **outline** is drawn outside the border and generally does not take
up layout space.

---

### 29. How does padding/margin shorthand work with 1, 2, 3, and 4 values?

The values follow **top → right → bottom → left**.

```css
padding: 10px;
```

All four sides.

```css
padding: 10px 20px;
```

Top/bottom = 10px, left/right = 20px.

```css
padding: 10px 20px 30px;
```

Top = 10px, left/right = 20px, bottom = 30px.

```css
padding: 10px 20px 30px 40px;
```

Top = 10px, right = 20px, bottom = 30px, left = 40px.

The same pattern applies to margin.

---

### 30. What does `margin: auto` do?

`auto` allows the browser to calculate the margin automatically.

A common use is horizontal centering of a block element with a defined
width:

```css
.box {
    width: 300px;
    margin: 0 auto;
}
```

---

### 31. What is the difference between `font-size`, `font-weight`, `font-style`, and `font-family`?

- `font-size` → Size of the text.
- `font-weight` → Thickness/boldness.
- `font-style` → Normal/italic/oblique style.
- `font-family` → Typeface used for the text.

---

### 32. What is the difference between `letter-spacing`, `word-spacing`, and `line-height`?

- `letter-spacing` → Space between characters.
- `word-spacing` → Space between words.
- `line-height` → Vertical distance between lines of text.

---

### 33. What does the `overflow` property do?

It controls what happens when content is larger than an element’s box.

Common values include:

```css
overflow: visible;
overflow: hidden;
overflow: scroll;
overflow: auto;
```

---

### 34. What is the difference between `overflow: hidden`, `scroll`, and `auto`?

- `hidden` → Excess content is clipped.
- `scroll` → Scrollbars are provided for scrolling.
- `auto` → Scrollbars are provided when necessary.

---

### 35. What is Flexbox, and why is it used?

Flexbox is a CSS layout system designed to arrange elements efficiently
along a **one-dimensional axis**.

It makes alignment, spacing, ordering, and responsive arrangement of
elements easier.

---

### 36. What are the main axis and cross axis in Flexbox?

The **main axis** is determined by `flex-direction`.

The **cross axis** runs perpendicular to the main axis.

For the default:

```css
flex-direction: row;
```

the main axis is horizontal and the cross axis is vertical.

---

### 37. What is the difference between `justify-content` and `align-items`?

`justify-content` controls alignment/distribution along the **main
axis**.

`align-items` controls alignment along the **cross axis**.

For the default `flex-direction: row`:

- `justify-content` → horizontal
- `align-items` → vertical

---

### 38. What is the difference between `align-items` and `align-content`?

`align-items` aligns flex items along the cross axis within a flex line.

`align-content` controls the spacing/alignment **between multiple flex
lines** when wrapping creates multiple lines.

`align-content` generally has no visible effect when there is only one
flex line.

---

### 39. What does `flex-direction` do?

It determines the direction of the main axis.

Common values:

```css
flex-direction: row;
flex-direction: row-reverse;
flex-direction: column;
flex-direction: column-reverse;
```

---

### 40. What does `flex-wrap` do?

It determines whether flex items must remain on one line or can move
onto multiple lines.

```css
flex-wrap: nowrap;
flex-wrap: wrap;
```

With `wrap`, items can move to additional lines when there isn’t enough
space.

---

### 41. What are `flex-grow`, `flex-shrink`, and `flex-basis`?

- `flex-grow` → Controls how an item can grow when extra space exists.
- `flex-shrink` → Controls how an item can shrink when space is
insufficient.
- `flex-basis` → Defines the item’s initial/main-size basis before
remaining space is distributed.

---

### 42. What does the `order` property do in Flexbox?

`order` controls the visual ordering of flex items.

```css
.item1 { order: 2; }
.item2 { order: 1; }
```

`item2` will appear before `item1` visually.

The default order is `0`.

---

### 43. How do you center an element horizontally and vertically using Flexbox?

```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
}
```

For the default row direction, this centers the item horizontally and
vertically.

---

### 44. What is the difference between `px`, `%`, `em`, `rem`, `vh`, and `vw`?

- `px` → CSS pixel unit.
- `%` → Relative to the relevant containing/reference dimension.
- `em` → Relative to the element’s font size for font sizing, and
generally to the relevant computed font size for other properties.
- `rem` → Relative to the root element’s font size.
- `vh` → Relative to viewport height.
- `vw` → Relative to viewport width.

---

### 45. What is the difference between `em` and `rem`?

`em` is relative to the relevant element’s font size and can compound
through nested elements.

`rem` is relative to the root (`html`) element’s font size, making it
more predictable across nesting.

---

### 46. What is the difference between `vh` and `vw`?

`vh` is based on the viewport’s height.

`vw` is based on the viewport’s width.

For example:

```css
height: 100vh;
width: 100vw;
```

---

### 47. Explain the different CSS `position` values: `static`, `relative`, `absolute`, `fixed`, and `sticky`.

- `static` → Normal document flow; offset properties do not reposition
it.
- `relative` → Remains in normal flow but can be visually offset from
its normal position.
- `absolute` → Removed from normal flow and positioned relative to its
containing block.
- `fixed` → Positioned relative to the viewport in the usual case and
stays fixed while scrolling.
- `sticky` → Behaves like a relatively positioned element until a
scroll threshold is reached, then sticks within its containing area.

---

### 48. What is the difference between relative and absolute positioning?

A relatively positioned element remains in normal document flow.

An absolutely positioned element is removed from normal flow and
positioned using its containing block.

---

### 49. Relative to what is an absolutely positioned element positioned?

It is positioned relative to its **containing block**.

A common case is an absolutely positioned child inside a parent with:

```css
.parent {
    position: relative;
}
```

Then the child’s `top`, `left`, etc. are calculated relative to that
containing block.

---

### 50. What is the difference between `absolute`, `fixed`, and `sticky`?

- **Absolute** → Positioned relative to its containing block and
removed from normal flow.
- **Fixed** → Typically positioned relative to the viewport and
remains fixed during scrolling.
- **Sticky** → Participates in normal flow and becomes stuck relative
to its scrolling container after reaching a specified offset.

---

### 51. What do `top`, `right`, `bottom`, and `left` do?

They specify offsets for positioned elements.

Example:

```css
.box {
    position: absolute;
    top: 20px;
    left: 30px;
}
```

The exact reference depends on the element’s positioning context.

---

### 52. What is `z-index`, and when does it work?

`z-index` controls the stacking order of overlapping elements.

A larger stacking value generally places an element above another within
the relevant stacking context.

It is most commonly used with positioned elements, although modern CSS
can create other stacking contexts as well.

---

### 53. What is the difference between `transform: translate()` and changing an element’s position?

`transform: translate()` visually moves an element without changing its
original position in normal document flow.

Positioning with `top`, `left`, etc. changes the positioned element
according to the rules of its positioning scheme.

Transforms are commonly useful for visual movement and animation.

---

### 54. What do `translate()`, `scale()`, `rotate()`, and `skew()` do?

- `translate()` → Moves an element.
- `scale()` → Enlarges or reduces it.
- `rotate()` → Rotates it.
- `skew()` → Slants/distorts it along an axis.

Example:

```css
transform: translate(20px, 10px);
transform: scale(1.2);
transform: rotate(45deg);
transform: skew(20deg);
```

---

### 55. What is a CSS transition?

A transition smoothly interpolates a CSS property from one state to
another over a specified duration.

Example:

```css
button {
    transition: background-color 0.3s;
}

button:hover {
    background-color: black;
}
```

---

### 56. What are `transition-duration`, `transition-delay`, `transition-property`, and `transition-timing-function`?

- `transition-property` → Which property should transition.
- `transition-duration` → How long the transition takes.
- `transition-delay` → How long to wait before starting.
- `transition-timing-function` → Controls the rate at which the
transition progresses.

---

### 57. What is the difference between a transition and an animation?

A **transition** generally describes a smooth change between two states,
often triggered by something such as `:hover`.

An **animation** can define multiple stages using `@keyframes` and can
run independently of user interaction.

---

### 58. What are `@keyframes`?

`@keyframes` defines the intermediate stages of a CSS animation.

Example:

```css
@keyframes move {
    from {
        transform: translateX(0);
    }

    to {
        transform: translateX(100px);
    }
}
```

---

### 59. What do `animation-duration`, `animation-iteration-count`, `animation-direction`, and `animation-delay` do?

- `animation-duration` → How long one animation cycle takes.
- `animation-iteration-count` → How many times it runs.
- `animation-direction` → Controls the direction of successive cycles.
- `animation-delay` → Delays the start of the animation.

---

### 60. How would you create a continuously running animation using CSS?

Use `animation-iteration-count: infinite`.

```css
.box {
    animation: rotateBox 2s linear infinite;
}

@keyframes rotateBox {
    from {
        transform: rotate(0deg);
    }

    to {
        transform: rotate(360deg);
    }
}
```

---