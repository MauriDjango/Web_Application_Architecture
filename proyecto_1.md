# Exploring the Fundamentals of Web Development in Client-Side Environments

## Web Application Architecture
-How does it work?
-What apps use this architecture?
-What does it provide?
-Review each architecture individually

Web Application Architecture refers to the overall structure of the software components that make up a web application i.e. 
applications, databases, and middleware (helps control the communication between components). The different architectures 
control how the information is passed between the different components and layers of an application, user access, and
data verification. The architecture chosen is a crucial decision as it will influence the scalability, reliability, security,
maintenance, and expandability of an application.

### Types of Web App Architectures

#### - Legacy Web Applications
Coming from and older generation of webpages and becoming slowly more and more outdated we will find
Legacy Web Apps. In the structure of these apps the entirety of the web page construction logic is stored in the server 
and every time the client wishes to interact with the page they send out a complete HTML page to a server. The server in
turn receives this request and sends back the entire updated HTML. This forces the client tot have to reload the entire
page each time for each update that is made.

#### - Single Page Applications 
One of the most popular architectures in use today would be Single Page Apps. As opposed to Legacy Web Apps, the entire 
page is only downloaded once whilst a layer a JavaScript communicate with the web services and makes real-time updates 
to the page. This reduces the amount of data needing to be transferred to a minimum.
Due to its structure its offers a high degree of agility, responsiveness, and is lightweight, lending itself well to 
being converted into mobile applications. The goal of this architecture is to offer and smooth and seamless user experience

#### - Widget Web Applications
Similar to Single Page Apps that save the hassle of having to reload the entire page each time an update is made we can 
also see Widget Web Applications. Here each page or service is separated into widgets or components. Using AJAX (Asynchronous JavaScript and XML)
these same widgets are able to receive and update their data without having to reload the entire page. 
Since the services are seperated into separate components they offer a high degree of modularity and usability. The
widgets can be added deleted or modified depending on the need and usage of the application without affecting other components
in its ecosystem.

#### - Serverless Architecture
Often referred to as Serverless Computing or FaaS (Function as a Service) Serverless Architecture is cloud computing. Providers
of the cloud structure handle the infrastructure, servers, and server related tasks, allowing developers to focus solely
on the application coding and development.

#### - Microservices
While Widget Web Apps focus on the user interface Microservices are more inclined towards backend services and capabilities.
The idea is to separate each service independently, able to be deployed anywhere and even being able to run on distinct languages
and distinct databases.

#### - Progressive Web Applications
Progressive web applications have the primary goal of providing a user experience similar to that of a platform specific
app ,being usable on any browser and having a responsive web design.
In regard to its use on any browser it uses the concept of Progressive Enhancement whereby the application can adapt it
functionality based on the capabilities of the browser.

## Browser Code Execution Mechanisms

### How is code executed in a browser?
A browser is the primary tool of a user to access and display web pages. Browser have the ability to execute JavaScript
thanks to their JavaScript engine. The code can be executed depending on certain conditions or triggers:

#### - Triggers
- **During page load** - In the <head> tag where it is executed before the page is rendered or in the <body> tag where it is executed as the page
is being loaded. This is pre-external resources
- **Events**
    - **DOMContentLoaded**, fired when the DOM (Document Object Model) is fully parsed and ready to be manipulated
    - **Window Load**, fired when all page resources, including images and external scripts, have finished loading.
    - **User Interactions**, event handlers can be added to HTML elements to respond to user actions such as clicking buttons, hovering,
