# Module 1: Get started with web development

## Web Hosting Types

### Shared hosting

- Cheapest option.
- Restricted to one physical server.
- Pay for a web service server in a physical server, but this server is shared with more than just one website. The hardware, power processing, memory and bandwidth is also shared.

### Virtual Private Service (VPS)

Restricted to one physical server.
This physical server provides virtual servers with dedicated CPU, memory and bandwidth for each VPS Instance (each website).

### Dedicated hosting

A whole physical server and web service dedicated to your website only.

### Cloud hosting

Not restricted to a physical server.
Uses a combination of multiple physical and virtual servers. In case a physical one fails, the data is sent to a virtual one so it always stays online.

## What is a Web Server? (NGINX)

- A web server stores and delivers the content for a website to clients (such as a web browser) that request it.
- Uses HTTP Protocol to communicate with the browser.
- Web acceleration: When a webserver caches content to speed delivery of a commonly requested content.
- Virtual Hosting: A Web server can host a single or multiple websites using the same software and hardware resources.

## What is a Web Browser? (Mozilla)

- A Web Browser retrieves information from other parts of the web and displays it on your machine. 
- Uses a piece of software called a rendering engine to translate the data that it receives into text, images and other visual content for the user.
- Cookies: Information about your usage of the website stored on your machine for the next time you visit that site. When you visit it again, it reads the cookies so it knows it's you. 
  With this, a site can use this file to target ads to you based in your usage.
  - Third-party cookies: Come from sites you're not visting at the time but can track you from site to site to gather information about you.
- Extensions can add new features and functionalities to a web browser.

## Who invented the Internet? And why? (Kurzgesagt) 

It wasn't a single person or team. The internet was built through combining projects and ideas of scientists from all over the world. TCP/IP (ARPANET, IETF), Packet Switching (NPL), the machine to machine direct connection without a gateway from France (CYCLADES), etc. TimBL was one of the founders of the World Wide Web (CERN); a service built on top of the internet for communication and data exchange using Web Browsers, HTTPS, HTML, etc. 

## What is Cloud Computing? (Amazon)

Cloud Computing is the on-demand delivery of IT resources via the internet. Instead of having to buy and manage a whole data center and servers, you can pay to access those resources as needed. The cloud is used for many functionalities, such as data backup, disaster recovery, email, virtual desktops, etc.
Since you don't have to worry about maganaging the servers, protocols, deploying globally, scaling, etc you can focus on what your business really needs to focus on.

## Browser Engines

Browser Engines are softwares destined translate the content of documents (code, such as HTML) into a visual, displayable and interactive visual representantion. Browser Engines create and implement structures so the different technologies of documents can interact with each other (DOM, etc).

## Search Engines

Search engines search the web for websites and webpages that contain information related to your search and display them to you as a list of links.


## Introduction to Internet Protocols

### IP versions

- IP Protocol Version 4 (Ipv4): The IP address contains four octets separed by dots. Example: 192.0.2.235

- IP Protocol Version 6 (Ipv6): The IP address contains eight groups of hexadecimal digits separated by colons. Example: 4527:0a00:1567:0200:ff00:0042:8329

### IP Packets

- Data sent through the internet are called IP Packets or Datagrams.

- Each IP Packet contains an IP Header and the payload (the data; IP Data).
  - IP Header: Destination IP address and Source IP Address.
  - Payload (IP Data): Data of the packet and some other protocols (TCP and UDP).

- TCP solves the problems of corrupt or lost packets and ensures it gets to the right destination and in order, but at the cost of a small delay when sending the data. Used to send data that must arrive correctly and in order such as text, images, etc.

- UDP solves the corrupt packet issue but packets can arrive out of order or not arrive at all. Used to send data that can tolerate some data loss but no delay such as voice calls, live video streaming, etc.

### HTTP

#### HTTP Request
Consists of a method, path, version and headers with additional information. Some contain a body (when using POST and PUT to transmit data).

GET /example.com/images/image.jpg HTTP/1.1
Host: developer.mozilla.org
Accept-language: en

Most commonly used methods:
- GET - Retrieve a resource.
- POST - Send data to a resource.
- PUT - Update a resource.
- DELETE - Removes a resource.
- PATCH - Partially updates a resource.

