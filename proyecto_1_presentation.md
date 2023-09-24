---
theme: default
class: default-class
marp: true

---

<style>
@import url('css/presentation_style.css');
</style>

<!-- .slide -->

# Exploring the Fundamentals of Web Development in Client-Side Environments

In this presentation, we'll dive into the core concepts of web development in client-side environments, examining various aspects of web application architecture, client-side programming languages, and essential technologies.

---
 
## Web Application Architecture

Web Application Architecture serves as the foundation of any web application. It defines the overall structure of the software components that constitute a web app. These components include applications, databases, and middleware, which control communication between different parts of the application.

Web architecture plays a critical role in determining a web app's scalability, reliability, security, maintenance, and expandability. Let's explore various types of web app architectures:

---

### Types of Web App Architectures

#### Legacy Web Applications

Legacy Web Apps represent an older generation of webpages where the entire web page construction logic resides on the server. Whenever a client interacts with the page, it sends a complete HTML page to the server, which responds with the updated HTML. Unfortunately, this approach necessitates reloading the entire page for each update.

#### Single Page Applications

Single Page Apps are a modern architecture that optimizes user experience. These apps download the entire page once and then use JavaScript to communicate with web services, enabling real-time updates without reloading the page. This architecture enhances agility, responsiveness, and is particularly suitable for mobile applications.

---

### Types of Web App Architectures

#### Widget Web Applications

Widget Web Apps take the optimization a step further by breaking down each page or service into widgets or components. Using AJAX, these widgets can receive and update their data without requiring a full page reload. This approach promotes modularity and usability, as widgets can be added, deleted, or modified independently.

#### Serverless Architecture

Serverless Architecture, often known as Function as a Service (FaaS), is a cloud computing paradigm. Cloud providers manage the infrastructure, allowing developers to focus solely on application coding and development. This architecture is well-suited for building scalable and cost-effective applications.

---

### Types of Web App Architectures

#### Microservices

Microservices architecture focuses on backend services. Each service operates independently and can be deployed anywhere, even using different programming languages and databases. This flexibility is particularly advantageous for large-scale applications.

#### Progressive Web Applications

Progressive Web Applications (PWAs) aim to provide a user experience similar to platform-specific apps, accessible on any browser with responsive web design. PWAs employ Progressive Enhancement to adapt functionality based on the capabilities of the user's browser.

---

## Browser Code Execution Mechanisms

### How is code executed in a browser?

A browser's JavaScript engine is responsible for executing code. It does so based on specific conditions or triggers:

- During page load: Code can be executed in the <head> tag before rendering or in the <body> tag as the page loads.
- Events: Events like DOMContentLoaded, Window Load, and user interactions trigger code execution.
- Timers and Intervals: JavaScript can be scheduled to execute at certain times or intervals.
- Asynchronous Operations: Tasks like making HTTP requests or handling external data occur independently of the main program flow, ensuring a smooth user experience.

JavaScript is the primary client-side language, but other languages like TypeScript, Dart, WebAssembly, Elm, and Swift are also used for specific purposes.

---

### Are all browsers compatible with the same web application?

Major browsers strive to adhere to standards set by organizations like W3C and WHATWG. However, differences exist that can lead to compatibility issues. Common issues include variations in support for JavaScript APIs, experimental CSS properties, and Web Components.

To mitigate compatibility problems:

- Use standardized web technologies recommended by W3C.
- Write clean code and follow best practices.
- Perform cross-browser testing.
- Implement feature detection to ensure support for specific features and offer alternatives when necessary.

---

## Client-Side Programming Languages

Client-side programming enriches web applications with interactivity and functionality. While JavaScript is the predominant language, others serve specific needs:

- **JavaScript**: The primary and most widely used language, JavaScript adds dynamic and interactive behavior to web pages.

- **TypeScript**: A superset of JavaScript, TypeScript introduces static typing and extends the JavaScript ecosystem.

- **Dart**: Developed by Google, Dart is used with the Flutter framework for cross-platform and web applications. It offers both ahead-of-time (AOT) and just-in-time (JIT) compilation options.

---

## Client-Side Programming Languages

- **WebAssembly**: Although not a language itself, WebAssembly allows client-side programming in languages like C/C++, Rust, and AssemblyScript. Code is compiled to low-level code executed directly in the browser's virtual machine.

