# CSS Fonts
- CSS provides various properties to control the appearance of text, including fonts
- the primary property for setting fonts is `font-family`

# Fonts Properties
- [Font Family](#font-family)
- [Font Size](#font-size)
- [Font Weight](#font-weight)
- [Text Alignment](#text-alignment)
- []()


## Font Family
- `font-family`
- specifies what you want your font to look like
- Typeface: design of the characters
    - the overall design and style of a set of characters, such as Arial, Times New Roman, or Helvetica. It's the visual blueprint for how text will appear
- can accept multiple font names as a "fallback" system
    - if the user's browser or operating system does not support the first font listed, it will attempt to use the next font in the list
    - this ensures a consistent look across different environments
    - `font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;`
        - the browser will first attempt to use "Helvetica Neue"
        - if that's not available, it will try Helvetica, then Arial
        - and then finally a generic sans-serif font if none of the specific typefaces are found
- `sans-serif` type of font were all the edges are pretty much at a right angle, like `Helvetica`
- `serif` type of fonts that have decorations or little feet at the edges, like `"Times New Roman"`
- when font names have mutiple words we must use Quotes, `"Helvetica Neue"`
- generic font will be differnt depending on the computer you are using
    - fonts such as `monospace`, `cursive`, `serif`, `sans-serif`, `fantasy` etc...
- [Google Fonts](https://fonts.google.com/) is a good place to find fonts
    - when you find a font you want to use it provides you with links tag that will add the font to your page
    - add the link tag in the head of the HTML document just below the css stylesheet link and then you can use it in your CSS
    - these fonts will be avaliable on every computer because of the link

## Font Size:
- `font-size`
- sets the size of the font

#### Absolute Sizes
- Keywords: `xx-small`, `x-small`, `small`, medium, large, x-large, xx-large
- predefined sizes relative to the user's default font size

#### Relative Sizes
- **Keywords** `smaller`, or `larger`
    - these adjust the font size relative to the parent element's font size.
- **Percentages**
    - font size is a percentage of the parent element's font size.
- **em units** about the size of the letter `m`
    - is 100% of the parent font-size
        - `<div><h1></h1></div>`
        - if the div font size is 20px and the h1 font size is set to 1em, then the font size of the h1 is 20px
- **rem units**
    - 1rem is always equal to the computed font size of the root HTML element, typically `<html></html>`, 100% of root
    - provides a consistent base for scaling across the entire document
    - rem units are a more consistent way of changing the sizes and therfore it is recommended to use instead of em units

#### Length Units
- **Absolute/Static Length Units**
    - **`px` (pixels)**: a fixed size on the screen, not responsive to user settings or viewport changes 1px equals 1/96th(0.26mm x 0.26mm) of an inch
    - **`pt` (points)**: often used in print media, 1pt equals 1/72nd(0.35mm x 0.35mm) of an inch
    - **`cm` (centimeters), `mm` (millimeters), `in` (inches), `pc` (picas), `Q `(quarter-millimeters)**
- **Viewport-Relative Units**
    - **`vw` (viewport width)**: 1vw is 1% of the viewport's width
    - **`vh` (viewport height)**: 1vh is 1% of the viewport's height
    - **`vmin` (viewport minimum)**: 1vmin is 1% of the smaller dimension (width or height) of the viewport
    - **`vmax` (viewport maximum)**: 1vmax is 1% of the larger dimension (width or height) of the viewport

#### Other Units
- **`ch` units**: represents the width of the "0" (zero) character in the current font
- **`ex` units**: represents the x-height of the current font (typically the height of lowercase letters like 'x')

#### Choosing the Right Unit
- For responsive designs: rem, em, vw, vh are often preferred for their adaptability to different screen sizes and user preferences
- For fixed layouts or specific print requirements: px or pt might be suitable
- For accessibility: Using relative units like rem allows users to adjust their browser's default font size, impacting the entire document and improving readability



## Font Weight
- `font-weight`
- controls the boldness of the font
- Basic Keywords: `normal`, `bold`
- Relative To Parent Keywords: `lighter`-100, `bolder`+100, range(100 to 900)
- Number: 100(light) to 900(bolder)

## Text Alignment
- `text-align`
- values can be 
    - `center`
    - `left`
    - `right`
    - `start`, `end`: text start writing from right to left, or left to right
    - :
