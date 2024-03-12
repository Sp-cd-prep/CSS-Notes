# CSS-Notes

## Class 1: Introduction to CSS and Text Formatting

### Part 1: Introduction to CSS

**Definition:**
CSS stands for Cascading Style Sheets. It is a language used to describe the presentation of web pages, including their layout, colors, fonts, and more. CSS allows you to control the visual appearance of HTML elements on a webpage.

**Implementation:**
CSS can be applied to HTML elements using three different methods: Inline, Internal, and External.

1. **Inline CSS:**
   Inline CSS is applied directly to an HTML element using the `style` attribute. It's useful for making small, specific style changes.

   ```html
   <p style="color: blue;">This is a blue text.</p>
   ```

2. **Internal CSS:**
   Internal CSS is placed within the `<style>` element in the HTML document's `<head>`. It affects elements throughout the document.

   ```html
   <head>
     <style>
       p {
         color: red;
       }
     </style>
   </head>
   ```

3. **External CSS:**
   External CSS is stored in a separate `.css` file and linked to the HTML document using the `<link>` element. This method is best for maintaining consistent styles across multiple pages.

   ```html
   <head>
     <link rel="stylesheet" type="text/css" href="styles.css" />
   </head>
   ```

### Part 2: Tags vs IDs vs Classes

**Tags:**
HTML tags represent different elements on a webpage, like headings (`<h1>`, `<h2>`, ...), paragraphs (`<p>`), links (`<a>`), etc. You can target these tags in your CSS to apply styles.

**IDs:**
An ID is a unique identifier given to an HTML element using the `id` attribute. IDs are used to target specific elements for styling and JavaScript interactions.

**Classes:**
A class is a reusable identifier applied to one or more HTML elements using the `class` attribute. Classes allow you to apply the same styles to multiple elements.

**Implementation:**

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" type="text/css" href="styles.css" />
  </head>
  <body>
    <h1>This is a heading</h1>
    <p id="unique-paragraph">This is a unique paragraph with an ID.</p>
    <p class="common-paragraph">This is a common paragraph with a class.</p>
  </body>
</html>
```

### Part 3: CSS Text Formatting

1. **Color:**
   The `color` property is used to change the text color. Colors can be specified in various ways, such as color names, HEX codes, RGB values, etc.

   ```css
   p {
     color: blue;
   }
   ```

2. **Font Family:**
   The `font-family` property defines the typeface for text. You can specify multiple font families, and the browser will use the first available font.

   ```css
   body {
     font-family: Arial, sans-serif;
   }
   ```

3. **Font Style:**
   The `font-style` property is used to apply styles like italic or oblique to text.

   ```css
   em {
     font-style: italic;
   }
   ```

4. **Font Size:**
   The `font-size` property sets the size of the font. It can be specified in various units like pixels (`px`), ems (`em`), or percentages (`%`).

   ```css
   h1 {
     font-size: 24px;
   }
   ```

5. **Using Google Fonts:**
   Google Fonts provides a wide range of free, web-safe fonts that you can use in your projects. To use Google Fonts, you need to link to the font stylesheet in your HTML.

   ```html
   <head>
     <link
       rel="stylesheet"
       href="https://fonts.googleapis.com/css?family=Roboto"
     />
   </head>
   ```

   ```css
   body {
     font-family: "Roboto", sans-serif;
   }
   ```

**Notes:**

- CSS is used to style HTML elements.
- There are three ways to apply CSS: Inline, Internal, and External.
- Tags, IDs, and Classes are used to target specific elements for styling.
- You can format text using properties like color, font family, font style, and font size.
- Google Fonts provides a wide variety of fonts for web use.

In HTML and CSS, both classes and IDs are used to apply styles to elements, but they serve different purposes and have distinct characteristics.

### Classes:

1. **Purpose:**
   - Used to define a class of elements that share common styles.
   - Multiple elements can have the same class.
   - Classes are suitable for styling groups of similar elements.

2. **Syntax:**
   ```html
   <div class="example-class">This is a div with a class.</div>
   ```

3. **CSS Selection:**
   ```css
   .example-class {
       /* Styles for elements with the class 'example-class' */
   }
   ```

4. **Usage:**
   - Can be applied to multiple elements on a page.
   - Enables the reusability of styles across different elements.

5. **Example:**
   ```html
   <p class="highlight">This paragraph has a highlight class.</p>
   <span class="highlight">This span also has a highlight class.</span>
   ```

### IDs:

1. **Purpose:**
   - Used to uniquely identify a single element on a page.
   - Each page should have only one element with a particular ID.

2. **Syntax:**
   ```html
   <div id="example-id">This is a div with an ID.</div>
   ```

3. **CSS Selection:**
   ```css
   #example-id {
       /* Styles for the element with the ID 'example-id' */
   }
   ```

4. **Usage:**
   - Should be unique within the HTML document.
   - Typically used for styling a specific, unique element.

5. **Example:**
   ```html
   <header id="main-header">This is the main header.</header>
   ```

### Key Differences:

- **Uniqueness:**
  - Classes can be shared among multiple elements.
  - IDs must be unique within a document.

- **Selection:**
  - Use a dot (`.`) for class selectors (e.g., `.example-class`).
  - Use a hash (`#`) for ID selectors (e.g., `#example-id`).

- **Styling Scope:**
  - Classes are generally used for styling groups of similar elements.
  - IDs are often used for styling a specific, unique element.

- **Applicability:**
  - Use classes when styling multiple elements with similar styles.
  - Use IDs when styling a single, unique element.

- **Usage in JavaScript:**
  - Classes are commonly used to identify and manipulate groups of elements with JavaScript.
  - IDs are often used to uniquely identify elements for more specific JavaScript interactions.

