# The Box Model
- describes how HTML elements are rendered as rectangular boxes on a webpage
- every HTML element is treated as a rectangular box with distinct layers
- the margin, padding, border, width and height properties form the box model

![CSS Box Model](assets/cssboxmodel.png)
__________________________________________
### Content
- the innermost area where the actual content of the element resides, such as text, images, or other media
- it's dimensions are determined by the width and height properties
### Padding
- a transparent area that surrounds the content and creates space between the content and the element's border
- it is controlled by properties like padding-top, padding-right, padding-bottom, padding-left, or the shorthand padding.
### Border
- a visible line that encloses the padding and content
- its appearance (thickness, style, color) is defined by properties such as border-width, border-style, and border-color, or the shorthand border

### Margin
- a transparent area surrounds the border and creates space between the element and other adjacent elements on the page
- it is controlled by properties like margin-top, margin-right, margin-bottom, margin-left, or the shorthand margin.

### Box-Sizing
- by default, the width and height properties in CSS refer to the content area only (known as content-box behavior)
- this means that any padding or border added will increase the overall size of the element beyond the specified width and height.
- however, the box-sizing property, often set to border-box, changes this behavior
- when box-sizing: border-box; is applied, the width and height properties include the padding and border within the specified dimensions, making it easier to manage element sizes in complex layouts
- the margin is never included in the calculation of an element's total width and height.

# BOX Model
- every HTML element is treated as a rectangular box, and we can change the dimensions of these boxes 