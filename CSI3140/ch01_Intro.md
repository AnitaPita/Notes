# Lecture 1: Introduction to Computers and the Internet

## 1.1: Introduction
* The Internet and web programming technologies you’ll learn in this course are designed to be portable, 
allowing you to design web pages and applications that run across an enormous range of Internet-enabled devices.

* **Client-side:** programming technologies that are used to build
web pages and applications that are run on the client (i.e.,
in the web browser on the user’s device). 
* **Server-side:** programming technologies that are used to build
applications that respond to requests from client-side web
browsers, such as searching the Internet, checking your
bank-account balance, ordering a book from Amazon,
bidding on an eBay auction, or ordering concert tickets, etc. 

* **Moore's Law:** Every year or two, the capacities of computers have approximately doubled inexpensively.
  * Moore’s Law applies especially to the amount of memory that
computers have for programs, the amount of secondary
storage (such as disk storage) they have to hold programs and
data over longer periods of time, and their processor
speeds—the speeds at which computers execute their
programs. Similar growth has occurred in the communications field, in
which costs have plummeted as enormous demand for
communications bandwidth (i.e., information-carrying
capacity) has attracted intense competition. 

## 1.2: The Internet in Industry and Research
* **The Internet in Industry and Research:** Electronic health records, human genome project, AMBER Alert, World Community Grid, One Laptop Per Child (OLPC), Cloud Computing, GPS, Robots, Email/IM/Video Chat/FTP, iTunes/Apple Store, Internet TV, Game Dev.

## 1.3: HTML5, CSS3, JavaScript and jQuery
* **HTML5:** Hypertext Markup Language is a special type of
computer language called markup language designed to
specify the content and structure of web pages (also called
documents) in a portable manner. HTML5 is the emerging version of HTML.
  * HTML enables you to create content that will...
     * render appropriately across an extraordinary range of devices connected to the Internet 
     * (smartphones, tablet computers, notebook computers, desktop computers, special purpose devices such as large-screen displays at concert arenas and sports stadiums, etc.)
* **XML:** eXtensible Markup Language
* **XHTML:** "stricter version of HTML based on XML
  * Some of the server-side technologies we cover later in the book produce web pages as XHTML documents, by default, but the trend
is clearly to HTML5.
* **CSS:** Cascading Style Sheets. 
  * Although HTML5 provides some capabilities for controlling a document’s presentation, it’s better *not to mix presentation with content.*
  * used to specify the presentation, or styling, of elements on a web page (e.g., fonts, spacing, sizes, colors, positioning, etc).
  * was designed to style portable web pages *independently* of their content and structure. 
  * By separating page styling from page content and structure, you can easily change the look and feel of the pages on an entire website, or a portion of the website, simply by swapping out one style sheet for another. 
  * *Current version = CSS3*
  
* **Javascript:**  portable scripting language. Programs written in JavaScript can run in web browsers across a wide range of devices.
  * helps you build **dynamic web pages** (i.e., pages that can be modified “on the fly” in response to events, such as user input,
time changes and more) and computer applications. 
  * enables you to do the client-side programming of web applications. 
  * was originally created by **Netscape.**
  * **ECMA:** European Computer Manufacturers Association
    * Both Netscape and Microsoft have been instrumental in the standardization of JavaScript developed by ECMA International, known as ECMAScript. ECMAScript 5, the current version of the standard, corresponds to the version of JavaScript used in the textbook.
    
* **Web Browsers and Web-Browser Portability:** Ensuring a consistent look and feel on client-side browsers.
  * Currently, a standard does not exist to which software vendors must adhere when they create web browsers. 
  * Although browsers share a common set of features, each browser might render pages differently.
  * *Browsers availability:* many versions and on many different platforms (Microsoft Windows, Apple Macintosh, Linux, UNIX, etc). 
  * Vendors add *features to each new version* that sometimes result in cross-platform *incompatibility* issues.
  * **HTML5 Test Website:** scores each browser based on its support for the latest features of HTML5
  * **Browsers used to test textbook examples:** Chrome, Firefox, Safari, Opera, IE9, and some iOS/Android.

