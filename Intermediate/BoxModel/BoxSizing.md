# `box-sizing`
- property that controls how the total width and height of an element are calculated in relation to its padding and border
- addresses a common challenge in CSS layouts where adding padding or borders to an element can unexpectedly increase its overall dimensions beyond the explicitly set width and height

### Main values for the box-sizing property
- `content-box (Default)`
    - default behavior.
    - width and height properties define the dimensions of the element's content area only
    - padding and border values are added to this content area, increasing the element's total occupied space
    - calculation: total width = width + padding (left + right) + border (left + right)
- `border-box`
    - width and height properties define the dimensions of the element including its padding and border.
    - content area shrinks to accommodate the specified padding and border within the declared width and height.
    - makes layout calculations more intuitive, as the specified width and height directly correspond to the visual space the element occupies on the page.
    - calculation: total width = width (where width already includes padding and border within its bounds).


**Using box-sizing: border-box; is often preferred in modern CSS development for its predictability and ease of layout management, especially in responsive design. It is common practice to apply box-sizing: border-box; globally to all elements using a universal selector**