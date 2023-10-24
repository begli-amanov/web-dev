## Lesson 3

### Spaces Within Selectors
Within the previous combined selector, `.hotdog p.mustard`, there is a space between the hotdog class selector and the paragraph type selector but not between the paragraph type selector and the mustard class selector. The use, and omission, of spaces makes a large difference in selectors.

Since there isn’t a space between the paragraph type selector and the mustard class selector that means the selector will only select paragraph elements with the class of mustard. If the paragraph type selector was removed, and the mustard class selector had spaces on both sides of it, it would select any element with the class of mustard, not just paragraphs.

The best practice is to not prefix a class selector with a type selector. Generally we want to select any element with a given class, not just one type of element. And following this best practice, our new combined selector would be better as `.hotdog .mustard`.


### Sizing Inline-Level Elements
Please keep in mind that inline-level elements will not accept the width and height properties or any values tied to them. Block and inline-block elements will, however, accept the width and height properties and their corresponding values.

op
### Margin & Padding on Inline-Level Elements
Inline-level elements are affected a bit differently than block and inline-block elements when it comes to margins and padding. Margins only work horizontally—left and right—on inline-level elements. Padding works on all four sides of inline-level elements; however, the vertical padding—the top and bottom—may bleed into the lines above and below an element.

Margins and padding work like normal for block and inline-block elements.


### Removing Spaces Between Inline-Block Elements
1. The first solution is to put each new `<section>` element’s opening tag on the same line as the previous `<\section>` element’s closing tag. Rather than using a new line for each element, we’ll end and begin elements on the same line.

2. Another way to remove the white space between inline-block elements is to open an HTML comment directly after an inline-block element’s closing tag. Then, close the HTML comment immediately before the next inline-block element’s opening tag. Doing this allows inline-block elements to begin and end on separate lines of HTML and “comments out” any potential spaces between the elements.


### When to Use an Image Element vs. a Background Image

The `<img>` element within HTML is the preferred option when the image being used holds semantic value and its content is relevant to the content of the page.

The `background` or `background-image` property within CSS is the preferred option when the image being used is part of the design or user interface of the page. As such, it’s not directly relevant to the content of the page.


### Audio

When the preload attribute isn’t present on the `<audio>` element, all information about an audio file is loaded, as if the value was set to `auto`. For this reason, using the `preload` attribute with a value of `metadata` or `none` is a good idea when an audio file is not essential to a page. It’ll help to conserve bandwidth and allow pages to load faster.


### Useful Tags

Tags for expandable parts of text

Progress and Meter tags for bars

Datalist tag for input type like Select

Optgroup tag for nesting options in drop down menu of select or datalist

Template tag for more dynamic control of the web page


### Buttons
By default, the `<button>` element acts as if it has a type attribute value of submit, so the type attribute and value may be omitted from the `<button>` element


### Labels ans inputs
Labels may include a for attribute. The value of the for attribute should be the same as the value of the id attribute on the form control the label corresponds to. Matching up the for and id attribute values ties the two elements together, allowing users to click on the <label> element to bring focus to the proper form control.


### CSS
One of the important stuff after `CSS RESET` is the following rule set:

`*,
*:before,
*:after {
   box-sizing: border-box;
}
`

### Vertical Align
The vertical-align property works only with inline and table-cell elements—it won’t work for block, inline-block, or any other element levels.


### Vertically centering text within a button with line-height
Line height may also be used to vertically center a single line of text within an element. Using the same property value for the line-height and height properties will vertically center the text:

height-22px
line-height-22px


### Semantic difference between TH and TD
table header element provides semantic value by signifying that the data within the cell is a heading, while the <td> element only represents a generic piece of data.


### What is DOM?

The DOM, or Document Object Model, is an API for HTML and XML documents which provides their structural representation. In our case, we are speaking specifically to HTML documents, thus the DOM represents all of the different elements and their relationship to each other.

The representation can be considered a tree of sorts, with each element having a different relationship with those around it. Elements nested inside others have a parent and child relationship while elements that share the same parent have a sibling relationship.