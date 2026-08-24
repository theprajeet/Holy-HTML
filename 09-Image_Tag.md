# Image Tag

## **Image (`<img>`) Tag**

The `<img>` tag is used to display images on a webpage. It is an **unpaired (empty)** tag.

**Syntax:**

```html
<img src="image.jpg" alt="Description">
```

### **Relative Path**

A **Relative Path** specifies the location of an image relative to the current HTML file.

**Example:**

```html
<img src="images/nature.jpg" alt="Nature">
```

If the HTML file and the `images` folder are in the same project, the browser loads the image from that folder.

### **Absolute Path**

An **Absolute Path** specifies the complete URL or full path of an image.

**Example:**

```html
<img src="https://example.com/images/nature.jpg" alt="Nature">
```

The browser loads the image directly from the specified website.

### **Attributes of the `<img>` Tag**

#### **`src`**

Specifies the path or URL of the image.

**Example:**

```html
<img src="nature.jpg">
```

#### **`alt`**

Provides alternative text if the image cannot be displayed.

**Example:**

```html
<img src="nature.jpg" alt="Nature Image">
```

#### **`width`**

Specifies the width of the image.

**Example:**

```html
<img src="nature.jpg" width="300">
```

#### **`height`**

Specifies the height of the image.

**Example:**

```html
<img src="nature.jpg" height="200">
```

#### **`title`**

Displays a tooltip when the mouse pointer is placed over the image.

**Example:**

```html
<img src="nature.jpg" title="Beautiful Nature">
```

### **Complete Example of Image Tag**

```html
<img
    src="images/nature.jpg"
    alt="Nature Image"
    width="300"
    height="200"
    title="Beautiful Nature">
```

### **Example of Using the `alt` Attribute**

The `alt` (alternative text) attribute displays a description of the image if the image cannot be loaded. It is also used by screen readers to improve accessibility for visually impaired users.

**Example:**

```html
<img src="nature.jpg" alt="A beautiful mountain with a lake" width="300">
```

**If the image is available:**

- The browser displays the image.

**If the image is missing or the file path is incorrect:**

- The browser displays the text:

```
A beautiful mountain with a lake
```

For example, if the image file does not exist:

```html
<img src="missing-image.jpg" alt="A beautiful mountain with a lake">
```

Since `missing-image.jpg` cannot be found, the browser displays the alternative text **“A beautiful mountain with a lake”** instead of the image.

---