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
  - ![CSS Syntax](https://github.com/caofontaine/Notes/tree/master/CSS/img/syntax.png "CSS Syntax")
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

