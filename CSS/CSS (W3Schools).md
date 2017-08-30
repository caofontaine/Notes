# CSS (W3Schools)
CSS is a language that describes the style of an HTML document.
## CSS Introduction
Cascading Style Sheets
Describes how HTML elements should be displayed on screen, paper, or in other media.
External stylesheets are stored in CSS files.
  ### Why Use CSS?
  - Used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.
  ### CSS Solved A Big Problem
  - HTML never intended to have tags for formatting web pages.
  - HTML describes the content of a webpage.
  ### CSS Saves A Lot of Work!
  - Style definitions are stored in .css files.
  - One file can change the single look of a web page.
## CSS Syntax and Selectors
  ### CSS Syntax
  - ![CSS Syntax](https://github.com/caofontaine/Notes/blob/master/CSS/img/syntax.png "CSS Syntax")
	* Selector - HTML element you want to style
    * Declaration block - one or more declarations separated by semi-colon
    * Each declaration has a property name and value.
  ### CSS Selectors
  - Used to “find” HTML elements based on their element name, id, class, attribute, etc.
  ### The element Selector
  - Selects elements based on element name.
  - Ex. &lt;p&gt; = p
  ### The id Selector
  - Uses the id attribute of an HTML element to select a specific element
  - To select an element based on id, use # with id name.
  ### The class Selector
  - Uses the class attribute of an HTML element to select a specific element
  - To select an element based on class, use . with class name.
  - p.classname to style select HTML element with that class name.
  ### Grouping Selectors
  - You can group elements with the same styling by separating each element with a comma before beginning the declaration block.
  ### CSS Comments
  - Help explain the code. Enclosed in /* */
## CSS How To…
  ### Three Ways to Insert CSS
  - External style sheet
  - Internal style sheet
  - Inline style
  ### External Stylesheets
  - You can change the look of a web page by including a file.
  - In the &lt;head&gt; include a &lt;link&gt; which has the path to your stylesheet.
  - ```<link rel="stylesheet" type="text/css" href="mystyle.css">```
  ### Internal Stylesheets
  - Can be used if a page has one single style.
  - Enclosed in &lt;style&gt; inside &lt;head&gt;
  ### Inline Styles
  - Apply a unique style for a single element.
  - Use style attribute on the relevant element.
  ### Multiple Stylesheets
  - If properties are defined for a selector in multiple stylesheets, then the value from the last read stylesheet will be used.
  ### Cascading Order
  - Inline style, External & Internal Stylesheets, Browser Default
## CSS Colors
CSS colors are specified by:
- a valid color name - like "red"
- an RGB value - like "rgb(255, 0, 0)"
- a HEX value - like "#ff0000"
## CSS Backgrounds
Defines the background effects for elements.
  ### Background Color
  - Denoted by background-color, changes the background color of an element.
  - Color values can be by name, RGB, or HEX.
  ### Background Image
  - Denoted by background-image, specifies an image to be used as a background.
  - ```background-image: url("paper.gif");```
  ### Background Image - Repeat Horizontally or Vertically
  - ```background-repeat: repeat-x (or repeat-y);```
  ### Background Image - Set position and no-repeat
  - ```background-repeat: no-repeat;```
  - ```background-position: right top;```
  ### Background Image - Fixed Position
  - Use background-attachment property to make image not scroll with the rest of the page.
  - ```background-attachment: fixed;```
  ### Background Image - Shorthand Property
  - You can use the shorthand property, denoted as “background” to avoid individually writing declarations for each background effect.
  - ```background: #ffffff url("img_tree.png") no-repeat right top;```
  - When writing in shorthand, the order is as follows:
    * background-color
    * background-image
    * background-repeat
    * background-attachment
    * background-position
## CSS Borders
Allows you to specify the style, width, and color of an element’s border.
  ### Border Style
  - The border-style property defines what kind of border to display.
    * dotted - Defines a dotted border
    * dashed - Defines a dashed border
    * solid - Defines a solid border
    * double - Defines a double border
    * groove - Defines a 3D grooved border. The effect depends on the border-color value
    * ridge - Defines a 3D ridged border. The effect depends on the border-color value
    * inset - Defines a 3D inset border. The effect depends on the border-color value
    * outset - Defines a 3D outset border. The effect depends on the border-color value
    * none - Defines no border
    * hidden - Defines a hidden border
  - It can have one to four values (top, right, bottom, left).
  ### Border Width
  - The border-width property specifies the width of the four borders
  - The width can be set as a specific size (in px, pt, cm, em, etc) or by using one of the three pre-defined values: thin, medium, or thick.
  - The border-width property can have from one to four values (top, right, bottom, left).
  ### Border Color
  - The border-color property is used to set the color of the four borders.
  - Color can be set by name, RGB, or HEX.
  - The border-color property can have from one to four values (top, right, bottom, left). 
  - If border-color is not set, it inherits the color of the element.
  ### Border - Individual Sides
  - You can specify each of the border (top, right, bottom, left).
  - ```
       p {
         border-top-style: dotted;
         border-right-style: solid;
         border-bottom-style: dotted;
         border-left-style: solid;
       }
	```
  - If border-style has two properties:
    * border-style: dotted solid;
      - top and bottom borders are dotted
      - right and left borders are solid
  ### Border - Shorthand Property
  - You can use the shorthand, denoted has “border”. Order as follows
    * border-width
    * border-style (required)
    * border-color
  - ```border: 5px solid red;```
  - Shorthand can be done for individual sides of a border as well.
    * border-left: 6px solid red;
  ### Rounded Borders
  - The border-radius property is used to add rounded corners to a border.
    * ```border-radius: 5px;```
  - Not available in IE8 or older browsers.
## CSS Margins
Used to generate space between elements.
Properties set the size of the white space outside the border.
You can set the margin for each side  - top, right, bottom, left
  ### Margin - Individual Sides
  - margin-top
  - margin-right
  - margin-bottom
  - margin-left
  - All margin properties can have the following values:
    * auto - the browser calculates the margin
    * length - specifies a margin in px, pt, cm, etc.
    * % - specifies a margin in % of the width of the containing element
    * inherit - specifies that the margin should be inherited from the parent element
  ### Margin - Shorthand Property
  - Just use shorthand “margin” to define top, right, bottom, left margin sides.
  - ```margin: 100px 150px 100px 80px;```
  ### The auto Value
  - Setting the margin property to auto will center the element within its container.
  - The element will then take up the specified width, and the remaining space will be split equally between the left and right margins.
  ### The inherit Value
  - Allows the margin property to be inherited from its parent container element.
  ### Margin Collapse
  - Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest of the two margins.
  - This does not happen on left and right margins. Only top and bottom margins.
  - ```
       h1 {
         margin: 0 0 50px 0;
       }

       h2 {
         margin: 20px 0 0 0;
       }
    ```
    * In the example above, the &lt;h1&gt; element has a bottom margin of 50px. The &lt;h2&gt; element has a top margin set to 20px.
	* Common sense would seem to suggest that the vertical margin between the &lt;h1&gt; and the &lt;h2&gt; would be a total of 70px (50px + 20px). But due to margin collapse, the actual margin ends up being 50px.
## CSS Padding
Generate space around content.
Clears an area around the content (inside the border) of an element.
Can set the padding for each side - top, right, bottom, left
  ### Padding - Individual Sides
  - padding-top
  - padding-right
  - padding-bottom
  - padding-left
  - All margin properties can have the following values:
    * length - specifies a margin in px, pt, cm, etc.
    * % - specifies a margin in % of the width of the containing element
    * inherit - specifies that the margin should be inherited from the parent element
  ### Padding - Shorthand Property
  - Just use shorthand “padding” to define top, right, bottom, left padding sides
  - ```padding: 50px 30px 50px 80px;```
## CSS Height and Width
Set the height and width of an element.
Can be set 3 ways:
1. Auto (browser sets it)
2. length values, like px, cm, etc.
3. A percent of the containing block
  ### Setting max-width
  - Sets maximum width of an element.
    * Can be specified in 3 ways:
      - length values, like px, cm, etc.
      - A percent of the containing block
      - none - meaning no maximum width
  - Issues will arise when browser window is smaller than specified width.
  - max-width overrides width property
## CSS Box Model
A box that wraps around every HTML element. Consists of margins, borders, padding, and the actual content.
![CSS Box Model](https://github.com/caofontaine/Notes/blob/master/CSS/img/boxmodel.png "CSS Box Model")
Content - The content of the box, where text and images appear
Padding - Clears an area around the content. The padding is transparent
Border - A border that goes around the padding and content
Margin - Clears an area outside the border. The margin is transparent
  ### Width and Height of an Element
  - Setting the width and height only measures the content area.
  - To calculate the full width and height of any element, you must add the margins, border, and padding sizes along with the content width and height sizes.
  - Total element width = width + left padding + right padding + left border + right border + left margin + right margin
  - Total element height = height + top padding + bottom padding + top border + bottom border + top margin + bottom margin
## CSS Outline
Specify style, color, and width of an outline.
Drawn around the element, outside the border, to make it “stand out”.
Not part of the element’s dimensions, or part of the total width and height of the element.
  ### Outline Style
  - Specifies the style of the outline.
    * dotted - Defines a dotted outline
    * dashed - Defines a dashed outline
    * solid - Defines a solid outline
    * double - Defines a double outline
    * groove - Defines a 3D grooved outline. The effect depends on the outline-color value
    * ridge - Defines a 3D ridged outline. The effect depends on the outline-color value
    * inset - Defines a 3D inset outline. The effect depends on the outline-color value
    * outset - Defines a 3D outset outline. The effect depends on the outline-color value
    * none - Defines no outline
    * hidden - Defines a hidden outline
  ### Outline Color
  - Sets the color of the outline.
  - Color is set by:
    * name - specify a color name, like "red"
    * RGB - specify a RGB value, like "rgb(255,0,0)"
    * Hex - specify a hex value, like "#ff0000"
    * invert - performs a color inversion (which ensures that the outline is visible, regardless of color background)
  ### Outline Width
  - Specifies the width out an outline.
  - Can be set by:
    * A specific size (in px, pt, cm, em, etc)
    * By using one of the three pre-defined values: thin, medium, or thick
  ### Outline - Shorthand Property
  - Can specify all options in “outline” property.
    * outline-width
    * outline-style (required)
    * outline-color
    * outline: 5px dotted red;
## CSS Text
  ### Text Color
  - Sets the color of the text.
  - Specified by:
    * a color name - like "red"
    * a HEX value - like "#ff0000"
    * an RGB value - like "rgb(255,0,0)"
  ### Text Alignment
  - The "text-align" property sets the horizontal alignment of content.
  - Can be set left or right aligned, centered, or justified.
    * Justify value stretches the lines so that each line has equal width (like in newspapers and magazines)
  ### Text Decoration
  - The "text-decoration" property sets or removes decorations from text.
  - The value text-decoration: none; is often used to remove underlines from links
  ### Text Transformation
  - "text-transform" property changes text to uppercase or lowercase, or capitalize the first letter of each word.
  ### Text Indentation
  - "text-indent" specifies the indentation of the first line of text.
  ### Letter Spacing
  - "letter-spacing" specifies space between characters in text.
  ### Line Height
  - "line-height" specifies space between lines
  ### Text Direction
  - "direction" property changes the text direction of an element.
  - ```direction: rtl;```
  ### Word Spacing
  - "word-spacing" specifies the space between words in text.
  ### Text Shadow
  - "text-shadow" adds shadow to text.
  - ```text-shadow: 3px 2px red;```
    * horizontal shadow (3px)
    * vertical shadow (2px) 
    * color of the shadow (red)
## CSS Fonts
The CSS font properties define the font family, boldness, size, and the style of a text.
  ### Difference Between Serif and Sans-serif Fonts
  - ![CSS Fonts](https://github.com/caofontaine/Notes/blob/master/CSS/img/serif.gif "CSS Fonts")
  ### CSS Font Families
  - generic family - a group of font families with a similar look (like "Serif" or "Monospace")
  - font family - a specific font family (like "Times New Roman" or "Arial")
  - ![CSS Font Table](https://github.com/caofontaine/Notes/blob/master/CSS/img/fonttable.png "CSS Font Table")
  ### Font Family
  - "font-family" sets the font family.
  - Can hold several font names as a fallback system. If the first one isn’t available, it uses the next one.
    * Pick a specific font first, then end with a generic family.
    * ```font-family: "Times New Roman", Times, serif;```
  ### Font Style
  - "font-style" sets the style of your font. Mostly is used for italics.
  - Property has 3 values:
    * normal - The text is shown normally
    * italic - The text is shown in italics
    * oblique - The text is "leaning" (oblique is very similar to italic, but less supported)
  ### Font Size
  - "font-size" sets the size of the text.
  - Font size can be absolute or relative size.
    * Absolute
      - Sets the text to a specified size
      - Does not allow a user to change the text size in all browsers (bad for accessibility reasons)
      - Absolute size is useful when the physical size of the output is known
    * Relative
      - Sets the size relative to surrounding elements
      - Allows a user to change the text size in browsers
  - If you do not specify a font size, the default size for normal text, like paragraphs, is 16px (16px=1em).
  ### Set Font Size With Pixels
  - ```font-size: 40px;```
  ### Set Font Size With Em
  - Allows user to resize text in browser menu.
  - W3C recommended unit.
  - pixels/16=em
  - ```font-size: 2.5em; /* 40px/16=2.5em */```
  ### Use A Combination of Percent and Em
  - Setting font size in percent and em allows the same size in all browsers and allows the browsers to resize the text.
  ### Font Weight
  - "font-weight" specifies weight of a font.
  - ```font-weight: bold;```
  ### Font Weight
  - "font-variant" specifies whether or not text should be displayed in small-caps font.
  - In a small-caps font, all lowercase letters are converted to uppercase letters. However, the converted uppercase letters appears in a smaller font size than the original uppercase letters in the text.
## CSS Icons
Simplest way to add icons is to add an external library.
Use the icon specified class from that library on any inline element.
## CSS Links
  ### Styling Links
  - Links can be styled with any property.
  - Links can be styled depending on what state they’re in.
    * a:link - a normal, unvisited link
    * a:visited - a link the user has visited
    * a:hover - a link when the user mouses over it
    * a:active - a link the moment it is clicked
    * When you edit the style each state, you must follow these rules:
      - a:hover MUST come after a:link and a:visited
      - a:active MUST come after a:hover
  ### Text Decoration
  - "text-decoration" is used typically to remove underlines from links.
  ### Background Color
  - "background-color" is used to change the background color of links.
  ### Advanced - Link Buttons
  - ```
       a:link, a:visited {
         background-color: #f44336;
         color: white;
         padding: 14px 25px;
         text-align: center; 
         text-decoration: none;
         display: inline-block;
       }

       a:hover, a:active {
         background-color: red;
       }
    ```
    * ![CSS Link Button](https://github.com/caofontaine/Notes/blob/master/CSS/img/linkbutton.png "CSS Link Button")
## CSS Lists
  ### HTML Lists and CSS List Properties
  - HTML lists - ordered (&lt;ol&gt;) & unordered (&lt;ul&gt;)
  - CSS list properties allow you to:
    * Set different list item markers for ordered  and unordered lists
    * Set an image as the list item marker
    * Add background colors to lists and list items
  ### Different List Item Markers
  - "list-style-type" specifies the type of list item marker
  ### An Image As The List Item Marker
  - "list-style-image" specifies an image as the list item marker
  - ```list-style-image: url('sqpurple.gif');```
  ### Position The List Item Markers
  - "list-style-position" specifies whether the list item marker should be inside or outside content flow
    * "outside" is the default setting
  ### Remove Default Settings
  - Set list-style-type to “none” to remove markers/bullets
  - Since lists have margins and padding, set those properties to 0.
  ### List - Shorthand Property
  - "list-style" is the shorthand
  - ```list-style: square inside url("sqpurple.gif");```
    * list-style-type (if a list-style-image is specified, the value of this property will be displayed if the image for some reason cannot be displayed)
    * list-style-position (specifies whether the list-item markers should appear inside or outside the content flow)
    * list-style-image (specifies an image as the list item marker)
      - If one of the property values is missing, it will take its default value.
  ### Styling List With Colors
  - Anything added to the &lt;ol&gt; or &lt;ul&gt; tags will affect the inner &lt;li&gt; tags.
## CSS Tables
  ### Table Borders
  - Specify border for &lt;table&gt;, &lt;th&gt;, and &lt;td&gt; using "border" property.
  ### Collapse Table Borders
  - Use "border-collapse" property if you want table borders to be collapsed into a single border.
  ### Table Width and Height
  - Just use "width" and "height" properties on table.
  ### Horizontal Alignment
  - Use "text-align" property to set text to be left, right, or center.
  - &lt;th&gt; is center aligned by default.
  ### Vertical Alignment
  - Use "vertical-align" to set vertical alignment to be top, middle, or bottom.
  - For &lt;th&gt; and &lt;td&gt;, middle is the default value.
  ### Table Padding
  - Use "padding" put space between border and content.
  ### Horizontal Dividers
  - Use "border-bottom" on &lt;th&gt; and &lt;td&gt; to set horizontal dividers.
  ### Hoverable Tables
  - Use ":hover" selector on &lt;tr&gt; to highlight table rows when hovered over it.
  - ```tr:hover {background-color: #f5f5f5}```
  ### Striped Tables
  - Use "nth-child()" selector to add "background-color" to even or odd rows.
  - ```tr:nth-child(even) {background-color: #f2f2f2}```
  ### Table Color
  - Use "background-color" to set background color of table elements.
  - Use "color" set text color of table elements.
  ### Responsive Table
  - Use container element with "overflow-x: auto" to make a table responsive.
  - Will display a horizontal scroll bar if table is viewed in a small screen
## CSS Display
  ### The display Property
  - The "display" property determines if/how an element is displayed.
  - Default "display" value is block or inline.
  ### Block-level Elements
  - Block-level elements always start on a new line and takes the full width available.
  - Example of elements - &lt;div&gt;, &lt;h1&gt;-&lt;h6&gt;, etc.
  ### Inline Elements
  - Inline elements don’t start on a new line and only takes as much width necessary.
  - Example of elements - &lt;a&gt;, &lt;span&gt;, &lt;img&gt;
  ### Display: none;
  - Commonly used with JavaScript to show or hide elements without deleting them.
  ### Override The Default Display Value
  - You can override the default display value for any element by going from inline to block, or vise-versa.
  ### Hide An Element - display: none or visibility: hidden?
  - display: none will hide an element and the page is displayed as if the element doesn’t exist
  - visibility: hidden will hide an element, but the page layout will be shown as if the element was still there
## CSS Max-width
  ### Using width, max-width, and margin: auto;
  - Setting the width of a block-level element will prevent it from stretching to the full width available.
  - Setting the margin to auto will horizontally center the element within its container.
  - Using “max-width” will prevent a scroll bar from appearing when viewing the page on a smaller screen.
## CSS Position
  ### The position Property
  - Specifies type of positioning method used for an element.
  - There are 4 position values:
    * static
    * relative
    * fixed
    * absolute
      - Elements are positioned by top, bottom, left, right properties.
      - This doesn’t work unless a position is defined, they also work differently for each type of positioning.
  ### position: static;
  - HTML elements are positioned static by default.
  - Positioned according to the normal flow of the page.
  ### position: relative;
  - HTML elements are positioned relative to its normal position.
  - Any settings on the top, right, bottom, or left properties will position the element away from its normal positioning.
  - Other content will not be adjusted to fit into the gap left by the element.
  ### position: fixed;
  - HTML elements are position relative to the viewport, meaning it is always in the same position even if the page is scrolled.
  - A fixed element doesn’t leave a gap in the page where it normally is.
  ### position: absolute;
  - HTML elements are positioned relative to the nearest positioned ancestor
  - If an absolute positioned element has no ancestor, it uses the document body, which then moves along with page scrolling.
  ### Overlapping Elements
  - The "z-index: property specifies the stack order of an element (which element is in front of the other).
## CSS Overflow
The "overflow" property specifies whether to clip content or add scroll bars when the content is too big to fit in a specified area.
The property has the following values:
- visible - Default. The overflow is not clipped. It renders outside the element's box
- hidden - The overflow is clipped, and the rest of the content will be invisible
- scroll - The overflow is clipped, but a scrollbar is added to see the rest of the content
- auto - If overflow is clipped, a scrollbar should be added to see the rest of the content
  ### overflow: visible
  - Overflow is visible by default, meaning content is not clipped and will render outside an element’s box.
  ### overflow: hidden
  - The overflow is clipped and the rest of the content is hidden.
  ### overflow: scroll
  - Overflow is clipped and scroll bar is shown inside the content box.
  ### overflow: auto
  - Only adds scroll bars when necessary.
  ### overflow-x and overflow-y
  - Specifies what to do to overflow horizontally and vertically.
## CSS Float
The float property specifies whether or not an element should float.
The clear property is used to control the behavior of floating elements.
  ### The float Property
  - Can be used to wrap text around images
  ### The clear Property
  - Used to control the behavior of floating elements
  - Elements after a floating element will flow around it. To avoid this, use the clear property.
  - The clear property specifies on which sides of an element floating elements are not allowed to float
  ### The clearfix Hack
  - If an element is taller than the element containing it, and it is floated, it will overflow outside of its container.
  - Then we can add overflow: auto; to the containing element to fix this problem
    * Works as long as you control margins and padding (or you get scrollbars)
  - More modern clearfix hack
    * ```
	     .clearfix::after {
           content: "";
           clear: both;
           display: table;
         }
	  ```
## CSS Inline-block
Using "inline-block" value of "display" property can create a grid of boxes that fills the browser width and wraps when the browser is resized.
## CSS Align
  ### Center Align Elements
  - Horizontally center a block element by setting margin: auto
  - Setting the width of the element will prevent it from stretching out to the edges of its container.
  - The element will then take up the specified width, and the remaining space will be split equally between the two margins.
  ### Center Align Text
  - Use "text-align" property with “center” value.
  ### Center An Image
  - Use margin: auto and display: block to make it a block element.
  ### Left and Right Align - Using position
  - Using position: absolute is one way to align elements left or right.
  ### Left and Right Align - Using float
  ### Center Vertically - Using padding
  - Use padding to center elements vertically.
  - To center elements horizontally and vertically, use padding and text-align.
  ### Center Vertically - Using line-height
  - Another trick is to use the line-height property with a value that is equal to the height property.
  ### Center Vertically - Using position & transform
  - ```
       .center p {
         margin: 0;
         position: absolute;
         top: 50%;
         left: 50%;
         transform: translate(-50%, -50%);
       }
    ```
## CSS Combinators
A combinator is something that describes the relationship between selectors.
There are four different combinators in CSS3:
- selector (space)
- child selector (>)
- adjacent sibling selector (+)
- general sibling selector (~)
  ### Descendant Selector
  - Matches all elements that are descendants of a specified element.
  - div p
  ### Child Selector
  - Selects all elements that are the immediate child of a specified element.
  - div > p
  ### Adjacent Sibling Selector
  - Selects all elements that are the adjacent siblings of a specified element.
  - Sibling elements must have the same parent, and "adjacent" means "immediately following".
  - div + p
    * Selects all &lt;p&gt; elements that are placed immediately after &lt;div&gt;
  ### General Sibling Selector
  - Selects all elements that are siblings of a specified element.
  - div ~ p
    * Selects all &lt;p&gt; elements that are siblings of &lt;div&gt;
## CSS Pseudo-classes
  ### What Are Pseudo-Classes?
  - Used to define the special state of an element.
  - Examples:
    * Style an element when a user mouses over it
    * Style visited and unvisited links differently
    * Style an element when it gets focus
    * ```
	     selector:pseudo-class {
           property:value;
         }
	  ```
  ### Anchor Pseudo-Classes
  ### Pseudo-classes and CSS Classes
  - Can combine a pseudo-class with a CSS class.
  - ```
       a.highlight:hover {
         color: #ff0000;
       }
    ```
  ### Hover on &lt;div&gt;
  ### Simple Tooltip Hover
  ### The :first-child Pseudo-class
  - Matches the specified element that is the first child of another element.
  ### Match the first &lt;i&gt; element in all &lt;p&gt; elements
  ### Match all &lt;i&gt; elements in all first child &lt;p&gt; elements
  ### The :lang Pseudo-class
  - Define special rules for different languages.
## CSS Pseudo-elements
  ### What Are Pseudo-Elements?
  - Used to style different parts of an element.
  - Examples:
    * Style the first letter, or line, of an element
    * Insert content before, or after, the content of an element
    * ```
	     selector::pseudo-element {
           property:value;
         }
	  ```
  ### The ::first-line Pseudo-element
  - Adds special style to the first line of an element.
  - ``` p::first-line ```
  - Can only be applied to block level elements.
  ### The ::first-letter Pseudo-element
  - Adds special style to the first letter of a text.
  - ``` p::first-letter ```
  - Can only be applied to block level elements.
  ### Pseudo-elements and CSS Classes
  - Pseudo-elements can be combined with CSS classes
  - ``` p.intro::first-letter ```
  ### Multiple Pseudo-Elements
  - The ::before Pseudo-element
  - Inserts content before the content of an element.
  - ``` h1::before ```
  ### The ::after Pseudo-element
  - Inserts content after the content of an element.
  - ``` h1::after ```
  ### The ::selection Pseudo-element
  - Matches portion of an element selected by user.
  - color, background, cursor, and outline properties can be applied to it.
  - ``` ::selection ```
## CSS Opacity
The "opacity" property specifies the opacity/transparency of an element.
  ### Transparent Image
  - The "opacity" property can take a value from 0.0-1.0. The lower the value, the more transparent.
  ### Transparent Hover Effect
  - By using the :hover selector, you can change the opacity of an element by mousing over.
  ### Transparent Box
  - When setting the opacity of an element, if there are other elements nested inside it, it will inherit the same opacity.
  ### Transparency Using RGBA
  - If you don’t want child elements inheriting opacity, you can use the rgba color value (red, green, blue, alpha). The alpha parameter will be your opacity.
  - ``` rgba(76, 175, 80, 0.3) ```
  ### Text In A Transparent Box
  - When setting the opacity of an element, if there are other elements nested inside it, it will inherit the same opacity.
## CSS Navigation Bar
  ### Navigation Bar = List of Links
  - Needs standard HTML as a base.
  - A list of links, so &lt;ul&gt; and &lt;li&gt; elements.
  ### Vertical Navigation Bar
  - Can style &lt;a&gt; elements in the list to build a vertical navigation bar.
  ### Horizontal Navigation Bar
  - Can be done either using inline or floating list items.
  - Inline List Items:
    * Set &lt;li&gt; element’s "display" to be inline since they are by default block elements.
  - Floating List Items:
    * Set the "float" property so list items can slide next to each other.
## CSS Dropdowns
  ### Basic Dropdown
  - Use any element to open the dropdown (&lt;span&gt;, &lt;button&gt;, etc.)
  - Use a &lt;div&gt; to wrap around dropdown content.
  - Wrap all content in a &lt;div&gt; to position the dropdown.
  - The .dropdown class is needed to be position: relative in order to have dropdown content right below it using position: absolute.
  - .dropdown-content will be hidden, but appears on hover.
## CSS Tooltips
  ### Basic Tooltip
  - Use a container element (like &lt;div&gt;) and add the "tooltip" class to it. When the user mouse over this &lt;div&gt;, it will show the tooltip text.
  - The tooltip text is placed inside an inline element (like &lt;span&gt;) with class="tooltiptext".
  - The tooltip class uses position:relative, which is needed to position the tooltip text (position:absolute).
  - The tooltiptext class holds the actual tooltip text. It is hidden by default, and will be visible on hover.
  - The CSS3 border-radius property is used to add rounded corners to the tooltip text.
  - The :hover selector is used to show the tooltip text when the user moves the mouse over the &lt;div&gt; with class="tooltip".
## CSS Image Gallery
## CSS Image Sprites
## CSS Attr Selectors
  ### Style HTML Element With Specific Attributes
  - It is possible to style HTML elements that have specific attributes or attribute values.
  ### CSS [attribute] Selector
  - [attribute] selector is used to select element with a specific attribute.
  - a[target]
    * Selects all &lt;a&gt; elements with "target" attribute.
  ### CSS [attribute="value"] Selector
  - [attribute="value"] is used to select elements with a specific attribute value.
  - a[target="_blank"]
    * Selects all &lt;a&gt; elements that have a "target" attribute value of "_blank".
  ### CSS [attribute~="value"] Selector
  - [attribute~="value"] is used to select elements with a specific attribute value with a specific word.
  - [title~="flower"]
    * selects all elements with a title attribute that contains a space-separated list of words, one of which is "flower"
  ### CSS [attribute|="value"] Selector
  - [attribute|="value"] is used to select elements with a specific attribute value starting with a specified value.
  - [class|="top"]
    * Selects all elements that have a class value of "top".
    * Value must be a whole word, “top” alone, or separated with a hyphen.
  ### CSS [attribute^="value"] Selector
  - [attribute^=”value”] is used to select elements whose attribute value begins with a specified value.
  - [class^="top"]
    * Selects all elements that have a class value of "top".
    * Doesn’t have to be a whole word.
  ### CSS [attribute$="value"] Selector
  - [attribute$="value"] is used to select elements whose attribute value ends with a specified value.
  - [class$="test"]
    * Doesn’t have to be a whole word.
  ### CSS [attribute*="value"] Selector
  - [attribute*="value"] is used to select elements whose attribute value contains a specified value.
  - [class*="te"]
    * Doesn’t have to be a whole word.
  ### Styling Forms
## CSS Forms
  ### Styling Input Fields
  - To select a specific input field, use input[type=&lt;input_type&gt;]
## CSS Counters
"Variables" maintained by CSS rules
  ### Automatic Numbering With Counters
  - counter-reset - Creates or resets a counter
  - counter-increment - Increments a counter value
  - content - Inserts generated content
  - counter() or counters() function - Adds the value of a counter to an element
  - ```
       body {
	     counter-reset: section;
       }

       h2::before {
	     counter-increment: section;
	     content: "Section " counter(section) ": ";
       }
    ```
  ### Nesting Counters