* **jQuery:** simplifies JavaScript programming by making it easier to manipulate a web page’s elements and to interact with servers in a portable manner across various web browsers. (is a JS *library*). 
  * provides a library of custom GUI controls (beyond the basic GUI controls provided by HTML5) that can be used to enhance the look and feel of web pages. 
    
* **Validating HTML5, CSS3, and JavaScript Code**
  * HTML5: validator.w3.org/, html5.validator.nu/
  * CSS3: jigsaw.w3.org/css-validator/
  * JavaScript: www.javascriptlint.com/, www.jslint.com/
  
## 1.4: Demos
* This section just talked about some kinds of projects you can make with web tech.

## 1.5: Evolution of the Internet and World Wide Web
* How was the Internet—a global network of computers— made possible? by the *convergence of computing and communications technologies. *
* **ARPA:** the Advanced Research Projects Agency, funded by the U.S. Department of Defense. 
  * In the late 1960s, ARPA rolled out blueprints for networking the main computer systems of about a dozen ARPA-funded universities and research institutions. They were to be connected with communications lines operating at a then-stunning 56 Kbps (i.e., 56,000 bits per
second)—this at a time when most people (of the few who could) were connecting over telephone lines to computers at a rate of 110 bits per second.
* **Bit:** short for “binary digit”. The smallest data item in a computer; it can assume the value 0 or 1.
* **ARPANET:** Developed by ARPA, eventually became today's Internet.
  * Rather than enabling researchers to share each other’s computers, it rapidly became clear that communicating quickly and easily via email was the key early benefit of the ARPANET. 

* **Packet Switching:** digital data is sent in small bundles called packets
  * packets contained address, error-control and sequencing information. 
  * address information allowed packets to be routed to their destinations.
  * sequencing information helped in reassembling the packets—which, because of complex routing mechanisms, could actually arrive out of order—into their original order for presentation to the recipient.
  * Packets from different senders were intermixed on the same lines to efficiently use the available bandwidth
  * The network was designed to operate without centralized control. 
  * If a portion of the network failed, the remaining working portions would still route packets from senders to receivers over alternative paths for reliability

* **TCP/IP:** The protocol (i.e., set of rules) for communicating over the ARPANET (TCP = *Transmission Control Protocol*)
  * TCP ensured that messages were properly routed from sender to receiver and that they arrived intact
  * As the Internet evolved, organizations worldwide were implementing their own networks for both intra-organization (i.e., within the organization) and inter-organization (i.e., between organizations) communications.
  * Challenge = to get these different networks to communicate. Solution? **IP** (Internet Protocol)
  * Each computer on Internet has a unique IP address
  * The current IP standard, namely Internet Protocol version 4 (IPv4), has been in use since 1984, and will soon run out of possible addresses.
  * IPv6 is just starting to be deployed. Features = enhanced security and a new addressing scheme, hugely expanding the number of
IP addresses available so that we will not run out of IP addresses in the foreseeable future

* **Explosive Growth:** Initially, Internet use was limited to universities and research institutions; then the military began using it intensively. Eventually, the government decided to allowcaccess to the Internet for commercial purposes
  * **Bandwidth** (i.e., the information-carrying capacity) on the Internet’s is increasing rapidly as costs dramatically decline

* **WWW:**  technology that allows computer users to execute web-based applications and to locate and view multimedia-based documents on almost any subject over the Internet
  * **1989:**  Tim Berners-Lee of CERN (the European Organization for Nuclear Research) began to develop a technology for sharing information via hyperlinked text documents. (**HTML**). He also wrote a communication protocol to form the backbone of his new
information system, which he called the World Wide Web.
  * **Hypertext Transfer Protocol (HTTP):** a communications protocol used to send information over the web.
  * **URL (Uniform Resource Locator):** specifies the address (i.e., location) of the web page displayed in the browser window.
* **HTTPS:** standard for transferring encrypted data on the web
  * URLs of websites that handle private information, such as credit card numbers, often begin with *https://*, the abbreviation for Hypertext Transfer Protocol Secure
  * combines HTTP with the Secure Sockets Layer (SSL) and the more recent Transport Layer Security (TLS) cryptographic schemes for
