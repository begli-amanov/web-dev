## Lesson 3

### Spaces Within Selectors
Within the previous combined selector, `.hotdog p.mustard`, there is a space between the hotdog class selector and the paragraph type selector but not between the paragraph type selector and the mustard class selector. The use, and omission, of spaces makes a large difference in selectors.

Since there isn’t a space between the paragraph type selector and the mustard class selector that means the selector will only select paragraph elements with the class of mustard. If the paragraph type selector was removed, and the mustard class selector had spaces on both sides of it, it would select any element with the class of mustard, not just paragraphs.

The best practice is to not prefix a class selector with a type selector. Generally we want to select any element with a given class, not just one type of element. And following this best practice, our new combined selector would be better as `.hotdog .mustard`.



### Sizing Inline-Level Elements
Please keep in mind that inline-level elements will not accept the width and height properties or any values tied to them. Block and inline-block elements will, however, accept the width and height properties and their corresponding values.


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