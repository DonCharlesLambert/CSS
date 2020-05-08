# CSS Flexbox

## Flexin'

### Display  
display: flex;  
lets you use other flex properties to build a responsive page  

### Flex-Direction  
flex-direction: row;  
how the elements within the element are organised.
* row
* row-reverse
* column
* column-reverse

### Justify-Content
justify-content: center;  
a flex container has a main axis  
for flex-direction: row this is a horizontal line through the container and for flex-direction: column it is a vertical line
* center
** aligns content on the center of the axis
* flex-start (default)
** aligns content at the start of the axis
* flex-end
* space-between
** first item is at the start of the axis, last item is at the end, other items spaced out inbetween
* space-around
** similar to space-between but first and last items are not locked at start/end
* space-evenly

### Align-Items
align-items: center;  
a flex container has a cross axis, perpendicular to the main axis  
* flex-start
* flex-end
* center
* stretch (default)
** Items are stretched to fill the container
* baseline
** For text, the line that letters sit on

### Flex-Wrap
flex-wrap: wrap;  
items that are bigger than the flex container move to a new row or colum  
* nowrap (default)
** does not wrap items
* wrap
* wrap reverse

### Flex-Shrink
flex-shrink: 1;  
applied to flex items rather than the container  
controls the size of the item when the container shrinks  
takes numbers as arguments

### Flex-Grow
flex-grow: 1;

### Flex-Basis
flex-basis: 10em;  
the initial size of the item before flex-shrink and flex-grow are applied

### Flex
flex: 1 0 10px;
Gives access to flex-grow, flex-shrink and flex-basis in that order

### Order
order: 2;
defines the order in which the items in the flex-box appear 

### Align-Self
Allows the item to align itself, takes same values as align item  