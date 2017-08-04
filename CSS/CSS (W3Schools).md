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
  - ```p {
         border-top-style: dotted;
         border-right-style: solid;
         border-bottom-style: dotted;
         border-left-style: solid;
       }```
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