#### HTTP Response

Consists of headers, version, status code and status message, and a message body which corresponds to the content given.

HTTP/1.1 200 OK
Date: Sat, 09 Oct 2010 14:28:02 GMT
Server: Apache
Last-Modified: Tue, 01 Dec 2009 20:18:22 GMT
ETag: "51142bc1-7449-479b075b2891b"
Accept-Ranges: bytes
Content-Length: 29769
Content-Type: text/html

**Status Codes** - Grouped by the first digit of the error:

- Informational: 100-199
- Successful: 200-299
- Redirection: 300-399
- Client error: 400-499
- Server error: 500-599

### HTTPS

- Secure version of HTTP: it encrypts the information so nobody else can see the information being sent or received.
- Before the content is sent to the client, it is encrypted with a secret code, only the other computer can turn the secret code back into the original content.


### Dynamic Host Configuration Protocol (DHCP)

- Used to assign a computer to an IP address.
- The computer communicates over the network with a type of server called a DHCP server. It keeps track of computers and their IP addresses.

### Domain Name System (DNS)

- Assigns a domain name to an IP address.

### Internet Message Access Protocol (IMAP)

- It's purpose is to receive, download emails and manage the mailbox on the server.

### Simple Mail Transfer Protocol (SMTP)

- Used to send emails
- Allows email clients to submit emails for sending via an SMTP server
- Can also be used to receive emails from an email client, but IMAP is more commonly used

### Post-Office Protocol (POP)

- Older protocol to download emails to an email client.
- Differently from IMAP, the POP deletes the email on the server once it has been downloaded to your local device.
- More straightforward than IMAP.

### File Transfer Protocol (FTP)

- Used to transfer files from a local computer to a server.
- The data is transfered insecurely (different from SFTP)
- Requires an FTP Server and an FTP Client.

### Secure Shell Protocol (SSH)

- Allows the user to interact with with a server remotely.
- Requires an SSH server and an SSH Client.
- All data sent over SSH is encrypted. Only the sending and receiving computers can understand the data.

### SSH (Secure) File Transfer Protocol (SFTP)

- Used to transfer files from a local computer to a server, but over the SSH protocol.
- Differently from the FTP, the SFTP sends the data encrypted.

## Webpages, Websites and Web Apps

- Webpage is a single page.
- Website is a group of webpages linked together in the same domain name.
- Web Apps or Web Applications, in comparison to a website, provides higher level of interactivity, personalized and dynamic content. The content shown depends on the user's inputs.   

## Developer Tools

Elements tab - Inspect HTML elements and properties
Console - Check JavaScript logs and errors.
Sources tab - Shows all content resolved for the current page
Network tab - Inspect the timeline and details of HTTPs requests and responses for a webpage
Memory tab - Display the parts of the code that are consuming the most resources
Performance tab - How the web browser is performing displaying the web page; Pinpoint the functions that are taking the most time to run.

## Libraries and Frameworks

### Library 
- Re-usable pieces of code, provides specific functionality.
- Easier to replace than a framework.
- Needs to select library set compability.
- Unopinionated

### Framework 

- Provides a structure for a web developer to build with, which has rules.
- Encourages or even "forces" to use best practices.
- Harder to replace than a library.
- Opinionated

## Application Programming Interface (API) and Services

- A service, application or interface offering advenced functionality with simple syntax.
- A set of functions that an application component or service can provide.

### Web API / Browser API

- Extends the functionality of a website or browser.
- APIs are also known as gateways or middleware because they act as a bridge between systems.

### RESTful API

- REST is a set of principles used to build highly efficient APIs.
- Send and receive data to and from a centralized database.
- Provides responses to requests.

### Sensor-Based API

- The API that Internet of Things (IoT) is based on.
- Physical sensors can communicate with each other through the API.

### APIs Web Servers

- Design the data backbone of a web client. 
- Must be able to get data = GET
- Must be able to create data = POST
- Must be able to update date = PUT
- Must be able to delete data = DELETE

### API endpoint

- Specifies how different resources can be accessed.

### IDE (Integrated Development Environment)

- Software for building applications.
- Syntax highlighting.
- IntelliSense (suggestions for autocompletion).
- Refactoring.
- Addional functionality with plugins and extensions.

