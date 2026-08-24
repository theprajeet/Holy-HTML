# HTML Question Bank

## 1. What is HTML, and what are the features of HTML?

### **HTML**

HTML (HyperText Markup Language) was created by Tim Berners-Lee in 1991 as a standard for creating web pages. **It's a markup language used to structure content on the web, it uses tags and elements to define content like text, links, and images for web browsers**. In layman's terms, HTML is like the skeleton of a website. It's a set of instructions that tells a web browser how to display text, images, videos, and other elements on a webpage. 

### **Features of HTML**

- It is platform-independent. For example, Chrome displays the same pages identically across different operating systems such as Mac, Linux, and Windows.
- Images, videos, and audio can be added to a web page (For example - YouTube shows videos on their website).
- HTML is a markup language and not a programming language.
- It can be integrated with other languages like CSS, JavaScript, etc. to show interactive (or dynamic) web pages.

The term 'Hypertext Markup Language' is composed of two main words: 'hypertext' and 'markup language.' 'Hypertext' refers to the linking of text with other documents wile Markup Language is a language used to define the structure, organization, and presentation of content using tags. It tells the browser what each piece of content is (such as a heading, paragraph, image, or table) but does not perform calculations or make decisions. Unlike a Programming Language, which contains logic, variables, loops, conditions, and functions to perform tasks and solve problems, a markup language is only used to describe and structure content.

---

## 2. How does the web work?

When a user wants to access a website, the following process takes place:

1. The user opens a web browser (such as Chrome, Firefox, or Edge).
2. The user enters a website name (for example, `www.google.com`) into the address bar.
3. The browser attempts to connect to the server that hosts the website.
4. However, servers do not understand human-readable domain names. They communicate using **IP (Internet Protocol) addresses**.
5. To convert the human-readable domain name into an IP address, the browser contacts the **DNS (Domain Name System)**.
6. DNS translates the domain name into its corresponding IP address.
7. Using the IP address, the browser connects to the appropriate web server.
8. The web server processes the request and sends the requested web page back to the browser.
9. Finally, the browser displays the web page to the user.
    - Web browsers perform two main tasks: parsing and rendering.
    - During the parsing stage, the browser receives raw bytes, which are converted into characters. These characters are then converted into tokens, which in turn are transformed into nodes. These nodes are organized into a tree-like data structure known as the DOM (Document Object Model).
    - Once the DOM tree is constructed, the browser moves on to the rendering stage. At this point, each node in the DOM tree is rendered and displayed on the screen.

---

## 3.  3-Tier Architecture and N-Tier Architecture

A **3-Tier Architecture** is a software architecture in which an application is divided into **three separate layers (tiers)**. Each layer has a specific responsibility, making the application easier to develop, maintain, scale, and debug.

The three layers communicate with each other, but each layer performs its own dedicated task.

### **1. Presentation Tier (Client Layer)**

This is the layer that users interact with. It is responsible for displaying information and collecting input from the user.

**Responsibilities:**

- Displays the User Interface (UI)
- Accepts user input
- Sends requests to the application layer
- Displays the response received from the server

**Examples:** HTML, CSS, JavaScript, React, Angular, Vue.js

### **2. Application Tier (Business Logic Layer)**

This layer contains the application’s business logic. It receives requests from the presentation layer, processes them, performs validations, communicates with the database if necessary, and returns the appropriate response.

**Responsibilities:**

- Processes user requests
- Implements business logic
- Validates user input
- Communicates with the database layer

**Examples:** Node.js, Express.js, Java, Spring Boot, Python (Django/Flask), ASP.NET

### **3. Data Tier (Database Layer)**

This layer is responsible for storing, retrieving, updating, and deleting data. It communicates only with the application layer.

**Responsibilities:**

- Stores application data
- Retrieves data
- Updates and deletes records
- Ensures data security and integrity

**Examples:** MySQL, PostgreSQL, MongoDB, Oracle, SQL Server

### **Working of 3-Tier Architecture**

