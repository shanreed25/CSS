# CSS Selectors
-  a pattern used to select and target specific HTML elements on a web page to apply styles to them
- it  is the first part of a CSS rule, followed by a declaration block containing CSS properties and their values


# Common types of CSS selectors include:
- **Type/Element Selectors**: select elements based on their HTML tag name
    - `p{}` selects all paragraph elements
- **Class Selectors**: select elements based on the value of their class attribute, prefixed with a period
    - `.main{} `selects all elements with `class="main"`
    - multiple elements can have the same class name
- **ID Selectors**: select a unique element based on the value of its id attribute, prefixed with a hash symbol
    - `#main-header{}` selects the element with `id="main-header"`
    - ids are unique and should only be given to one element
- **Attribute Selectors**: select elements based on the presence or value of an HTML attribute 
    - `input[type="text"]{}` selects all input elements with `type="text"`
    - `p[draggable]{}` selects all input elements with the `draggable` attribute
- **Universal Selector**: selects all elements on a page, represented by an asterisk  `*`
- **Combinators**: combine multiple simple selectors to create more specific selections, such as descendant combinators 
    - (space), child combinators (>), and sibling combinators (+, ~).
- **Pseudo-classes**: select elements based on their state or position within the document tree
    - `:hover{}` selects an element when the mouse pointer is over it
- **Pseudo-elements**: select and style specific parts of an element 
    - `::before{}` inserts content before an element