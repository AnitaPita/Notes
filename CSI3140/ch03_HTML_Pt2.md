# Chapter 3: Introduction to HTML, Part 2

## 3.1: New HTML5 Form Input Types

## 3.1.1: Color

**`color`:** input type enables the user to enter a color. 
* Most browsers render input type as a textfield in which you can type a **hexadecimal code** or a **color name**.
  * Future:  when you click a color input, browsers will likely display a **color picker** (already being done in chrome)
  
**`autofocus`:** automatically gives the focus to the input element, allowing the user to begin typing in that
element immediately.
* is an optional attribute that can be used in only **one** input element on a form

**Validation:** new HTML5 input types are **self validating on the client side**. 
* Upon form submission, browser immediately checks the self-validating elements to ensure that the data entered is correct.
* Benefits: Eliminate extra JS, reduce amount of invalid data submitted, reduce Internet traffic.
* *Server should still validate all input.*
* **`formnovalidate`:** add it to `input` type `submit` to bypass validation.

**`date`:** user can enter a date in the form `yyyy-mm-dd`.
* **Firefox and IE** display a text field in which a user can enter a date such as `2012-01-27`.
* **Chrome and Safari** display a **spinner control** (text field with an up-down arrow on the right side) allowing the user to select a date by clicking the up or down arrow; *start date* = current date.
* **Opera** displays a calendar from which you can choose a date.
* In future, trend will be to display a calendar.

**`datetime`:** user can enter a date (y, m, d), time (hh, minute, second, fraction of a second) and the time zone set to UTC.
* **`datetime-local`:** user to enter the date and time in a single control (without time zone). 

**`email`:**  user to enter an e-mail address or a list of e-mail addresses separated by commas (if the multiple attribute is specified). 
* An input in improper email format will ask the user to enter an email address is rendered pointing to the input element. (HTML5 doesn't actually check if the address exist though).

**`placeholder:`** place temporary text in a text field. 
* Is generally light gray and provides an example of the text and/or text format the user should enter.
* When focus is placed in text field, the `placeholder` text disappears.
* Is only used in `text`, `search`, `url`, `tel`, `email`, and `password`.

**`required`:** forces the user to enter a value before submitting the form. Can be added to any `input` type.

**`month`:**  user can enter a year and month in the format `yyyymm`, such as `2012-01`.
* If the user enters the data in an improper format (e.g. "January 2012") and submits... callout stating that an invalid value was entered.

**`number`:** enter a numerical value.
* *mobile browsers* display a numeric keypad while *desktop browsers* may have a text field or a spinner control.
* **`min`:** sets the minimum valid number.
* **`max:`** sets the maximum valid number.
* **`step`:** determines the increment in which the numbers increase.
* **`value`:** sets the initial value displayed in the form.
* The spinner control includes only the valid numbers. 

**`range`:** You can set the minimum and maximum and specify a value. 
* appears as a slider control in Chrome, Safari and Opera.
* *is inherently self-validating* because you cannot move the slider outside of its bounds.

**`search`:**  provides a search field for entering a query.
* Functionally equivalent to a `text` input type. Also, displays an *X* when you start typing so you can quickly clear the field.

**`tel`:** enter a telephone number.
* Rendered as a text field, in all browsers, and HTML5 does *not* self-validate it (use a `pattern` attribute with a regular expression instead)

**`time`:**  user can enter an hour, minute, seconds and fraction of second.
*  time MUST have two digits representing the hour, followed by a colon (:) and two digits representing the minute (i.e. only hour and minute are required)

**`url`:**  rendered as a text field, and the proper format is http://www.deitel.com
* www.deitel.com or www.deitelcom will not validate. Again, HTML5 only checks format, not if website exists.

**`week`:**  select a year and week number in the format `yyyy-Wnn`, where nn is 01–53
* e.g. `2012-W01` = first week of 2012.

## 3.2: Input/Datalist Elements and Autocomplete Attribute

**`autocomplete`:** can be used on input types to automatically fill in the user’s information based on previous input—such as name, address or e-mail.
* Can be enabled for either an entire form or individual elements.
* Format: `autocomplete = "on"`
* ONLY works if you specify a `name` or `id` attribute for the `input` element.

**`datalist`:** provides input options for a text input element.
* Depending on browser, drop-down list may appear after *clicking* on the field or after *typing* in field. Also, if a letter is typed, may either show all results that *start* with the letter or *contain* the letter.

## 3.3: Page-Structure Elements

**`header`:** creates a header for this page that contains both text and graphics, and can be used *multiple* times on a page.

**`time`:**  enables you to identify adate, a time or both. 

**`nav`:** groups navigation links. 
* For example, you can put an ordered/unordered list in between `<nav>` tags with `<li>` elements inside.

**`figure`:** describes a figure (e.g image, chart or table) in the document so that it could be moved to the side of the page or to another page.
* **`figcaption`:** provides a caption for the image in the `figure` element.

**`article`:**  standalone content that could potentially be used or distributed elsewhere, such as a news article, forum post or blog entry.
* can be nested (e.g. comments can be an `article` element inside an `article`).

**`summary`:** displays a rightpointing arrow next to a summary or caption when the document is rendered in a browser. 
*  **`details`:** When `summary` is clicked, the arrow points downward and reveals the content in this element.

**`section`:** describes a section of a document, usually with a heading for each section. Can also be nested.

**`aside`:** describes content that’s related to the surrounding content (e.g. an article) but is somewhat separate from the flow of the text. (E.g. an aside in a news story might include some background history)

**`meter`:** renders a visual representation of a measure within a range. 
* Contains a `min`, a `max`, and a `value` attribute. E.g responders to a survey question.

**`footer`:** describes a footer— content that usually appears at the bottom of a page or section element
* E.g. copyright notice and contact information.

**`mark`:** highlights the text that’s enclosed in the element. 
* `<mark>Two chapters on Control Statements</mark>`

**`wbr`:** indicates the appropriate place to break a word when the text wraps to multiple lines (to prevent a word from breaking in an awkward place).
