# Applied Accessbility

## Notes

* alt attributes provides alternative text if the image can not render, is also
converted to audio by screen readers. Required in HTML5 for each image but can be blank.
* don't use h tags for fashion, audio readers rely on this for summaries
* articles group indepedent self containing content which should be able to stand alone
* section element should be used for different sections of an article per say
(thematically related content)
* header is used to wrap introductory information (e.g a h1 tag)
* nav wraps around main navigation links
* footer holds copyright information and links to related documents
* an input in a form should be nested in a label tag, the label tag should have a for
attribute that is equal to the id of the input
* dates/time in text must be wrapped with a time tag with an attribute of datetime set to the
formal date/time
* Web Content Accessibility Guidelines (WCAG) recommend at least a 4.5 to 1
contrast ratio for normal text
* Be considerate of color blind users
* The text inside an a tag should be informative for screen readers
* access keys (these are cool) used as an attribute for a and button tags,
e.g accesskey="g"
* tabindex attribute


## Tags
* main
* header
* footer
* nav
* article
* section

* figure
** figcaption

* audio
** source

* fieldset
** legend
holds a set of inputs (usually for radio buttons) legend is the caption/title
fieldset creates a cool box that cuts at legend

* sup
superscript