securing communications and identification information over the web.
  * A client browser that wishes to communicate securely with a server iniates (over TCP/IP) a **TLS Handshake** with the server. 
    * During the Handshake process, the server and client agree on parameters that will be used to encrypt messages sent between them. 
  
* **Mosaic:** browser which featured a user-friendly GUI; released in 1993
  * Marc Andreessen, whose team at the National Center for Supercomputing Applications (NCSA) developed Mosaic, went on to found **Netscape**, the company that many people credit with igniting the explosive Internet economy of the late 1990s.
* **dot com bust:** economic bust brought hard times in the early 2000s.
  * **Web 2.0:** The resurgence that began in 2004 or so.

## 1.6: Web Basics

* **Web Page:**  nothing more than an HTML document  that describes to a web browser the document’s content and structure. 
* **Hyperlinks:** Load a specific web document. Both images and text may be used as hyperlinks. 
  * When the user clicks a hyperlink, a web server locates the requested web page and sends it to the user’s web browser.
  * User can type the address of a web page into the browser’s address field, pressing Enter to view the specified page.
  * Can reference other web pgs, email addresses, files and more.
  * **mailto:emailAddress:** clicking the link loads your default e-mail program and opens a message window addressed to the specified e-mail address. 
  * If a hyperlink references a file that the browser is incapable of displaying, the browser prepares to **download** the file, and generally prompts the user for information about how the file should be stored.
  * **URI:** Uniform Resource Identifier. if it starts w/ "http://", it's a **URL** (Uniform resource locator). 
  * **Parts of a URL:** A URL contains information that directs a browser to the resource that the user wishes to access. Web servers make such resources available to web clients. Popular web servers include Apache’s *HTTP Server* and Microsoft’s *Internet Information Services (IIS)*.
   * The string **http://** indicates that the HyperText Transfer Protocol (HTTP) should be used to obtain the resource.
   * **fully qualified hostname:** (e.g: www.deitel.com) the name of the web server computer on which the resource resides. 
   * computer is referred to as the **host**, because it houses and maintains resources.
     *  hostname www.deitel.com is translated into an IP (Internet Protocol) address—a numerical value that uniquely identifies the server on the Internet. 
   *  **Internet Domain Name System (DNS) server:** maintains a database of hostnames and their corresponding IP addresses and performs the translations automatically.
   * Remainder of the URL specifies the **resource location** and **resource name** on the web server.
     * The location could represent an actual directory on the web server’s file system. For security reasons, however, the resource’s location is typically a **virtual directory.** The web server translates the virtual directory into a real location on the server, thus *hiding the resource’s true location.*
  
### Making a Request and Receiving a Response
* Web browser sends an HTTP request to the server. 
* The word **GET** is an HTTP method indicating that the client wishes to obtain a resource from the server. 
* The remainder of the request provides the *path name* of the resource (e.g., an HTML5 document) and the *protocol’s name and version number* (HTTP/1.1).
* The client’s request also contains some required and optional headers
* **Response:**  server first sends a line of text that indicates the HTTP version, followed by a numeric code and a phrase describing the status of the transaction (e.g.: HTTP/1.1 200 OK, HTTP/1.1 404 Not found).
* **HTTP Header:**  server sends one or more HTTP headers, which provide additional information about the data that will be sent.
  * In this case, the server is sending an HTML5 text document, so one HTTP header for this example would be: *Content-Type: text/html*
  * **Multipurpose Internet Mail Extensions (MIME):** type of the content that the server is transmitting to the browser. This is provided in this header. MIME is the standard or convention for specifying the content type of a message.
    * e.g. MIME type *text/plain* indicates that the sent information is text that can be displayed directly.
    * e.g.  MIME type *image/jpeg* indicates that the content is a JPEG image.
  * The header or set of headers is followed by a blank line, which indicates to the client browser that the server is finished sending HTTP headers. 
  * Finally, the server sends the contents of the requested document (e.g., the file *downloads.html*).
  * The client-side browser then *renders* (displays) the document, which may involve additional HTTP requests to obtain associated CSS and images.