- **Elm**: Elm is a statically typed functional programming language and front-end framework that emphasizes correct typing and reliability.

- **Swift**: Originally designed for iOS, Swift is now used for server-side and cross-platform development due to its concise syntax and strong type safety.

---

## Script Language Characteristics

Scripting languages, such as JavaScript, offer distinct advantages for front-end web development:

- **Dynamic Typing**: Scripting languages like JavaScript offer flexibility with dynamic typing.
- **Interpreted Nature**: They are interpreted, allowing rapid development and testing without compilation.
- **Suited for Web Pages**: Scripting languages excel at creating dynamic web pages and handling repetitive tasks.

In contrast, traditional programming languages like C++ are compiled, leading to faster execution and suitability for large-scale applications and system programming.

---

## Client-Side Technologies and Associated Languages

### CSS

CSS (Cascading Style Sheets) controls the presentation and styling of HTML elements, ensuring separation of presentation from structure for maintainability and flexibility.

### HTML5

HTML5 builds upon HTML4 by introducing native multimedia support, expanded elements, a geolocation API, and local/session storage, enhancing web application capabilities.

### JavaScript

JavaScript adds functionality and interactivity to web pages, enabling manipulation of the Document Object Model (DOM), handling user interactions, and making asynchronous requests to servers.

---

## Client-Side Technologies and Associated Languages

### JQuery

JQuery is a lightweight JavaScript library that simplifies DOM manipulation, event handling, and AJAX interactions. It ensures compatibility across browsers.

### DOM

The Document Object Model (DOM) represents the structure of HTML/XML as a tree, facilitating manipulation by JavaScript. It grants developers control over data presentation and modification.

### AJAX

Asynchronous JavaScript and XML (AJAX) allows applications to make server requests independently, updating data without requiring full page refreshes, enhancing user experience.

---

## Client-Side Technologies and Associated Languages

### Front-End Frameworks

Front-end frameworks like React, Vue, and Angular provide reusable UI components and development tools for efficient web application development.

### Web Components

Web components leverage web platform APIs, ES Modules, and component libraries to create custom HTML elements with unique behavior and styling. They encourage modular and maintainable web applications.

---

## Programming Tools

Web development has advanced with the introduction of specialized tools:

### Integrated Development Environments (IDEs)

IDEs like Visual Studio Code, WebStorm, and IntelliJ combine text editing, debugging, testing, and packaging, streamlining the development process.

### Version Control

Version control systems like Git enable tracking and maintenance of code changes. Developers can collaborate, test, and revert changes as needed, ensuring code integrity.


---

## Programming Tools

### Browser Development Tools

These are integrated tools within web browsers designed to assist developers in inspecting, debugging, and optimizing web applications.

- **Debugger Panel:** Developers can set breakpoints and step through code for efficient debugging.

- **Network Panels:** Helps track requests made by a web page, aiding in performance optimization.

- **Elements Panel:** Allows real-time inspection and manipulation of the DOM structure to monitor changes and effects.

### Browser Testing

Browser testing tools such as Selenium assist in verifying application functionality across multiple browsers, addressing compatibility concerns.

---

## Bibliography

Web Application Architecture - https://contentsnare.com/web-application-architecture/
Web Application Architecture - https://kinsta.com/es/blog/arquitectura-aplicaciones-web/#tipos-de-arquitectura-de-aplicaciones-web
Web Application Architecture - https://www.scnsoft.com/blog/web-application-architecture#key-terms
Web Application Architecture - https://www.clickittech.com/devops/web-application-architecture/
Web Application Architecture - https://thinksys.com/development/web-application-architecture-complete-guide/
Browser Code Execution - https://medium.com/tech-desk/browsers-and-their-working-mechanisms-33a6a6e3a681
Browser Compatability - https://www.omniconvert.com/what-is/browser-compatibility/
Scripting Languages vs Traditional Languages - https://www.unosquare.com/blog/scripting-and-programming-languages-differences-advantages-and-optimal-use-cases/
Client-Side Web Technologies - https://learn.microsoft.com/en-us/dotnet/architecture/modern-web-apps-azure/common-client-side-web-technologies
Client-Side Web Technologies - https://docs.oracle.com/cd/E13218_01/wlp/docs102/clientdev/ria.html


