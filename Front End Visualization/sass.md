# Sass
Sass, or "Syntactically Awesome StyleSheets", is a language extension of CSS.
There are two syntaxes available for Sass. The first, known as SCSS (Sassy CSS) and used throughout these challenges, is an extension of the syntax of CSS. This means that every valid CSS stylesheet is a valid SCSS file with the same meaning. Files using this syntax have the .scss extension.

## Linking

    type="text/sass"
Type is set to text/sass rather than text/css

## Variables
Declaring a variable

    $main-fonts: Arial, sans-serif;

Using a variable

    h1{
	    font-family: $main-fonts;
    }

## Nesting Styles
Styles for child elements can be nested within styles for parent elements

## Mixin
A mixin is a group of CSS declarations that can be reused throughout the stylesheet
```scss
    @mixin box-shadow($x, $y, $blur, $c){ 
      -webkit-box-shadow: $x $y $blur $c;
      -moz-box-shadow: $x $y $blur $c;
      -ms-box-shadow: $x $y $blur $c;
      box-shadow: $x $y $blur $c;
    }
```    
The mixin is called using the @include directive
```scss
	div {
	  @include box-shadow(0px, 0px, 4px, #fff);
	}
```
## Stolen Syntax!

### If, Else If and Else
```scss
    @mixin text-effect($val) {
      @if $val == danger {
        color: red;
      }
      @else if $val == alert {
        color: yellow;
      }
      @else if $val == success {
        color: green;
      }
      @else {
        color: black;
      }
    }
```
### For
For start to end excludes the end number
```scss
	@for $i from 1 through 12 {
	  .col-#{$i} { width: 100%/12 * $i; }
	}
```
For start through end includes the end number
```scss
    @for $i from 1 through 12 {
      .col-#{$i} { width: 100%/12 * $i; }
    }
```
### Each
Loops over each item in a list
```scss
	@each $color in blue, red, green {
	  .#{$color}-text {color: $color;}
	}
```

Loops over each item in a map
```scss
	$colors: (color1: blue, color2: red, color3: green);

	@each $key, $color in $colors {
	  .#{$color}-text {color: $color;}
	}
```

### While
```scss
	$x: 1;
	@while $x < 13 {
	  .col-#{$x} { width: 100%/12 * $x;}
	  $x: $x + 1;
	}
```

### Extend
This one is pretty cool, computer science is beautiful
```scss
.panel{
  background-color: red;
  height: 70px;
  border: 2px solid green;
}


.big-panel{
  @extend .panel;
  width: 150px;
  font-size: 2em;
}
```