1. The user interacts with the **Presentation Layer**.
2. The request is sent to the **Application Layer**.
3. The Application Layer processes the request and communicates with the **Database Layer** if required.
4. The Database returns the requested data.
5. The Application Layer processes the response and sends it back to the Presentation Layer.
6. The browser displays the result to the user.

---

# **N-Tier Architecture**

An **N-Tier Architecture** is an extension of the 3-Tier Architecture. Here, the application is divided into **multiple layers (N layers)** instead of only three. Each layer is responsible for a specific functionality, making large applications more modular, scalable, secure, and easier to maintain.

The letter **‘N’** represents **any number of layers**.

### **Common Layers in an N-Tier Architecture**

- Presentation Layer (UI)
- API Layer
- Authentication Layer
- Business Logic Layer
- Service Layer
- Data Access Layer
- Database Layer
- Cache Layer

The exact number of layers depends on the application’s complexity.

### **Advantages of N-Tier Architecture**

- Better scalability
- Easier maintenance
- Improved security
- Code reusability
- Easier testing and debugging
- Different teams can work on different layers independently

---

# 4. HTML Tags

### **HTML Tags**

HTML tags are the markers that define the start and end of an element. They are wrapped in angle brackets, like **`<p>`** and **`</p>`**.

### **HTML Elements**

An HTML element includes an opening tag, content, and a closing tag, forming a complete set. For example, **`<p>This is a paragraph.</p>`**.

If you want to build a beautiful website, tags are essential elements that help you achieve that.

An HTML tag acts as a container for content or other HTML tags. Tags are words enclosed within **`<`** and **`>`** angle brackets.

They serve as keywords that instruct the web browser on how to format and display the content.

### **Commonly used tags in HTML**

Here are some commonly used tags in HTML. These are the only tags used 70% of the time.

### **Document Structure Tags**

1. **`<DOCTYPE html>`**: Specifies the document type.
2. **`<html>`**: Encloses the entire HTML document.
3. **`<head>`**: Contains meta-information and links to scripts and stylesheets.
4. **`<body>`**: Contains the content of the web page.

### **Metadata Tags**

1. **`<title>`**: Sets the title of the web page.
2. **`<meta>`**: Provides metadata such as character set, author, and viewport settings.
3. **`<link>`**: Links external resources like stylesheets.

### **Text Formatting Tags**

1. **`<p>`**: Paragraph.
2. **`<h1>`**, **`<h2>`**, **`<h3>`**, **`<h4>`**, **`<h5>`**, **`<h6>`**: Headings.
3. **`<strong>`**: Strong emphasis (typically bold).
4. **`<em>`**: Emphasis (typically italic).
5. **`<br>`**: Line break.
6. **`<hr>`**: Horizontal rule.

### **List Tags**

1. **`<ul>`**: Unordered list.
2. **`<ol>`**: Ordered list.
3. **`<li>`**: List item.

### **Hyperlink and Media Tags**

1. **`<a>`**: Anchor (used for links).
2. **`<img>`**: Image.
3. **`<audio>`**: Audio content.
4. **`<video>`**: Video content.

### **Form Tags**

1. **`<form>`**: Form.
2. **`<input>`**: Input field.
3. **`<textarea>`**: Text area.
4. **`<button>`**: Button.
5. **`<select>`**: Dropdown list.
6. **`<option>`**: Options within a **`<select>`** or **`<datalist>`**.

### **Table Tags**

1. **`<table>`**: Table.
2. **`<tr>`**: Table row.
3. **`<td>`**: Table data cell.
4. **`<th>`**: Table header cell.
5. **`<thead>`**: Table header group.
6. **`<tbody>`**: Table body group.
7. **`<tfoot>`**: Table footer group.

### **Semantic Tags**

1. **`<header>`**: Header section.
2. **`<footer>`**: Footer section.
3. **`<article>`**: Article.
4. **`<section>`**: Section.
5. **`<nav>`**: Navigation.
6. **`<aside>`**: Sidebar content.

## **Paired and Unpaired HTML Tags**

