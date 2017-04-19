# Chapter 2: Introduction to HTML, Part 1

## 2.1: Introduction
Will look at tables, forms, internal linking, and meta elements.

## 2.2: Editing HTML5
You edit HTML5 docs in **editors** (e.g. Notepad, TextEdit, vi, emacs) and save with .html
* **Web servers:** store HTML5 docs
* **Clients:** (e.g web browsers running on local computers) request specific resources like HTML5 docs from web servers.

## 2.3: First HTML HTML5 Example
* **DOCTYPE:** required in HTML5 documents so that browsers render the page in standards mode.
   * **Quirks Mode:** Some browsers open in this mode to maintain backward compatibility with web pages that are not up-to-date with the latest standards
* **Comments:** improve readability and describe the content of a document. Uses  \<!-- and end with -->
* **`Head`:** contains information about the HTML5 document, such as the character set (UTF-8, the most popular character-encoding scheme for the web) that the page uses, which helps the browser determine how to render the content and title of the page. 
  * can also contain CSS3 style sheets, and scripts for creating dynamic web pages. 
  * Nested in between the \<html> start and end tags
* **`Body`:**  contains the page’s content, which the browser displays when the user visits the web page.

### Tags
* **Start Tags:** consists of the element name in angle brackets. For example, `<html>` 
* **End Tags:** consists of the element name preceded by a forward slash (/) in angle brackets. For example, \</html>
* **Void Tags/Empty Elements:** Do not have end tags.

**Attributes:** provide additional information about an element, which browsers use to determine how to process the element.
* Each attribute has a **name** and a **value** separated by an equals sign (=). E.g. `<meta charset = “utf-8”>`
* **Good practices:** use lowercase letters for elements. Also, use 3 spaces for each level of indentation.

**Title Element:** Enclosed in the head element's start and end tags; describes the web page
* Usually appears in title bar of browser window. Also used to ID  a page when users add the page to their list of Favorites or Bookmarks.

**Paragraph Element:** All text placed between the `<p>` and `</p>` tags forms one paragraph. 
* When a browser renders a paragraph, it places extra space above and below the paragraph.

## 2.4: W3C HTML5 Validation Example
* Validation services ensure that an HTML5 doc is syntactically correct to make sure it displays properly. Use something like **W3C MarkUp Validation Service**.

## 2.5: Headings
**h1 through h6:** specify relative importance of information.
* Since text size varies between browsers, we use CSS to control text size more stringently.
* Placing a heading @ top of each pg helps viewers understand the purpose of the pg. They can also create an outline and are indexed by search engines.

## 2.6: Linking
* **Hyperlink:** references or links to other resources, such as HTML5 documents and images. Typically underlined and colored blue.
* **`strong` element:** content has high importance. Usually rendered bold. 
* **anchored (`a`) element:** used in creating links.
* **`href` (hypertext reference):** specifies a resource's location, such as a web page/location within a web page, a file, or an email address
  * What if URL doesn't indicate a specific document? Web server returns a default web page "index.html"; this can be configured. 
  * Good practice: enclose attribute values in either single or double quotation marks.
  * **404 error:** If the web server cannot locate a requested document.
* **Hyperlinking to an E-mail address:** use mailto: `emailAddress`. launch the default e-mail program (e.g., Mozilla Thunderbird, Microsoft Outlook or Apple Mail) to enable the user to write an e-mail message to the linked address. 
* **Relative URL:** Location relative to a base URL.

## 2.7: Images
* **PNG and JPEG:** Most popular img formats.
* **Image-editing software:** Adobe Photoshop, G.I.M.P, Inkscape.
* Format: `<img src = "" width = "" height = "" alt = "">`
* **`src`** specifies image's location
* **`alt`** contains text that is displayed if the client cannot render the image. Also important for accessibility.
* **`Width` and `height`:** Optional, but if omitted, browser uses image's actual width and height; measured in **pixels**
  * Inclusion helps browser render and load pages faster. Also, try to maintain proportions e.g. 2:1.
* Images are **void elements:** contain only attributes and don't markup text (i.e. not placed btw start and end tags)
  * Terminate by adding / before the > of the start tag. 
* **Using images as hyperlinks:** Can create graphical web pages that link to other resources.
  * **How?** put an `<img>` between `<a href = "">` and `</a>`
  
## 2.8: Special Characters and Horizontal Rules
* **Character entity references:** Format = "&code", represents special characters. Code can be word abbreviations or numbers.
  * E.g. `&copy` makes a copyright symbol, `&trade` makes a trademark symbol.
* **Horizontal Rule:** indicated by `<hr>`, renders a horizontal line with extra space above and below it in most browsers. 
  * Should be considered a *legacy element* since CSS can be used to do this and add other formatting. 
