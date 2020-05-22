# jQuery

    $(document).ready(function(){
	    //waits till HTML is rendered before running
    })

## Selector
Selects all button elements from the document

      $("button")

Select all elements with class well

	  $(".well")

Select element with id target

	  $("#target")

Selects all elements with class target that are the nth child in their parent container

    $(".target:nth-child(n)")

Selects all elements that are the nth child in their parent container where n is odd/even. Zero-indexed.

    $(".target:odd")
    $(".target:even")

## Functions
### Changing HTML & Text
Removes all h3 elements

    $("h3").remove();

Moves an element to within another element

    $("#target").appendTo("#my-div");

Completely replaces the HTML within all h3 elements

    $("h3").html("<em>jQuery Playground</em>");

Completely replaces the text within all h3 elements but does not evaluate the tags

    $("h3").text("<em>jQuery Playground</em>");

### Changing Classes
Adds the btn class to all button elements

      $("button").addClass("btn")
  
Removes the btn-primary class from button with id target

      $("#target").addClass("btn-primary")

### Changing props
Add a disabled prop to all buttons

      $("button").prop("disabled", true);

### Changing Styles
Add a CSS style to button with id target. Note that the attribute and the value are passed as two separate arguments.

    $("#target1").css("color", "blue");

### Other
Clones an element

    $("#target").clone();

Gets the parent of an element

    $("#target").parent();

Gets all the children of an element

    $("#target").children()


### Joke
need animated.css or something

    $("body").addClass("animated hinge")