Well, that was a really long list. Don't worry, we will study these in detail. In HTML, tags can be broadly categorized into two types:

### **1. Paired Tags (Container Tags)**

These are tags that come in pairs, consisting of an opening tag and a corresponding closing tag. The content goes between these two tags.

- **Opening Tag**: The opening tag starts with **`<`** and ends with **`>`**. For example, **`<p>`**.
- **Closing Tag**: The closing tag also starts with **`<`** but includes a forward slash **`/`** before the tag name, and ends with **`>`**. For example, **`</p>`**.

### **Examples:**

- Paragraphs: **`<p>This is a paragraph.</p>`**
- Headings: **`<h1>This is a heading.</h1>`**

### **2. Unpaired Tags (Self-Closing Tags or Stand-Alone Tags)**

These are tags that don't require a closing tag. They are self-contained, encapsulating all the information within a single tag.

- **Self-Closing Tag**: A self-closing tag starts with **`<`** and ends with **`/>`** (though the **`/`** is optional in HTML5). For example, **`<img />`** or **`<br>`**.

**Note:** Later if you happen to use React or a framework like Next.js, you will have to close the tag like this **`<br/>`** **`<hr/>`**. So it is better to cultivate the habit!

### **Examples of self-closing tags:**

- Line Break: **`<br/>`**
- Horizontal Rule: **`<hr/>`**
- Image: **`<img src="image.jpg" alt="An example image"/>`**

---

# 5. Block Level Element and Inline Element

HTML elements are broadly classified into **Block-Level Elements** and **Inline Elements** based on how they are displayed on a web page.

A **Block-Level Element** always starts on a new line and occupies the full available width of its parent container by default. In contrast, an **Inline Element** does not start on a new line and only occupies as much width as its content requires.

```jsx
Example

<div>This is a block-level element.</div>
<div>This starts on the next line.</div>

<span>This is an inline element.</span>
<span>This appears on the same line.</span>
```

```jsx
Output

This is a block-level element.
This starts on the next line.

This is an inline element. This appears on the same line.
```

---

# 6. HTML Attributes

HTML attributes are used to define the characteristics of an HTML element. They are placed within the element's opening tag and consist of two parts: the **name** and the **value**.

- **Name**: Specifies the property for that element.
- **Value**: Sets the value of that property for the element.

### **Types of HTML Attributes**

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

`<p id="html">This is an HTML tutorial</p><p id="python">This is a Python tutorial</p>`

In this example, the ID attribute helps to distinguish between two paragraphs by having different values: "html" and "python".

### **Class Attribute**

The class attribute is used to associate an HTML element with a particular class, typically for styling or JavaScript manipulation. Unlike the ID attribute, the class attribute is not unique, and multiple elements can share the same class.

### **Title Attribute**

The title attribute provides additional information about an element and is often displayed as a tooltip when the mouse hovers over it.

Example:

`<h4 title="hello, motto">Title attribute</h4>`

### **Style Attribute**

The style attribute allows for inline styling of HTML elements. It is used in conjunction with CSS properties to directly style individual elements within the HTML code.

### **Case Sensitivity**

The HTML standard is flexible about the case of attribute names, allowing them to be written in either uppercase or lowercase, such as "title" or "TITLE." However, for best practices and compatibility with stricter document types like XHTML, the W3C recommends using lowercase attributes.

---

# 7. Write the basic syntax for the anchor and image tags.

#### **Basic Syntax of Anchor (`<a>`) Tag**

The **Anchor (`<a>`) tag** is used to create hyperlinks that allow users to navigate from one web page to another, open files, send emails, or jump to different sections of the same page.

**Syntax:**

```html
<a href="URL">Link Text</a>
```

**Example:**

```html
<a href="https://www.google.com">Visit Google</a>
```

#### **Basic Syntax of Image (`<img>`) Tag**

The **Image (`<img>`) tag** is used to display images on a web page. It is an **empty (self-closing) tag**, meaning it does not have a closing tag.

**Syntax:**

```html
<img src="image_path" alt="Image Description">
```

**Example:**

