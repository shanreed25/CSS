# Fixed Elements
**A fixed element is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled.**

- change its CSS position property to fixed, allowing it to stay visible as the user continues scrolling

## Fixing the Div after scrolling using position: sticky
- `position: sticky;`
- makes the div stay in place as you scroll down. Set the top property to determine how far from the top the div will remain visible
- Initially behaves like position: relative, meaning it's positioned relative to its nearest positioned ancestor. 
- Once the user scrolls past a specified offset, it "sticks" to the top or bottom of the viewport, acting like position: fixed. 
- It's often used for elements like headers that become fixed after scrolling past a certain point. 

## Fixing the Div after scrolling using position: fixed
- `position: fixed;`
- keeps the div in a fixed position on the screen, regardless of scrolling. Set the top, right, bottom, or left properties to position it as needed
- The element remains in its fixed position on the screen, even when the page is scrolled. 
- It is positioned relative to the browser window (viewport). 
- It's commonly used for elements like navigation bars or footers that should always be visible. 

## Difference between position: fixed and position: sticky i
thie difference lies in how they are positioned relative to the user's scrolling behavior. 
- position: fixed keeps an element fixed at a specific position on the screen, regardless of the user's scroll position. 
- position: sticky, on the other hand, behaves like position: relative until the user scrolls a certain point, at which point it "sticks" to the top or bottom of the viewport, becoming fixed.- fixed is always fixed in place, while sticky becomes fixed after scrolling a certain amount. 
- Both help keep elements visible while scrolling, but they do so at different times. 
- The choice between them depends on whether you want an element to always stay in place or only stick after scrolling to a specific point. 