# CSS Grid

## Grid
>display: grid;  

turns an element into a grid container


>grid-template-columns: 50px 50px;  

the number of parameters is the number of columns, the paramaters are the width of the columns  


>grid-template-rows: 50px 50px;  

the number of parameters is the number of rows, the paramaters are the width of the rows  
alternativley can write repeat(2, 50px)  
to specify the minimum and maximum size of a row use minmax(x, y)


>grid-column-gap: 10px;  
>grid-row-gap: 10px;  

puts a 10px gap between each row/column


>grid-gap: 10px;

if given one value puts a 10px gap between rows AND columns  
if two values given the first is rows second is gap for columns


>grid-column: 1/3

defines the number of columns and ITEM takes up  
in the example the item spans from the 1st line (beginning of 1st column) to the third line (end of 2nd column)


>grid-row: 1/3

see grid-column


>justify-self: center

used to align the ITEM in the cell horizontally  
* stretch (default)
* center
* end


>align-self: center

aligns the ITEM in the cell vertically  
takes the same values as justify-self


>justify-items: center
>align-items: center

used on the container...  


>grid-template-areas:
"header header header"
". content content"
"footer footer footer";

merges the cells together into named areas  
. means empty cell


>grid-area: header;

allocates an item to a grid-area


>grid-area: 3/1/4/4;

allocations an area to the grid  
first value is horizontal line (-) to start at, third is horizontal line to end at  
second value is vertical line (|) to start at, fourth is vertical line to end at


## Functions
repeat(2, 1fr)  
* first parameter can be auto-fill
* first paramater can be auto-fit, like auto-fill but stretchs the elements
minmax(50px, 200px)  

## Units
* px  
* em
* fr
	* sets the col/row to a fraction of the available space  
* auto  
* %
	* sets the col/row to a percentage width of its container