### HTTP get and post request
* **get request:** typically gets (or retrieves) information from a server, such as an HTML document, an image or search results based on a user- submitted search term.
  * get request appends data to the URL
  * e.g. **search** is the name of Google’s server-side form handler, q is the name of a variable in the Google’s search form and deitel is the search term. 
  * The **?** in the preceding URL separates the **query string** from the rest of the URL in a request.
  * A **name/value pair** is passed to the server with the variable name and its value separated by an equals sign (=). 
  * If more than one name/value pair is submitted, each pair is separated by an **ampersand** (&).
* **post request:**  typically posts (or sends) data to a server. Common uses of post requests are to send form data to a server. 
  * An HTTP post request posts data to a server-side form handler that processes the data. 
  * A get request typically limits the query string (i.e., everything to the right of the ?) to a specific number of characters (e.g., a few thousand characters), so it’s often necessary to send large amounts of information using the post method.
  * also sometimes preferred because it hides the submitted data from the user by embedding it in an HTTP message. The form data still reaches the server and is processed in a similar fashion to a get request, but the user *does not see the exact information sent.*
  
### Client-side caching
* Browsers often **cache** (save on disk) recently viewed web pages for quick reloading. 
* If there are no changes between the version stored in the cacheand the current version on the web->speeds up your browsing experience.
* HTTP response can indicate (in one of its header fields) the length of *time* for which the content remains “fresh”.
  * If this amount of time has not been reached, the browser can avoid another request to the server and simply load the document from the cache. 
  * There’s also the “not modified” HTTP response, indicating that the file content has not changed since it was last requested. 

## 1.7: Multitier Application Architecture
Web-based applications are often multitier applications (sometimes referred to as n-tier applications) that divide functionality into
separate tiers (i.e., logical groupings of functionality). 
* **Bottom tier:**  (also called the data tier or the *information tier*) maintains the application’s data. It typically stores data in a relational database management system (RDBMS).
* **Middle tier:**  implements business logic, controller logic and presentation logic to control interactions between the application’s clients and its data.  acts as an intermediary between data in the information tier and the application’s clients. 
  * **Middle-tier controller logic:** processes client requests (such as requests to view a product catalog) and retrieves data from the database. 
  * **Middle tier presentation logic:**  processes data from the information tier and presents the content to the client.
  * **Middle tier Business logic:** enforces business rules and ensures that data is reliable before the application updates a database or presents data to users. Business rules dictate how clients access data and how applications process data.
* **Top tier:** (also called user interface tier or *client tier*) is the application’s UI, which gathers input and displays output.
  * Users interact directly with the application through the user interface, which is typically a web browser or a mobile device. 
  * In response to *user actions* (e.g., clicking a hyperlink), the top tier interacts with the middle tier to make requests and to retrieve data from the information tier. The top tier then displays the data retrieved for the user. 
  
## 1.8: Client-Side Scripting versus Server-Side Scripting
* **Client-side scripting:** JavaScript can be used to validate user input, to interact with the browser, to enhance web pages, and to add client/server communication between a browser and a web server.
  * Client-side scripting does have some limitations, such as **browser dependency**: the browser or **scripting host** must support the scripting language and capabilities.
  * Client-side scripts are restricted from arbitrarily accessing the local hardware and file system for security reasons. 
  * Client-side scripts can be viewed by the client by using the browser’s source-viewing capability, so sensitive information, such as passwords or other personally identifiable data, should not be on the client. 
  * All client-side data validation should be mirrored on the server. Also, placing certain operations in JavaScript on the client can open web applications to security issues.
* **Server-side scripting:**  generate custom responses for clients.
  * e.g a server queries the database, dynamically generates an HTML document containing the flight list, and sends the document to the client. This allows clients to obtain the most current flight information from the database by connecting to an airline’s web server.
  * have a wider range of **programmatic capabilities** than their client-side equivalents. 
  *  have access to server-side software that extends server functionalities
     * Microsoft web servers use ISAPI (Internet Server Application Program Interface) extensions.
     * Apache HTTP Servers use modules. 

## 1.9: World Wide Web Consortium (W3C)
* October 1994: Tim Berners-Lee founded the organization, devoted to developing nonproprietary, interoperable technologies for the World Wide Web.
* Primary goal is to make the web universally accessible, regardless of disability, language or culture. 
* Is also a *standards organization*.
* **Recommendations:** Web technologies standardized by the W3C
* Current and forthcoming W3C Recommendations include HTML5, CSS3, and XML.

