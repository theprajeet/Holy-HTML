# Introduction

## 3-Tier Architecture and N-Tier Architecture

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

## **N-Tier Architecture**

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
- Different teams can work on different layers independently.

---

## How Does a Browser Work?

### **How a User Accesses a Website**

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

---

### **DNS (Domain Name System)**

**Definition:**

DNS (Domain Name System) is a system that converts a human-readable domain name into its corresponding IP address so that the browser can communicate with the correct server.

**Example:**

- Domain Name: `www.google.com`
- IP Address: `142.250.183.110` (example)

Without DNS, users would have to remember numerical IP addresses instead of simple website names.

---

### **IP Address (Internet Protocol Address)**

**Definition:**

An IP (Internet Protocol) Address is a unique numerical address assigned to every device connected to the internet. It helps identify the device and enables communication between computers over the internet.

**Example:**

- `192.168.1.1`
- `142.250.183.110`

Every website hosted on the internet has an IP address that allows browsers to locate its server.

---

### **Types of Web Applications**

There are two types of web applications:

1. Static Web Applications
2. Dynamic Web Applications

#### **1. Static Web Applications**

**Definition:**

A Static Web Application is a website whose content remains the same for every user. The server simply sends pre-written HTML, CSS, and JavaScript files to the browser without modifying the content.

#### **Characteristics**

- Content is fixed and does not change frequently.
- Same content is displayed to every user.
- No database is required.
- Faster because the server only serves files.
- Easier to develop and host.
- Mainly built using HTML, CSS, and JavaScript.

Examples - Personal Portfolio Website, Company Landing Page, Resume Website, Documentation Website

#### **2. Dynamic Web Applications**

**Definition:**

A Dynamic Web Application generates content based on user requests. The server processes the request, interacts with a database if required, and sends customized content to the user.

#### **Characteristics**

- Content changes according to the user or request.
- Uses a backend server and a database.
- Users can log in, register, update information, and interact with the application.
- More complex than static websites.
- Suitable for applications requiring real-time or personalized data.

**Examples -** Facebook, Instagram, YouTube, Amazon, Flipkart, Gmail

---

## **Web Page vs Website vs Web Server**

### Web Page

A **Web Page** is a single HTML document that is displayed in a web browser. It contains content such as text, images, videos, links, forms, and other multimedia elements.

Examples: Home Page, About Us Page, Contact Us Page

### **Website**

A **Website** is a collection of related web pages that are connected through hyperlinks and share the same domain name.

Example**:** A college website may contain: Home Page, About Page, Courses Page, Faculty Page, Contact Page. Together, these pages form a website.

### **Web Server**

A **Web Server** is a software or computer system that stores websites, processes client requests, and delivers web pages to users over the internet using the HTTP or HTTPS protocol. A web server receives requests from browsers, processes them, and returns the requested resources.

Examples: Apache HTTP Server, Nginx, Microsoft IIS, Node.js (using Express.js)

---