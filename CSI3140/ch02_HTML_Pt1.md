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
**`table` element**

## 2.11: Forms

## 2.12: Internal Linking

## 2.13: Meta elements

## 2.14: Web Resources
