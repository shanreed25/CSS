# CSS Functions
**Are special values or constructs used within property declarations to perform calculations, transformations, or to represent specific data types. They allow for more dynamic and complex styling than static values alone.**

### Mathematical Functions
- These perform calculations. The most prominent example is calc(), which allows for arithmetic operations within property values, such as width: calc(100% - 20px);. Other math functions include min(), max(), and clamp(), used for setting value ranges.
### Transform Functions
- Used with the transform property to manipulate the position, size, and orientation of elements. Examples include translate(), rotate(), scale(), and skew(), which can be applied in 2D or 3D space (translate3d(), rotateX(), etc.).
### Color Functions
- Define colors using various models. Examples include rgb(), rgba(), hsl(), hsla(), and hwb(), allowing for color definition with or without an alpha (opacity) channel.
### [Image and Gradient Functions](./Background/BackgroundFunctions.md)
- Define background images or gradients. Examples include url() for referencing image files, linear-gradient(), radial-gradient(), and conic-gradient() for creating smooth color transitions, and their repeating-* counterparts for creating patterns.
### Filter Functions
- Used with the filter property to apply visual effects to elements, such as blur(), grayscale(), contrast(), drop-shadow(), and invert().
### Attribute and Environment Functions
- attr() can retrieve the value of an HTML attribute, while env() accesses user agent-defined environment variables.
### Shape Functions
- Used for defining shapes, particularly with clip-path or shape-outside, such as circle(), ellipse(), and polygon()