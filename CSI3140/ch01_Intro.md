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
  
