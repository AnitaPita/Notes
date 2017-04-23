# Chapter 4: Introduction to CSS, Part 1

## 4.1: Intro
* **CSS:** Used to specify the presentation of elements separately from the content and structure of the document.
* `jigsaw.w3.org/css-validator/`: CSS validator

## 4.2: Inline Style
**Inline Style:** declare the format of an individual element using the HTML5 attribute `style`.
* e.g. `<p style = "font-size: 20pt; color: red;">`

`color` property sets text color using either **color names** or **hexadecimal code** (e.g. #FF00FF is purple b/c it's #RRGGBB)

## 4.3: Embedded Style Sheets
**Embedded:** embed a CSS3 document in an HTML5 document’s `head` section, using the style element. 

`<style type = "text/css">
em { font-weight: bold;
color: black; }
h1 { font-family: tahoma, helvetica, sans-serif; }
p { font-size: 12pt;
font-family: arial, sans-serif; }
.special { color: purple; }
</style>`

* Styles that are placed in a style element use selectors to apply style elements throughout the **entire** document
* Style element’s type attribute specifies the MIME type (the specific encoding format) of the style sheet. Style sheets use **text/css**
  * Other examples = image/png, text/javascript
* Each rule body in a style sheet is enclosed in curly braces, i.e., { and }.
* **`em`:** its contents should be emphasized
* **Syntax** = selector string {property name : value} (many different declarations can be in here too)
* **`font-weight`:**  specifies the “boldness” of text (e.g. `bold`, `normal`(400), `bolder`, `lighter`, multiple of 100 up to 900)
* **Style classes:** preceded by a period, define styles that apply to elements in particular class. OR can declare id selectors.
  * How to declare: `<p class = "special"></p>`
* **`font-family`:** specifies the name of the font to use; last item in font-family list should be generic in case a browser does not support a specific font.
* **`font-size`:** specifies the size used to render the font
  * Can be specified by *absolute size* (pt, mm, pc) or *relative size* (in em, ex or in xxs/xs/smaller/small/medium/large/larger etc) but **relative is preferred.**

## 4.4: Conflicting Styles
1) Styles may be defined by a user, an author or a user agent. **User agent < User < Author**. 
2) Most styles defined for parent elements are inherited by child (nested) elements, but in conflict **descendant property > ancestor property**.
* **`text-decoration`:** applies decorations to text in an element. (e.g. `none`, `underline`, `overline`, `line-through`, `blink`)
* **Pseudoclass:** give you access to content that’s not declared in the document. Format = `:hover {}`
  * **`hover`:**  activated when the user moves the mouse cursor over an element

## 4.5: Linking External Style Sheets
**External style sheets:** separate documents that contain only CSS rules
* **Skinning:** need to modify only a single CSS file to make style changes across all the pages that use those styles
* CSS document: just start doing `body {} a:hover {} ul {}` etc in a `x.css` file
  * Linking in HTML: `<link rel = "stylesheet" type "text/css" href = "x.css">`

## 4.6: Absolute Positioning and Z-index
**`position`:** absolute or relative. ABSOLUTE positions it according to the distance from the top, right, bottom or left margin of its containing block element
* **`z-index`:** layer overlapping elements (high z-index = front)

## 4.7: Relative Positioning and Span
**Relative positioning:** elements are positioned relative to other elements
**Inline Element:** does not change the flow of the document. e.g `img`, `a`, `em`, `span`, `strong`.
**Block Element:** Displayed on their own line, have virtual boxes around them, e.g. `p`, headings, `div`
  * Can contain inline elements, but inline elements can't contain block elements

## 4.8: Backgrounds
CSS can control backgrounds of block-lvl elements by adding **color** or **image**.
* **`background-image`:** Specifies the URL of the image, in the format `url(logo.png)`
* **`background-position`:** Places the image on the page using the values `top`, `right`, `bottom`, `left` and `center` OR use  horizontal length followed by vertical length (e.g. `background-position: 50% 30px;`)
* **`background-repeat`:** tiles the background image: can be `repeat`, `no-repeat`, `repeat-x` or `repeat-y`
* **`background-attachment: fixed`** Fixes the image in the position specified by `background-position`(default = `scroll`, so with `fixed` the image won't move as you scroll down the page)
* **`text-indent`:** Indents the first line of text in the element by the specified amount 
* **`font-style`:** either `normal`, `italic`, or `oblique`

## 4.9: Element Dimensions
* **`width` and `height`:** can be relative (%) or absolute
* **`text-align`:** can be `center`, `justify`, `left` or `right`.
* **`overflow`:** Content might sometimes exceed the set boundaries, in which case the element must be made large enough for all the content to fit. If `overflow:scroll`, puts a scroll bar, otherwise can be `visible` (default) or `hidden`. 

## 4.10: Box Model and Text Flow
Consists of:
* Content height/width
* padding-(bottom, left, top, right)
* border-x-width(where x = bottom, left, top, right) (can be: thin, medium or thick)
  * Other border elements: `border-color`, `border-style` (none, hidden, dotted, dashed, solid, etc)
* margin-(bottom, left, top, right)
* Whole thing: box height/width

**Floating elements:**  allows you to move an element to one side of the screen; other content in the document then flows around the floated element. (e.g. for a `.floated` css class, make `<h1 class = "floated"></h1>` in the HTML doc.

## 4.11: Media Types/Media Queries
**CSS Media types:** allow you to decide what a page should look like depending on the kind of media being used to display the page; most common = `screen`
* `handheld` = mobile, `braille` = machines that can read/print web in braille, `speech` = speech-synthesizing browser, `print` = how web page is affected when printed
* use `@media all` (or replace all with any of the above) before a block of styles surrounded by curly braces.
  * e.g `print` should be a lighter-coloured background version of `screen`. 
* Media queries are described in the next section, but examples are width, height, device-width, device-height, orientation, aspect-ratio, and device-aspect-ratio.

## 4.12: Drop-Down Menus
Parts of the drop down (use a combo of `:hover` and `display`):
* `body { /* some styles*/}`
* `nav {/* some styles*/}`
* `nav ul {display: none; list-style: none;}` i.e when not over list, you don't want to show options
* `nav:hover ul {display:block;} i.e show the display of drop-down when hovering over nav bar
* `nav ul li {background-color:white;}
* `nac ul li:hover {background-color: powderblue;} i.e highlight the item when hovering over it
