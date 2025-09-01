# Background Functions
**CSS offers several functions that can be used within background properties to create dynamic and complex backgrounds. These functions are primarily used with the background-image property or as part of the background shorthand property**

### Gradient Functions
- `linear-gradient()`: Creates a linear gradient, transitioning smoothly between two or more colors along a straight line. You can specify the direction (e.g., to right, 45deg) and color stops
    - `background-image: linear-gradient(to right, red, yellow);`
- `radial-gradient()`: Creates a radial gradient, transitioning smoothly between two or more colors radiating outward from a central point. You can specify the shape (e.g., circle, ellipse), size, position, and color stops
    - `background-image: radial-gradient(circle at center, blue, green);`
- `conic-gradient()`: Creates a conic gradient, transitioning between colors around a central point, similar to a pie chart. You can specify the starting angle, position, and color stops
    - `background-image: conic-gradient(from 90deg at 50% 50%, red, yellow, green);`


### Image Functions

### Other Functions