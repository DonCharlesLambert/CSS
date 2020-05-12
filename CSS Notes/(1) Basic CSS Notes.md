# CSS Notes

## Prelude
All HTML elements are rectangles

## Linking
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">

## Selectors
>h2{  
  color: blue;  
}

#### CLASS
>.blue{  
  color: blue;
}  

#### ID
>#mytitle{  
  color: blue;
}  

#### ATTRIBUTE
>[attr=val]{  
  color: blue;
}  

## Variables
declared a css variables using
> --var-name: value;

Reference the variable using
> var(--var-name)

Fallback using
> var(--var-name, fallback-value)

## Precedence
!important (e.g color: pink !important;)  
inline  
id  
class  

## Colors
words		(e.g red)  
6 digit hex	(e.g #FF0000)  
3 digit hex	(e.g #F00)  
RGB		(e.g rgb(255, 0, 0))  

## Units
px - pixels  
in - inches  
mm - millimeters  
em - based on the font-size (if used to set font-size based on parent's font-size)  


## Attributes
* color
* font-size
* font-family

* width
* border-width
* border-color
* border-style
* border-radius

* padding <-- space between content and border
    * padding-top
    * padding-bottom
    * padding-left
    * padding-right
* margin <-- space between border and neighbouring elements
    * margin-top
    * margin-bottom
    * margin-left
    * margin-right

* background-color

### font-family degrading
font-family: Helvetica, sans-serif;  
Degrades to san-serif if Helvetica not found

### margin & padding clockwise notation
top right bottom left  
padding: 10px 5px 10px 5px;