```html
<img src="nature.jpg" alt="Beautiful Nature">
```

**Common Attributes:**

- `src` – Specifies the path or URL of the image.
- `alt` – Provides alternative text if the image cannot be displayed.
- `width` – Sets the width of the image.
- `height` – Sets the height of the image.

**Example with Width and Height:**

```html
<img src="nature.jpg" alt="Beautiful Nature" width="300" height="200">
```

---

# 8. What are table, th, td, tr, cell spacing, cell padding?

### HTML Table

A **Table** in HTML is used to organize and display data in the form of **rows and columns**. It is created using the `<table>` tag, while other tags like `<tr>`, `<th>`, and `<td>` are used to define its structure.

---

### **`<table>` Tag**

The `<table>` tag is the container that defines the entire table. All rows, columns, headers, and data cells are placed inside this tag.

**Syntax:**

```html
<table>
    ...
</table>
```

### **`<tr>` (Table Row)**

The `<tr>` tag is used to create a **row** in a table. Every row contains one or more header cells (`<th>`) or data cells (`<td>`).

**Syntax:**

```html
<tr>
    ...
</tr>
```

### **`<th>` (Table Header)**

The `<th>` tag is used to create a **header cell** in a table. By default, the text inside a `<th>` is **bold** and **center-aligned**.

It is generally used for column headings or row headings.

**Syntax:**

```html
<th>Header</th>
```

### **`<td>` (Table Data)**

The `<td>` tag is used to create a **data cell** in a table. It contains the actual information or values.

**Syntax:**

```html
<td>Data</td>
```

### **Cell Spacing**

**Cell Spacing** is the amount of **space between two adjacent table cells**. It creates a gap between the borders of neighboring cells.

It is specified using the `cellspacing` attribute of the `<table>` tag.

**Syntax:**

```html
<table cellspacing="10">
```

**Example:** If `cellspacing="10"`, there will be a **10-pixel gap** between each table cell.

**Note:** The `cellspacing` attribute is deprecated in HTML5. In modern HTML, CSS (`border-spacing`) is used instead.

### **Cell Padding**

**Cell Padding** is the amount of **space between the content of a cell and its border**. It provides inner spacing, making the content appear away from the cell’s edges.

It is specified using the `cellpadding` attribute of the `<table>` tag.

**Syntax:**

```html
<table cellpadding="10">
```

**Example:** If `cellpadding="10"`, there will be **10 pixels of space** between the cell content and the cell border.

**Note:** The `cellpadding` attribute is deprecated in HTML5. In modern HTML, CSS (`padding`) is used instead.

### **Example of an HTML Table**

```html
<table border="1" cellspacing="5" cellpadding="10">
    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>

    <tr>
        <td>Rahul</td>
        <td>21</td>
    </tr>

    <tr>
        <td>Priya</td>
        <td>20</td>
    </tr>
</table>
```

### **Output**

| **Name** | **Age** |
| --- | --- |
| Rahul | 21 |
| Priya | 20 |

---

# 9. A HTML Table

### HTML Code

```jsx
<!DOCTYPE html>
<html>
<head>
    <title>Table Example</title>
</head>
<body>

<table border="1" cellspacing="5" cellpadding="10">

    <tr>
        <th colspan="4">Student Details</th>
    </tr>

    <tr>
        <th>Roll No</th>
        <th>Name</th>
        <th>Department</th>
        <th>Semester</th>
    </tr>

    <tr>
        <td rowspan="2">101</td>
        <td>Rahul</td>
        <td>CSE</td>
        <td>5</td>
    </tr>

    <tr>
        <td>Priya</td>
        <td>ISE</td>
        <td>5</td>
    </tr>

</table>

</body>
</html>
```

### Output

```jsx
OUTPUT

+-----------------------------------------------+
|               Student Details                 |
+----------+------------+--------------+--------+
| Roll No  | Name       | Department   | Sem    |
+----------+------------+--------------+--------+
|          | Rahul      | CSE          | 5      |
|   101    +------------+--------------+--------+
|          | Priya      | ISE          | 5      |
+----------+------------+--------------+--------+
```