# Module 2: Introduction to HTML and CSS

## Document Object Model (DOM)

- Programming API for HTML and XML documents.
- Defines the logical structure of documents and the way a document is accessed and manipulated.
- Tree structure: nodes, parents and children.
- Each node and element is an object.

## Accessible Rich Internet Application (ARIA)

Web accessiblity semantics.


# Module 3: UI Frameworks

## Dependecy Tree
- A group of dependecies needed to run a project.

## Package Manager

- Automatically downloads and installs dependecies/packages.
- Takes care of the dependecy tree.
- You can publish your own packets.
- Most common web development package manager: Node Package Manager (NPM).

## Bundling tool

- Combine all web resources, dependecies/packages into a bundle that can be referenced later in the HTML.
- Common bundling tools: Gulp, Webpack

## Responsive Design

### Flexible grids

- Made of:
  - Columns
  - Gutters - space between the columns
  - Margins - space between the content and the left and right side of the screen
- Not pixel based
- Flexbility
- Percentages

### Fluid images

- Percentages
- Flexible width and height depending on the column

### Media queries

Can query the:
- Display size
- Orientation
- Aspect ratio

## Responsive Grid

### Breakpoint

- The pixel value specified.
- The point in which a website content and layout will adapt to provide the best UX.
- Can function in different ways across 3 different grids: Fixed Grid, Fluid grid, Hybrid grid.

### Fixed Grid

- Fixed width columns
- Fixed content width
- Flexible margins
- Change in the breakpoint: Flexible margins occupy the remaining space on the screen

### Fluid/Full Width Grid

- Fluid width columns
- Flexible content width
- Fixed gutters
- Change in the breakpoint: Columns either grow or shrink to adapt to available space

### Hybrid Grids

- Both fluid and fixed width components
- Frameworks provide CSS rules based on different device sizes

## Bootstrap

### Breakpoints and Infixes

| Breakpoint        | Class infix | Dimensions |
|-------------------|-------------|------------|
| Extra small       |             | < 576px    |
| Small             |     sm      | >= 576px   |
| Medium            |     md      | >= 768px   |
| Large             |     lg      | >= 992px   |
| Extra large       |     xl      | >= 1200px  |
| Extra extra large |     xxl     | >= 1400px  |

### Modifiers

Change the visual style of components

## Bootstrap's Grid System

Structure:
 - Containers
 - Rows
 - Columns

## Bootstrap Components

Pre-made sets of UI elements and styles.

## Introduction to React

## Static and Dynamic Content

### Static Content

Files and content that the server transfers just as it is stored on the web server; videos, images, etc.

### Dynamic Content

- Generated when the HTTP Request is made
- Can be:
  - Based on an input of a user
  - Based on the current date

1. Web browser action --> Web server --> Application server (or backend) --> generates dynamic content
2. Web rowser <-- Web server <-- Application server sends back the dynamic content generated

## Application Server

- Runs application logic
- Communicates with database
- Checks permissions

## Caching

Web server saves a copy of dynamic content readily availabe upon request.

## Single Page Application (SPA)

### Bundling

Server atends and loads all necessary HTML, CSS and JS immediately.

### Lazy Loading

Server sends only the HTML, CSS and JS needed to load the application, additional resources are downloaded as required.

## What is React

- Open source library availabe since 2013
- For single page applications
- For mobile applications: React Native

## React component

A small piece of a user interface.

## Virtual DOM

### Reconciliation

- React builds a representation of the Browser DOM in memory.
- React checks if the components in the Virtual DOM match with the Browser DOM. If a change is required, only the changed component is changed in the Browser DOM.

### Reconciliation Process

1. The Virtual DOM is updated
2. Diffs the updated version of the virtual DOM with the previous version and check which elements have changed.
3. Changed elements are updated in the Browser DOM.
4. Webpage updates to match the Browser DOM.

### React Fiber Architecture

- React incrementally renders the webpage: instead of updating the Browser DOM with all the Virtual DOM changes, React can spread the updates over time.
- It's a priority system. The highest priority changes - the elements visible to the user at the moment - are updated first.

## Component Hierarchy
- Tree structure
- There's always a Root or App Component
