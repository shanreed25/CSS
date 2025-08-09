# Cascading Style Sheets: CSS
- a style sheet language used for describing the presentation of a document written in HTML or XML, including SVG, MathML, or XHTML
- describes how elements should be rendered on screen, on paper, in speech, or on other media
- crucial for creating visually appealing, user-friendly, and maintainable websites, as it separates the presentation of a document from its content and structure
- **Layout**: Positioning elements, setting margins and padding, creating columns, and defining responsiveness for different screen sizes.
- **Typography**: Choosing fonts, setting font sizes, colors, line heights, and text alignment.
- **Colors and backgrounds**: Defining background colors and images, text colors, and element borders.
- **Visual effects**: Adding shadows, transitions, animations, and other visual enhancements

### Cascading
- CSS rules cascade, meaning that multiple style sheets and rules can apply to the same element, with a defined order of precedence determining which rule takes effect
- refers to the process by which a web browser determines which CSS rules to apply when multiple, potentially conflicting, styles target the same HTML element
- cascade follows a specific set of rules to resolve these conflicts, ensuring a predictable outcome for how elements are styled
    - **Specificity**: This is a measure of how precise a CSS selector is. More specific selectors (e.g., an ID selector like #myElement) override less specific ones (e.g., a tag selector like p).
    - **Origin**: Styles can come from different sources:
        - **User agent stylesheets**: Default styles provided by the browser.
        - **User stylesheets**: Custom styles defined by the user.
        - **Author stylesheets**: Styles defined by the web developer (the most common type).
        - **!important declarations**: These override normal declarations, regardless of specificity or origin, but should be used sparingly.
    - **Source Order**: When rules have the same specificity and origin, the rule that appears later in the stylesheet (or linked/imported files) takes precedence. This means the last declared style will "win" if other factors are equal.
- the cascade algorithm evaluates all applicable styles for an element, then applies these rules in a hierarchical order, with more specific and later-declared styles typically overriding earlier or less specific ones
    - allows developers to apply broad styles and then progressively refine them with more targeted rules
- elements also inherit styles from their parent elements

### Style Sheet
- refers to a collection of rules that define the presentation and layout of a web document. It acts as a blueprint for how HTML elements should appear in a web browser
- **Rules and Declarations**: consists of CSS rules, each containing a selector (which targets specific HTML elements) and a declaration block
    - the declaration block holds one or more declarations, where each declaration specifies a property (color, font-size) and its corresponding value (blue, 16px)
- **Separation of Concerns**: enable the separation of content (HTML) from presentation (CSS)
    - makes web development more organized, maintainable, and efficient, as changes to the visual design can be made without altering the HTML structure

### Types of Style Sheets
- there are three primary methods for integrating CSS with HTML
- **External Style Sheets**: separate `.css` files linked to HTML documents, allowing for consistent styling across multiple web pages
    - add `<link rel="stylesheet" href="file.css">` element in the head of the html file
- **Internal Style Sheets**: styles are defined within `<style>` tags in the `<head>` section of an HTML document, applying styles specifically to that page
    - this `<style>` tag can be put in other places in a html document but, it is convention to add it in the `<head>` section of the document
    - `<style>p {font-size: 10px;}</style>`
- **Inline Styles**: styles are applied directly to individual HTML elements using the style attribute, offering highly specific styling but generally less maintainable for large projects
    - `<p style="color: purple; font-size: 10px;">This is a paragraph with inline styles.</p>`


# How CSS Works
- applys rules to specific HTML elements
- these rules consist of a 
    - **[selector](./Selectors.md)**: targets the HTML element, 
        - a selector for a `<h1>` tag is `h1{declration block}`
    - **declaration block**: contains properties and their corresponding values, defining the style
        - `h1{property:value}`


# Other Stylesheet Languages
- **Sass**: Syntactically Awesome Style Sheet
- **Less**: Leaner CSS
- and many others



### Basic CSS concepts 
**Understanding these core concepts provides a strong foundation for writing effective and maintainable CSS**
- Syntax

- Cascading
- Inheritance
    - Some CSS properties, like color and font-family, are inherited by child elements from their parent elements. This means you can set a style once on a parent element, and its children will automatically adopt that style unless explicitly overridden.
- [Selectors](./Selectors.md)
    - used to select the HTML elements you want to style
- [The Box Model](./BoxModel.md)
    - every HTML element is treated as a rectangular box and the box model describes the layout of these boxes
