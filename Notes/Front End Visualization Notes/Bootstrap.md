The course is completed but this feels incomplete
# Boostrap
Bootstrap is responsive, it figures out how wide the screen is and resizes HTML elements accordingly. Link boostrap to your HTML document the same way you would link a stylesheet.

Linking Bootstrap

    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous"/>


Linking Font Awesome

    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css" integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous">


## Layout
    <div class="row">
    </div>
Creates a bootstrap table row

    <div class="col-xs-*">
    </div>
Creates a column in the row  
Where * is between 1 and 12 and determines the size of the column as a proportion of the screen

## Font Awesome
Provides icons (e.g)

    <i  class="fas fa-thumbs-up"></i>

## Div Classes
* container-fluid
	* responsively takes up the width of the view-port
* well
	* creates a well looking div
## Images Classes
* img-responsive

## Text Classes
* text-center
* text-primary
* text-danger

## Buttons Classes
* btn
* btn-default
* btn-primary
* btn-info
* btn-danger
* btn-block
	* button is the width of the container

## Form Classes
* form-control
	* Gives all `<input>` ,`<textarea>` and `<select>` widths of 100%, also makes them look good