# Container class
- is used for structuring content within a responsive web design
- provides a foundational element for containing, padding, and aligning content within a webpage


## How It Works
- **Fixed-Width Container**
    - the default .container class creates a responsive, fixed-width container
    - its max-width property changes at predefined breakpoints (e.g., small, medium, large, extra-large screen sizes) to adapt to different device widths
    - content within this container will be centered on the page and will have horizontal padding.
- **Responsive Behavior**
    - the container class utilizes Bootstrap's breakpoint system
    - as the browser or device viewport resizes, the container's width adjusts at these specific breakpoints, ensuring the content remains well-organized and readable across various screen sizes
- **Content Wrapper**
    - acts as a wrapper for other Bootstrap components and your custom content, such as rows, columns, headings, paragraphs, and image
    - allows you to leverage Bootstrap's grid system and other utilities within a structured and responsive layout.


## Types of Containers
- **`.container`** standard responsive, fixed-width container that adjusts its max-width at different responsive breakpoints (e.g., small, medium, large screens)
- **`.container-fluid`** a full-width container that spans the entire width of the viewport, regardless of screen size
- **Responsive Containers `.container-{breakpoint}` (e.g., .container-sm, .container-md, .container-lg, .container-xl, .container-xxl)** 
    - These classes provide a hybrid approach. They are 100% wide until a specified breakpoint is reached, after which they adopt fixed max-width values for larger breakpoints
    - For example, `.container-md` will be 100% wide on extra-small and small screens, but will have a fixed max-width at medium and larger breakpoints