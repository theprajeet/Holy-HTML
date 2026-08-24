# HTML Forms

An **HTML form** is **a document section containing interactive controls that collect user input and submit it to a web server**. It is defined using the `<form>` element, which acts as a container for data entry fields like text boxes, checkboxes, radio buttons, and submit buttons

Forms serve as the gateway between the user and the server, allowing for dynamic, interactive web experiences. They are crucial for tasks such as user authentication, data submission, feedback collection, and more. Simply put, forms make websites more engaging and functional.

#### **HTML Forms Structure**

The fundamental structure of an HTML form is encapsulated within the **`<form>`** tags. Inside these tags, you'll place various form controls like text fields, checkboxes, radio buttons, and buttons for submitting the form.

```html
<form action="/submit" method="post">
    <!-- Text input for username -->
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" required>
    <br><br>

    <!-- Password input -->
    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required>
    <br><br>

    <!-- Radio buttons for gender -->
    <label>Gender:</label>
    <input type="radio" id="male" name="gender" value="male">
    <label for="male">Male</label>
    <input type="radio" id="female" name="gender" value="female">
    <label for="female">Female</label>
    <br><br>

    <!-- Submit button -->
    <input type="submit" value="Submit">
</form>
```

---

## HTML Input

The **`<input>`** tag is commonly used to create form controls. The attributes of this tag define the control's behaviour.

```html
<input type="" name="" value="">
```

The **"type"** attribute specifies the type of input control (e.g., text, password, checkbox).

The **"name"** attribute is used for identifying the control, especially when the data is sent to the server.

The **"value"** attribute sets a default value for the control, which the user can overwrite.

Input types in HTML forms are the backbone of interactive web applications. They allow users to send information to web servers for various purposes like searching, logging in, or providing feedback.

### **Text Input**

The text input type is the most basic form of input and is widely used for collecting simple text data.

```html
<input type="text" name="username" placeholder="Enter your username">
```

In the above example, the **`placeholder`** attribute provides a hint to the user about what to enter.

### **Password Input**

The password input type is similar to the text type but hides the characters entered by the user for security reasons.

```html
<input type="password" name="password" placeholder="Enter your password">
```

### **Radio Buttons**

Radio buttons are used when you want the user to select only one option from a set of choices.

```html
<input type="radio" id="male" name="gender" value="male">
<label for="male">Male</label>
<input type="radio" id="female" name="gender" value="female">
<label for="female">Female</label>
```

### **Checkbox**

Checkboxes allow the user to select multiple options from a set.

```html
<input type="checkbox" id="subscribe" name="subscribe" value="yes">
<label for="subscribe">Subscribe to newsletter</label>
```

### **More Input Types**

Here is a comprehensive list of input types you can use in HTML:

| **Input Type** | **Description** |
| --- | --- |
| text | Allows the user to type a single line of text. |
| password | Allows the user to type a password. |
| submit | Represents a button that, when pressed, submits the form. |
| reset | Represents a button that, when pressed, resets all the form controls to their initial values. |
| radio | Represents an option in a set of options that are mutually exclusive with each other. |
| checkbox | Represents an option in a set that may be selected independently of other options. |
| button | Represents a clickable button. |
| color | Allows the user to select a color. |
| date | Allows the user to select a date. |
| datetime-local | Allows the user to select a date and time with no time zone. |
| email | Allows the user to enter an email address. |
| file | Allows the user to select one or more files from their device storage. |
| hidden | Represents a value that is not displayed but is submitted to the server. |
| image | Defines an image that acts as a submit button. |
| month | Allows the user to select a month and year. |
| number | Allows the user to enter a number. |
| range | Allows the user to select a number from a range. |
| search | Allows the user to enter a search query string. |
| tel | Allows the user to enter a telephone number. |
| time | Allows the user to select a time. |
| url | Allows the user to enter a URL. |
| week | Allows the user to select a week. |

---

## **Textarea & Select**

In addition to the basic input types, HTML forms offer other controls like **`textarea`** and **`select`** for richer user interaction. These elements allow for more complex data collection and provide a better user experience. In this blog, we will dive into these form controls and provide examples.

### **The Textarea Element**

The **`textarea`** element is used when you need multiline text input from the user. This is particularly useful for comments, reviews, or any other type of input where the length is unpredictable.

```html
<textarea name="comment" rows="4" cols="50">
      Enter your comment here...
</textarea>
```

The **`rows`** and **`cols`** attributes define the visible dimensions of the textarea.

### **The Select Element**

The **`select`** element creates a dropdown menu for the user. It is useful when you have a predefined list of options for the user to choose from.

```html
<select name="fruits">
      <option value="apple">Apple</option>
      <option value="banana">Banana</option>
      <option value="cherry">Cherry</option>
</select>
```

Each **`option`** inside the **`select`** tag represents an item in the dropdown list.

### **Combining Textarea and Select**

You can combine **`textarea`** and **`select`** in the same form to capture varied types of user input

```html
<form action="/submit">
      <textarea name="comment" rows="4" cols="50">Enter your comment here...</textarea>
      <select name="fruits">
        <option value="apple">Apple</option>
        <option value="banana">Banana</option>
        <option value="cherry">Cherry</option>
      </select>
      <input type="submit" value="Submit">
</form>
```

---

## More on Forms

HTML forms are the backbone of interactive websites. They allow users to submit data, which can be processed on the server. While we have covered basic input types in previous tutorials, this tutorial aims to delve deeper into form attributes, both common and new HTML5 additions. We'll also look at HTML5 validation attributes to ensure data integrity.

### **Common Attributes**

### **action**

The **`action`** attribute specifies the URL where the form data should be sent after submission.

```html
<form action="/submit.php" method="POST">
</form>
```

### **method**

The **`method`** attribute defines how data is sent. The two most common methods are **`GET`** and **`POST`**.

```html
<form action="/submit.php" method="POST">
</form>
```

### **name**

The **`name`** attribute specifies the name for the form element, making it easier to reference in scripts or the server-side code.

```html
<input type="text" name="username">
```

---

### **New HTML5 Attributes**

### **placeholder**

This attribute provides a hint to the user as to what can be entered in the field.

```html
<input type="text" placeholder="Enter your username">
```

### **required**

The **`required`** attribute makes a field mandatory to fill out.

```html
<input type="text" required>
```

### **autofocus**

The **`autofocus`** attribute automatically focuses the cursor on the particular input when the page loads.

```html
<input type="text" autofocus>
```

### **HTML5 Validation Attributes**

### **required**

As mentioned above, this attribute makes a field mandatory.

```html
<input type="text" required>
```

### **pattern**

The **`pattern`** attribute specifies a regular expression that the input must match to be valid.

```html
<input type="text" pattern="[a-zA-Z0-9]+">
```

---