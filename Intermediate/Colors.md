# CSS Colors
- colors are a fundamental aspect of web design, allowing developers to apply various hues to HTML elements like text, backgrounds, borders, and more

- **`background-color: purple;`** background color
    - this property can be set on any elements, it colors the background area of the element
- **`color: purple;`**: font/text color

### [Named Colors](https://developer.mozilla.org/en-US/docs/Web/CSS/named-color)
- predefined keywords representing specific colors
- red, blue, royalblue, green, indigo, black, white, rebeccapurple etc....

### Hexadecimal Values (Hex Codes)
- common and concise way to represent colors using a six-digit hexadecimal number prefixed with a #
- each pair of digits corresponds to the red, green, and blue components of the color
    - #FF0000 for red or #000000 for black
- a shorthand three-digit notation can be used when each pair of digits is the same
    - #F00 is equivalent to #FF0000

### RGB and RGBA Values
- **RGB (Red, Green, Blue)**: defines colors by specifying the intensity of red, green, and blue light components, each ranging from 0 to 255
    -  Red `rgb(255, 0, 0)`
    -  Green `rgb(0, 255, 0)`
    -  Blue `rgb(0, 0, 255)`
- **RGBA (Red, Green, Blue, Alpha)**: extends RGB by adding an alpha channel for transparency, where the alpha value ranges from 0 (fully transparent) to 1 (fully opaque)
    - Semi-Transparent Green `rgba(0, 255, 0, 0.5)`

### HSL and HSLA Values
- HSL (Hue, Saturation, Lightness): defines colors based on their 
    - hue (color on the color wheel, 0-360 degrees)
    - saturation (intensity of the color, 0-100%)
    - lightness (brightness, 0-100%)
    - `hsl(120, 100%, 50%)` for pure green
- HSLA (Hue, Saturation, Lightness, Alpha): extends HSL by adding an alpha channel for transparency
    - `hsla(120, 100%, 50%, 0.5)` for semi-transparent green

### currentcolor Keyword
- a keyword that refers to the computed value of the color property of the element, allowing other properties like border-color to inherit the text color.
- These various color formats provide flexibility in defining and applying colors within CSS, enabling precise control over the visual appearance of web content.


- [Color Hunt](https://colorhunt.co/)
    -  a popular online platform that provides curated color palettes for designers, artists, developers, illustrators, and anyone seeking fresh color combinations for their projects