# Applied Visual Design

## Selectors

### Psuedo Selectors

## Psuedo Class Selector
>a:hover{  
  color: red;  
}

Color of tag becomes red when hovered over

## Psuedo Element Selector
>.element::before{  
  content: "";  
  color: red;  
}

>.element::after{  
  content: "";  
  color: red;  
}

must have a content property  
content used to add photos or text to the selected element  
can be an empty string  

## Color
rgba(255, 255, 255, 0.1)  
hsl(0, 100%, 50%)  
* Hue is from red to blue like a color wheel  
* Saturation is the amount of gray  
* Lightness is the amount of black or white  


## Backgrounds
linear-gradient()  
* e.g linear-gradient(35deg, #CCFFFF, #FFCCCC);

repeating-linear-gradient()
* e.g 
repeating-linear-gradient(  
      		90deg,  
      		yellow 0px,  
      		blue 40px,  
      		green 40px,  
      		red 80px  
    	    );  
	starts at 0px on yellow, blends in blue at 40px, straight into green at 40px ect

background: url()
* makes the background image from url

## Attributes
* text-align
	justify (same as word processing)
	center
	right
	left

* width
* height
* box-shadow
	takes the following args:
	offset-x offset-y blur-radius spread-radius color
* opacity
	takes values:
	0 to 1
* text-transform
	takes values:
	lowercase, uppercase, capitalize, initial, inherit, none
* font-weight
	takes values:
	0 to 1000
* line-height
* position
	takes values:
	relative, absolute, fixed
		absolute removes the element from the normal flow so surrounding items ignore it
		fixed does the same but a fixed position won't move when a user scrolls
* top, bottom, left, right
* float
	takes values:
	left, right
	float items are all removed from normal flow
	float as high as they can left/right in the parent contaienr
* z-index
	move to front/move to back
* margin: auto
	centers the element(s)
* transform
	takes values:
	scale(x)
	skewX(xdeg)
	skewY(ydeg)
	rotate(xdeg)
	

## Tags
* strong 	<-- makes text bold
* u 		<-- underlines text
* em		<-- italics (em for emphasis)
* s		<-- strikethrough
* hr		<-- adds a horizontal line, self closing

## Animation
>#rect {  
    animation-name: rainbow;  
    animation-duration: 4s;  
  }  
  
>@keyframes rainbow{  
    0%{  
      background-color: blue;  
    }  
    50%{  
      background-color: green;  
    }  
    100%{  
      background-color: yellow;  
    }  
  }  

a template for creating a simple animation^

> animation-fill-mode: forwards;

doesn't reset the animation

> animation-iteration-count: infinite;

yes! can also be any positive integer ofc

> aniamtion-timing-function

determines how quickly the element moves through key frames
options:
* ease		<-- start slow, speed up, end slow
* ease-in		<-- starts slow, ends fast
* ease-out	<-- starts fast, slows down
* linear		<-- constant 
* cubic-bezier(0.25, 0.25, 0.75, 0.75);
	* p1x, p1y, p2x, p2y
	* y value is progress in animation
	* x value is time as a porportion of animation-duration
	* A y value can be larger than 1 for a faster change (yup!)