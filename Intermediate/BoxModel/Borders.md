# Border
- a visible line that encloses the padding and content
- the border does not change the width and height of the element
- its appearance, thickness, style, and color can be customized


#### `border:`
- `border: width style color;`: `border: 10px dashed red;`
    - shorthand for `border-width: 10px;`, `border-style: dashed;`, and `border-color: red;`
    
#### `border-width:`
- can take 1value, 2 values or 4 values
- `border-width: 20px;` applies 20px wide border to all four sides(top right bottom left)
- **with 4 values**: `border-width: top right bottom left;`: `border-width: 10px 15px 0px 20px;`
    - goes in a clockwise direction
    - shorthand for `border-top: 10px;`, `border-right: 15px;`, `border-bottom: 0px;`, `border-left: 20px;`
- **with 2 values**: `border-width: topandbottom rightandleft;`: `border-width: 10px 20px;`
    - shorthand for `border-top: 10px;`, `border-right: 20px;`, `border-bottom: 10px;`, `border-left: 20px;`