---

# 10. A HTML Lists

### HTML Code

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

# **11. HTML Media Tags**

HTML provides media tags to display images, play audio, play videos, and embed external content such as web pages or PDF files. The most commonly used media tags are `<img>`, `<audio>`, `<video>`, `<source>`, and `<iframe>`.

The following example demonstrates all of these tags.

### **HTML Code**

```html
<!DOCTYPE html>
<html>
<head>
    <title>HTML Media Tags</title>
</head>
<body>

    <h2>Image</h2>
    <img src="nature.jpg" alt="Nature Image" width="300" height="200">

    <h2>Audio</h2>
    <audio controls>
        <source src="song.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>

    <h2>Video</h2>
    <video width="400" height="250" controls>
        <source src="video.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>

    <h2>Embedded Web Page</h2>
    <iframe src="https://www.wikipedia.org"
            width="500"
            height="300">
    </iframe>

</body>
</html>
```

### **Output**

```
Image
+---------------------------+
|                           |
|       Nature Image        |
|                           |
+---------------------------+

Audio
▶️  ───────────────  🔊

Video
+--------------------------------------+
|                                      |
|            ▶ Video Player            |
|                                      |
+--------------------------------------+

Embedded Web Page
+--------------------------------------+
|                                      |
|         Wikipedia Website            |
|                                      |
+--------------------------------------+
```

### **Common Attributes**

### **`<img>`**

`src`, `alt`, `width`, `height`

### **`<audio>`**

`controls`, `autoplay`, `loop`, `muted`

### **`<video>`**

`controls`, `autoplay`, `loop`, `muted`, `width`, `height`, `poster`

### **`<source>`**

`src`, `type`

### **`<iframe>`**

`src`, `width`, `height`, `title`

---

# 12. HTML Form

HTML forms are used to collect user input. The `<form>` tag acts as the container for various input fields such as text boxes, password fields, radio buttons, checkboxes, email fields, date pickers, and buttons.

The following example includes all the requested fields.

### **HTML Code**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Registration Form</title>
</head>
<body>

    <h2>Registration Form</h2>

    <form>

        <label>First Name:</label>
        <input type="text" name="firstname"><br><br>

        <label>Last Name:</label>
        <input type="text" name="lastname"><br><br>

        <label>Username:</label>
        <input type="text" name="username"><br><br>

        <label>Password:</label>
        <input type="password" name="password"><br><br>

        <label>Email:</label>
        <input type="email" name="email"><br><br>

        <label>Date of Birth:</label>
        <input type="date" name="dob"><br><br>

        <label>Gender:</label>
        <input type="radio" name="gender" value="Male"> Male
        <input type="radio" name="gender" value="Female"> Female
        <input type="radio" name="gender" value="Other"> Other
        <br><br>

        <label>Skills:</label><br>
        <input type="checkbox" name="skills" value="HTML"> HTML
        <input type="checkbox" name="skills" value="CSS"> CSS
        <input type="checkbox" name="skills" value="JavaScript"> JavaScript
        <input type="checkbox" name="skills" value="React"> React
        <br><br>

        <input type="submit" value="Create">
        <input type="reset" value="Cancel">

    </form>

</body>
</html>
```

### **Output**

```
                Registration Form

First Name:     ______________________

Last Name:      ______________________

Username:       ______________________

Password:       ______________________

Email:          ______________________

Date of Birth:  [  dd/mm/yyyy  ]

Gender:         ( ) Male   ( ) Female   ( ) Other

Skills:
                [ ] HTML
                [ ] CSS
                [ ] JavaScript
                [ ] React

              [ Create ]   [ Cancel ]
             