or submitting forms.
- **Timers and Intervals** - JS can be set to execute at a certain time or after a certain period.
- **Asynchronous Operations** [ Tasks that can be executed independently of the main program flow, such as HTTP requests or handling data received from
external sources allowing the UX (User Experience) to remain smooth and not block the main program execution.

> JavaScript is the most common and widely used scripting language for client-side development
and is the default language for web browsers however not the only one.

### Are all browsers compatible with the same web application?
All major browsers strive to be compliant with standards set by both the W3C (World Wide Web Consortium) and the WHATWG
(Web Hypertext Application Technology). This helps ensure that they maintain a high level of compatibility and can support 
the latest features of HTML, CSS, and JavaScript. However, there are still differences between the browsers that could 
lead to compatability issues. 

#### - Possible compatability issues
- **JS APIs** - Browsers can differ on the level of support they have for certain APIs. If the application depends on these
APIs for functionality special care must be taken to ensure compatability.
- **Experimental CSS** - To incorporate some experimental css properties browsers may require different prefixes to 
- **Web Components** - Similar to JS API's support web components can vary among different browsers and should be tested
for compatability

### Ways to avoid compatability issues
Though compatability issues do exists and are nigh inevitable making sure proper testing takes place to judge compatability
and tracking of known issues is of high priority. There are also some practices and actions that can be followed to help 
insure browser compatability.

#### - Solutions
- Above all using standardized web technologies recommended by the W3C
- Using clean code and best coding practices
- Using cross browser testing
- Using feature detection libraries to ensure feature support before applying functionalities and offering alternatives

## Client-Side Programming Languages
One of the core components of any web application is the client-side programming. This code helps add interactivity and
functionality to a web application such as the dynamic loading and rendering of content, handling user interactions, 
and manipulating the DOM. There are many client-side languages besides JavaScript whilst many compile to JavaScript 
some compile to their own language.

| **Language**    | **JavaScript**                                                                                                                                                                                                                        | **TypeScript**                                                                                                                                                                      | **Dart**                                                                                                                                                                                                                                                                                        |
|-----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Description** | The primary and most used. Adds dynamic and interactive behavior                                                                                                                                                                      | A superset of JavaScript that is statically  typed boating a rich ecosystem  extending JS pre-exisitng ecosystem                                                                    | Developed by google to be used  with the flutter framework to develop  cross-platform and web applications disitnguishing itself by haaving  the option to be compiled ahead of time (AOT) or just in time (JIT)                                                                                |
| **Language**    | **WebAssembly**                                                                                                                                                                                                                       | **Elm**                                                                                                                                                                             | **Swift**                                                                                                                                                                                                                                                                                       |
| **Description** | Though not a language in itself it provides the ability to  program client-side in languages such as C/C++, Rust, and  AssemblyScript being compiled to low-level code that can be  executed directly in the browsers virtual machine | Compiled to JS Elm is a statically typed functional programming  language/front-end framework. Its focuses is on correct typing and  reliability helping prevent errors at runtime. | Made for the apply ecosystem, Swift is designed to be easy to have a  concise syntax and prevent type issues with it's strong type safety. Although originally being for iOS it can now be used for server-side programming and cross-platform programming thanks to open-source contributions. |

## Script Language Characteristics
On the client-side of things the language that you'll regularly find are scripting languages i.e. Javascript, Ruby, Python,
and perl (Depending on the need of the application). There are specific reason why scripting languages tend to be favourable
when it comes to front-end web development as compared to more traditional programming languages.

### Scripting languages vs traditional programming languages
Scripting languages typically tend to be interpreted rather than compiled. For the purposes of rapid development and being
able to make quick changes and being able to test them interpreted languages triumph over compiled languages. In the case of
interpreted you wouldn't have to first compile the entire application to test the changes.

#### - Scripting Languages
- Dynamic typing adds a degree of flexibility and adaptability to the application
- Interpreted languages can be run without the need to compile the code first
- Scripting languages lend themselves to repetitive tasks
- Performing one-off tasks
- Creating dynamic web pages
- 
#### - Traditional Programming Languages
- Strict typing lends to having fewer runtime errors and a more reliable code
- Compiled code leads to faster execution
- Suited to building large complex applications
- Can be used to create system applications such as operating systems and drivers
- Optimal for database programming

## Client-Side Technologies and Associated Languages

### CSS
### HTML5
### JavaScript
### JQuery
### DOM
### AJAX
### Front-End Framework
### Web Components
