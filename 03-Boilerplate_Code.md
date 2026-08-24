# HTML Boilerplate Code

An **HTML Boilerplate** is the basic structure of every HTML document. It contains the essential tags required for a web browser to correctly understand and display a webpage.

Every HTML file should begin with this basic template.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>

</body>
</html>
```

### **`<!DOCTYPE html>`**

The `<!DOCTYPE html>` declaration tells the browser that the document is written in **HTML5**, which is the latest version of HTML. It ensures that the browser renders the webpage using the latest HTML standards.

### **`<html>`**

The `<html>` tag is the **root element** of an HTML document. All other HTML elements are placed inside this tag. The `lang` attribute specifies the language of the webpage, i.e
 `<html lang="en">` Here, `lang="en"` indicates that the content of the webpage is in **English**.

### **`<head>`**

The `<head>` section contains information **about the webpage** that is not displayed directly in the browser. It includes metadata, the page title, links to CSS files, JavaScript files, icons, and other settings.

### **`<meta charset="UTF-8">`**

The `charset` attribute specifies the character encoding used by the webpage. `UTF-8` is the most commonly used character encoding because it supports almost all languages and special characters.

### **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**

The viewport meta tag helps make the webpage **responsive** on different devices such as desktops, tablets, and mobile phones.

- `width=device-width` sets the webpage width equal to the width of the device.
- `initial-scale=1.0` sets the initial zoom level to 100%.

### **`<title>`**

The `<title>` tag specifies the title of the webpage. The title appears on the **browser tab**, bookmarks, and search engine results.

### **`<body>`**

The `<body>` tag contains all the content that is visible to the user in the browser, such as text, images, headings, tables, forms, videos, and links. Everything that should appear on the webpage is placed inside the `<body>` tag.

### **Complete Example**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Boilerplate</title>
</head>

<body>
    <h1>Welcome to HTML</h1>
    <p>This is my first webpage.</p>
</body>
</html>
```

### **Output**

```
Browser Tab:
HTML Boilerplate

-------------------------------------
| Welcome to HTML                   |
| This is my first webpage.         |
-------------------------------------
```