```

---

# 13. Semantic Tags

**Semantic Tags** are HTML tags that clearly describe the **meaning and purpose of the content** they contain. They make the structure of a web page easier for developers, browsers, and search engines to understand.

Unlike non-semantic tags such as `<div>` and `<span>`, semantic tags indicate what kind of content they hold, improving **readability, accessibility, SEO (Search Engine Optimization), and code maintenance**.

### **Common Semantic Tags**

- `<header>` – Defines the header section of a webpage or a section.
- `<nav>` – Defines a navigation menu containing links.
- `<main>` – Represents the main content of the webpage.
- `<section>` – Defines a thematic section of related content.
- `<article>` – Represents independent, self-contained content such as a blog post or news article.
- `<aside>` – Contains content related to the main content, such as sidebars or advertisements.
- `<footer>` – Defines the footer section of a webpage or a section.
- `<figure>` – Groups media content such as images, diagrams, or illustrations.
- `<figcaption>` – Provides a caption for a `<figure>` element.
- `<details>` – Creates a collapsible section that users can expand or collapse.
- `<summary>` – Defines the visible heading for a `<details>` element.
- `<time>` – Represents a specific date or time.
- `<address>` – Contains contact information for the author or organization.

### **Benefits of Semantic Tags**

- Improve code readability.
- Enhance accessibility for screen readers.
- Help search engines understand the webpage structure (better SEO).
- Make webpages easier to maintain and debug.
- Provide a meaningful structure to the content.

### **Examples of Semantic Tags**

`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`, `<figure>`, `<figcaption>`, `<details>`, `<summary>`, `<time>`, `<address>`

---

# 14. HTML 5 vs HTML 4

HTML4 and HTML5 are versions of the HyperText Markup Language used to create web pages. **HTML5** is the latest version and introduces many new features such as semantic elements, multimedia support, improved forms, and better performance, making web development easier and more efficient than HTML4.

| **HTML4** | **HTML5** |
| --- | --- |
| Introduced in **1997**. | Introduced in **2014** as the latest standard. |
| Does not have semantic tags. | Introduces semantic tags like `<header>`, `<nav>`, `<section>`, `<article>`, `<footer>`. |
| Multimedia requires external plugins like Flash. | Supports multimedia using `<audio>` and `<video>` without plugins. |
| Limited support for form input types. | Provides new input types such as `email`, `date`, `number`, `range`, `color`, `url`, etc. |
| Does not support graphics directly. | Supports graphics using `<canvas>` and SVG. |
| Limited support for offline storage. | Supports local storage and session storage. |
| Simpler APIs and fewer browser features. | Provides APIs such as Geolocation, Drag & Drop, Web Storage, Web Workers, and WebSockets. |
| Longer and more complex DOCTYPE declaration. | Uses a simple DOCTYPE declaration: `<!DOCTYPE html>`. |
| Less SEO-friendly due to lack of semantic structure. | More SEO-friendly because of semantic elements. |
| Lower accessibility support. | Better accessibility for screen readers and assistive technologies. |

---

# 15. Web Page, Web Server and Website

A **Web Page** is a single HTML document displayed in a browser. A **Website** is a collection of related web pages under a single domain name. A **Web Server** is a software or computer system that stores websites, processes user requests, and delivers web pages to users over the internet.

| **Web Page** | **Website** | **Web Server** |
| --- | --- | --- |
| A single HTML document displayed in a browser. | A collection of related web pages. | A software or computer system that stores and serves websites. |
| It is the smallest unit of a website. | It consists of multiple web pages connected through hyperlinks. | It receives requests from clients (browsers) and sends the requested web pages. |
| Has its own unique URL. | Has a single domain name containing multiple URLs. | Identified by an IP address and domain name. |
| Used to display specific information. | Used to provide complete information or services. | Used to host websites and manage client requests. |
| Cannot exist independently as a complete website. | Can contain hundreds or thousands of web pages. | Can host one or multiple websites. |
| Created using HTML, CSS, and JavaScript. | Built using multiple web technologies. | Runs web server software such as Apache, Nginx, or IIS. |

## **Examples**

- **Web Page:** Home Page, About Us Page, Contact Page, Login Page
- **Website:** Google, Amazon, Wikipedia, Flipkart
- **Web Server:** Apache HTTP Server, Nginx, Microsoft IIS, Node.js (Express.js)

---