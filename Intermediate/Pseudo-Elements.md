# Pseudo-elements 
- are keywords added to a CSS selector that allow for the styling of specific, non-standard parts of an element or the insertion of content that is not explicitly present in the HTML
- they behave as if a new HTML element has been added to the markup, but they are created and controlled entirely through CSS
    - are not actual elements in the HTML Document Object Model (DOM) but are generated and styled by CSS
- they enable the styling of elements or content that cannot be targeted with standard CSS selectors, such as the first letter of a paragraph or the content before or after an element


### Syntax:
- modern pseudo-elements use a double-colon syntax: `::`
- for backward compatibility, some older pseudo-elements may still be seen with a single colon (:) 

#### Pseudo classes
- `:first-child` - Select the element when it’s the first inside its parent: `p:first-child {}`
- `:last-child` - Select the element when it’s the last inside its parent: `.item:last-child {}`
- `:only-child` - Select an element when it’s the only thing inside its parent: `li:only-child {}`
- `:nth-child()` - Select an element by it’s number
    - Good for zebra-striping table rows
    - `li:nth-child(2) {}`
    - `tr:nth-child(odd) {}`
    - `div:nth-child(5n) {}`
- `:nth-last-child()` - Select an element by it’s number, counting backwards from the end
    - Third from the bottom - `li:nth-last-child(3) {}`
- `:nth-of-type()` - Select an element by it’s number, but only counting others that match—not all children.
    - Second <p> element in its parent - `p:nth-of-type(2) {}`
- `:nth-last-of-type()` - Select an element by it’s number, counting backwards from the end.
    - Second <p> from the bottom - `p:nth-last-of-type(2) {}`
- `:first-of-type` - Select an element that’s the first of its kind within its parent: `p:first-of-type {}`
- `:last-of-type` - Select an element that’s the last of its kind within its parent: `p:last-of-type {}`
- `:only-of-type` - Select an element when it’s the only child of its parent of a specific kind: `p:only-of-type {}`
    - `section div:only-of-type {}`
- `:empty` - Select an element it has no children: `ul:empty {}`
- `:disabled` - Select an element when its disabled attribute is set: `button:disabled {}`
- `:checked` - Select an <input> when its checked attribute is set: `input:checked {}`
- `:target` - Select an element when the URL matches its ID: `li:target {}`
- `:not()` - Select matching elements that do not match the selection inside the (): `p:not(.mammal) {}`
    - `input:not(:checked) {}`

#### Pseudo elements
- `::before` - A hidden element before the content of most elements.
    ```
        blockquote::before {
        content: "“";
        font-size: 5rem;
        }
    ```
    - [Learn more about ::before.](https://learntheweb.courses/topics/before-after/)

- `::after` - A hidden element after the content of most elements.
    ```
        blockquote::after {
        content: "”";
        font-size: 5rem;
        }
    ```
    - [Learn more about ::after.](https://learntheweb.courses/topics/before-after/)

- `::first-line` - Select the first line of text, Good for highlighting the first line of a paragraph: `p::first-line {}`
- `::first-letter` - Select the first character in the text, Good for drop caps: `p::first-letter {}`
- `::selection` - Style an element when it has been selected and highlighted: `::selection {color: red;}`

#### Interacttion Selectors
- `:link` - For styling a link that hasn’t been visited: `a:link {color: #4484c2;}`
- `:visited` - For styling a link that has been visited: `a:visited {color: #ccc;}`
- `:hover` - For styling an element when the mouse hovers over it: `a:hover {color: #00f;}`
- `:focus` - For styling an element for when the keyboard focuses it, only works on `<a>`, `<button>`, and form inputs by default
    ```
    button:focus {
    outline: 3px solid #000;
    outline-offset: 2px;
    }
    ```
- `:active` - For styling an element when the mouse button is clicked down on it: `a:active {color: #f33;}`