* **Special characters** can also be  represented as **numeric character references**:decimal or hexadecimal 
  * E.g. ampersand = `&#38` in decimal and `&=x26` in hexadecimal.

## 2.9: Lists
* **Unordered List `<ul>`:** creates a list in which each item in the list begins with a bullet symbol (typically a disc)
  * Each entry is an `<li>` element.
* **Ordered List `<ol>`:** creates a list in which each item begins with a number.
* **Nested Lists:** Express hierarchy.

## 2.10: Tables
**`table` element:** organize data into rows and columns.
**`caption` element:** specifies a table's title.
**`summary` attribute:** accessibility feature for visually impaired individuals.
**`thead`:** contains header info such as the column names.
**`tbody`:** Primary table data
**`tfoot`:** Calculation results, footnotes. Written above or below the body code but always displays at the bottom of the page.
**`tr`:** Defines individual tables rows.
**`th`:** Defines a column header in the table head or table foot section. Most browsers **center** and **bold** the text in this element.
**`td`:** Contains table data.
**`rowspan` and `colspan`:** merges data cells. Its *values* specify the number of rows/columns occupied by the cell.
  * Can be placed inside any `td` or `th`element. 
  * `br` is rendered as a line break. It is a **void element** but is also considered *legacy*.

<table border = "1">
<caption><strong>Table of Fruits (1st column) and
Their Prices (2nd column)</strong></caption>
<thead>
<tr> <!-- <tr> inserts a table row -->
<th>Fruit</th> <!-- insert a heading cell -->
<th>Price</th>
</tr>
</thead>

<tfoot>
<tr>
<th>Total</th>
<th>$3.75</th>
</tr>
</tfoot>

<tbody>
<tr>
<td>Apple</td>
<td>$0.25</td>
</tr>
<tr>
46 <td>Orange</td>
47 <td>$0.50</td>
48 </tr>
49 <tr>
50 <td>Banana</td>
51 <td>$1.00</td>
52 </tr>
53 <tr>
54 <td>Pineapple</td>
55 <td>$2.00</td>
56 </tr>
</tbody>
</table>

## 2.11: Forms
* **Forms** collect data from users.
* **`method`:** specifies how the form’s data is sent to the web server. 
  * `post` sends form data in the body of the HTTP message, not as part of the URL.
  * `get` appends the form data directly to the end of the URL of the form-processing script; visible in browser’s Address field.
* **`action`:** specifies the form-processing script (on the web server) to which the form data will be sent.
* **`input` elements:**  specify data to be sent to the form-processing script that processes the form (aka `form handler`).
  * **`type` attribute:** determines input type
  * **Hidden inputs:** nonvisual components. Store any data that you specify such as e-mail addresses.
  * **`text input`:** inserts a text field into the form, which allows the user to input data.
  * **`label`:**  provides users with information about the input element’s purpose.
  * **`size`:**  specifies the number of characters visible in the text field.
  * **`maxlength`:** limits the number of characters input into a text field.
  * **`submit`:** When the submit button is pressed, the form’s data is sent to the location specified in the form’s action attribute.
    * **`value`:**  sets the text displayed on the button.
  * **`reset`:**  reset all form elements to their default values.
* **`textarea`:**  inserts a multiline text area into the form. 
  * **`rows` and `cols`:** specify number of rows and columns (i.e characters per line).
  * Can include default text using `value`.
* **`password`:** inserts a password box into a form. **Masks** information input with another character, usually asterisks.
* **`checkbox`:** Select an option. Checkboxes that have the same `name` but different `value` attributes belong to the same group.
  * If two `checkbox` elements have the same `value` then the web server scripts can't distinguish them.
* **`radio` buttons:** Only one radio button in a group can be selected at a time.
  * If you don't set the names of each radio button then all buttons can be checked at the same time: *logic error*.
* **`select`:** provides a drop-down list of items. `name` defines the list, and `option` elements are items in the list.
  
## 2.12: Internal Linking
`a` tag can be used  to link to another section of the same document by specifying the element’s `id` as the link’s `href`.
* E.g. `<a href = #bugs>Go to favourite bugs</a>`

## 2.13: Meta elements
* **`name`:** identifies the type of the `meta` element
* **`content`attribute:** 
  * `keywords meta` element: provides search engines with a list of words that describe a page, which are compared with words in search requests.
  * `description meta` element, provides a short description of a site in sentence form, used by search engines to catalog your site (this text is sometimes displayed as part of the search result).
* Must be placed in the `head` section of HTML5 doc, otherwise they won't be read by search engines.