## 1.10: Web 2.0, Going Social
* 2003: noticeable shift in how people and businesses were using the web and developing web-based applications. 
* Web 2.0 was coined by Dale Dougherty of O’Reilly Media in 2003 to describe this trend.
* Generally, Web 2.0 companies use the web as a platform to create collaborative, community-based web sites (e.g., social networking sites, blogs, wikis).
* **Web 1.0** (the state of the web through the 1990s and early 2000s) was focused on a relatively small number of companies and advertisers producing content for users to access
  * Also called the "Brochure Web".
  * Analogy: One way to look at Web 1.0 is as a lecture, a small number of professors informing a large audience of students.
* **Web 2.0** involves the users
  * they create content and help organize it, share it, remix it, critique it, update it, etc.
  * Analogy: a conversation, with everyone having the opportunity to speak and share views.
* **Architecture of Participation:**  design that encourages user interaction and community contributions.
  * **collective intelligence:** the concept that a large diverse group of people will create smart ideas
  * **Rich Internet Applications (RIAs):**  being developed using technologies (such as Ajax) that have the look and feel of desktop software, hence enhancing a user’s overall experience
  
* **Search Engines and Social Media:** The way we find the information on these sites is also changing—people are tagging (i.e., labeling) web content by subject or keyword in a way that helps anyone locate information more effectively.
* **Semantic Web:** In the future, computers will learn to understand the meaning of the data on the web.
* **Google:** returns extremely accurate search results. It has become the most widely used search engine and one of the most popular websites in the world.
  * In 1996, Stanford computer science Ph.D. candidates Larry Page and Sergey Brin began collaborating on a new search engine.
  * In 1997, they chose the name Google—a play on the mathematical term googol, which is a number that is equal to 1 followed by 100
  zeros (or 10100), a staggeringly large number.

* Web services, inexpensive computers, abundant highspeed Internet access, open source software and many other elements have inspired new, exciting, **lightweight business models** that people can launch with only a small investment.
* Some types of websites with rich and robust functionality that might have required millions of dollars to build in the 1990s can now be built for nominal sums.

* **Ajax:** A premier Web 2.0 software. Ajax helps Internet-based applications perform like desktop applications.
  *  such applications suffer transmission delays as data is shuttled back and forth between your computer and servers on the Internet, so Ajax is super useful.

## 1.11: Data Hierarchy
Data items processed by computers form a data hierarchy that becomes larger and more complex in structure as we progress from bits to characters to fields.
* **Bits:** The smallest data item in a computer can assume the value 0 or the value 1.
* **Characters:**  Digits, letters and special symbols. 
* **Fields:** composed of characters or bytes
* **Records:** Several related fields (e.g. a payroll system)
* **Files:** groups of related records
* **Database:**  electronic collection of data that’s organized for easy access and manipulation.

## 1.12: Operating Systems
* **OS:** software systems that make using computers more convenient for users, application developers and system administrators. 
  *  provide services that allow each application to execute safely, efficiently and concurrently (i.e., in parallel) with other applications.
* **Kernel:** software that contains the core components of the operating system
* **Popular desktop OSs:** Linux (open-source), Windows (proprietary), and Mac OS
* **Popular mobile OSs:** Android, iOS, BlackBerry OS, Windows Phone.

## 1.13: Types of Programming Languages
* **Machine Language:** Defined by its hardware design. Generally consist of numbers (ultimately reduced to 1s and 0s).
* **Assembly Language:** English language abbreviations to represent elementary operations.
* **Assemblers:** Translator programs that convert assembly language to machine language.
* **High-level languages:**  single statements could be written to accomplish substantial tasks.
* **Compilers:** convert high-level language programs into machine language
* **Interpreter Programs:**  execute high-level language programs directly, although more slowly than compiled programs

## 1.14: Object Technology
* **Objects:** essentially reusable software components. 
  * Almost any noun can be reasonably represented as a software object in terms of:
    * **Attributes** (e.g., name, color and size)
    * **Behaviors** (e.g., calculating, moving and communicating). 
### TODO

## 1.15: Keeping up with IT
## TODO
