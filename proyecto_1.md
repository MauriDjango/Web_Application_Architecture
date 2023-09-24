# Exploring the Fundamentals of Web Development in Client-Side Environments

## Web Application Architecture

Web Application Architecture refers to the overall structure of the software components that make up a web application i.e. 
applications, databases, and middleware (helps control the communication between components). The different architectures 
control how the information is passed between the different components and layers of an application, user access, and
data verification. The architecture chosen is a crucial decision as it will influence the scalability, reliability, security,
maintenance, and expandability of an application.

![Picture did not load](/img/architecture_model.jpg)

### Types of Web App Architectures

#### - Legacy Web Applications
Coming from and older generation of webpages and becoming slowly more and more outdated we will find
Legacy Web Apps. In the structure of these apps the entirety of the web page construction logic is stored in the server 
and every time the client wishes to interact with the page they send out a complete HTML page to a server. The server in
turn receives this request and sends back the entire updated HTML. This forces the client tot have to reload the entire
page each time for each update that is made. 

Some examples would be some government websites, educational platforms, and blogging platforms

![Picture did not load](/img/legacy_app.png)

Image credit to https://www.scnsoft.com/blog/web-application-architecture#key-terms

#### - Single Page Applications 
One of the most popular architectures in use today would be Single Page Apps. As opposed to Legacy Web Apps, the entire 
page is only downloaded once whilst a layer a JavaScript communicate with the web services and makes real-time updates 
to the page. This reduces the amount of data needing to be transferred to a minimum.
Due to its structure its offers a high degree of agility, responsiveness, and is lightweight, lending itself well to 
being converted into mobile applications. The goal of this architecture is to offer and smooth and seamless user experience.


Airbnb, twitter, and GitHub all use single page architecture.

![Picture did not load](/img/spa_app.png)

Image credit to https://www.scnsoft.com/blog/web-application-architecture#key-terms

#### - Widget Web Applications
Similar to Single Page Apps that save the hassle of having to reload the entire page each time an update is made we can 
also see Widget Web Applications. Here each page or service is separated into widgets or components. Using AJAX (Asynchronous JavaScript and XML)
these same widgets are able to receive and update their data without having to reload the entire page. 
Since the services are seperated into separate components they offer a high degree of modularity and usability. The
widgets can be added deleted or modified depending on the need and usage of the application without affecting other components
in its ecosystem. 

DuckDuckGO, some weather websites, and my yahoo are examples of some websites that use this architecture.

![Picture did not load](/img/widget_app.png)

Image credit to https://www.scnsoft.com/blog/web-application-architecture#key-terms


#### - Serverless Architecture
Often referred to as Serverless Computing or FaaS (Function as a Service) Serverless Architecture is cloud computing. Providers
of the cloud structure handle the infrastructure, servers, and server related tasks, allowing developers to focus solely
on the application coding and development.

Nordstrom, Yelp, and Slack aare all web application known to use this service.

#### - Microservices
While Widget Web Apps focus on the user interface Microservices are more inclined towards backend services and capabilities.
The idea is to separate each service independently, able to be deployed anywhere and even being able to run on distinct languages
and distinct databases.

LinkedIn, Spotify, and Amazon among many other known web applications employ this architecture.

#### - Progressive Web Applications
Progressive web applications have the primary goal of providing a user experience similar to that of a platform specific
app ,being usable on any browser and having a responsive web design.
In regard to its use on any browser it uses the concept of Progressive Enhancement whereby the application can adapt it
functionality based on the capabilities of the browser.

Pinterest, Uber, and AliExpress use this architecture.

## Browser Code Execution Mechanisms

### How is code executed in a browser?
A browser is the primary tool of a user to access and display web pages. Browser have the ability to execute JavaScript
thanks to their JavaScript engine. After the DOM model is created and the CCSOM has been applied the engine can begin to
execute JS code based on its location. The code can be executed depending on certain conditions or triggers:

![Picture did not load](/img/browser_execution.webp)

Image thanks to https://medium.com/tech-desk/browsers-and-their-working-mechanisms-33a6a6e3a681

#### - Triggers
- **During page load** - In the <head> tag where it is executed before the page is rendered or in the <body> tag where it is executed as the page
is being loaded. This is pre-external resources
- **Events**
    - **DOMContentLoaded**, fired when the DOM (Document Object Model) is fully parsed and ready to be manipulated
    - **Window Load**, fired when all page resources, including images and external scripts, have finished loading.
    - **User Interactions**, event handlers can be added to HTML elements to respond to user actions such as clicking buttons, hovering,
or submitting forms.
- **Timers and Intervals** - JS can be set to execute at a certain time or after a certain period.
- **Asynchronous Operations** - Tasks that can be executed independently of the main program flow, such as HTTP requests or handling data received from
external sources allowing the UX (User Experience) to remain smooth and not block the main program execution.

> JavaScript is the most common and widely used scripting language for client-side development
and is the default language for web browsers, however it is not the only one.

### Are all browsers compatible with the same web application?
All major browsers strive to be compliant with standards set by both the W3C (World Wide Web Consortium) and the WHATWG
(Web Hypertext Application Technology). This helps ensure that they maintain a high level of compatibility and can support 
the latest features of HTML, CSS, and JavaScript. However, there are still differences between the browsers that could 
lead to compatability issues. 

![Picture did not load](/img/web_compatability.png)

Image thanks to http://davincisdk.blogspot.com/2013/11/html5-browser-support.html

#### - Possible compatability issues
- **JS APIs** - Browsers can differ on the level of support they have for certain APIs. If the application depends on these
APIs for functionality special care must be taken to ensure compatability.
- **Experimental CSS** - To incorporate some experimental css properties browsers may require different prefixes to 
- **Web Components** - Similar to JS APIs support web components can vary among different browsers and should be tested
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
| **Description** | The primary and most used. Adds dynamic and interactive behavior                                                                                                                                                                      | A superset of JavaScript that is statically  typed boating a rich ecosystem  extending JS pre-existing ecosystem                                                                    | Developed by google to be used  with the flutter framework to develop  cross-platform and web applications distinguishing itself by having  the option to be compiled ahead of time (AOT) or just in time (JIT)                                                                                 |
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

#### - Traditional Programming Languages
- Strict typing lends to having fewer runtime errors and a more reliable code
- Compiled code leads to faster execution
- Suited to building large complex applications
- Can be used to create system applications such as operating systems and drivers
- Optimal for database programming

## Client-Side Technologies and Associated Languages

### CSS
CSS is a styling language used to describe how HTML should appear on a web page. It has the capacity to control the color, font,
visual style, and layout of the elements. Having these aspects controlled by CSS instead of HTML helps separate what would
be the structure of the web page from the presentations, helping the code be more maintainable and easier to modify.

### HTML5
HTML is a markup language used to control the structure of a web page. Similar to the idea of CSS, which controls the styling 
separate from structure, HTML does the exact opposite, controlling the structure separately from the rest of the code 
ensuring maintainability and adaptability. The most recent version of HTML, HTML5 expanded on the capabilities of HTML4. 
Some new features included in HTML5 are native multimedia support, expanded elements, geolocation API, and local and 
session storage to name a few.

### JavaScript
JavaScript is a scripting language used to add functionality and interactivity to a web page. Running under the structure
provided by HTML, JS allows manipulation of the Document Object Model, handle and direct user interactions, and make asynchronous
requests to servers.

### JQuery
Is a lightweight JS library that simplifies manipulation of the DOM model, event handling, and AJAX interactions. It maintains
compatability across browsers, letting developers write quick adn concise code for common JS tasks.

### DOM
Document Object Model is an interface that is created by the browser engine once it receives the relevant information from
the server. It houses and represents the structure of an HTML or XML file as a tree facilitating the manipulation of it by
JavaScript. Having this also allows developers to control when and how the data is modified and presented aiding  in the 
development of interactive and dynamic web pages.

### AJAX
Asynchronous JavaScript and XML is a set of techniques that allows applications to make requests to servers independently 
of the main program. Making the requests in the background of the application allows data to be updated without the necessity
of refreshing the entire page. You can imagine how much this lends to maintaining fluid interaction and functioning of a web 
page, preserving and maintaining the user experience.

### Front-End Framework
Nowadays, very rarely will you hear a conversation about applications without also hearing frameworks. The reason being
that in reality frameworks are collections of reusable elements destined towards aiding the fast and efficient development
of applications. These frameworks contain UI components, libraries, tools, and layouts to heal streamline web development.
Some of the most popular currently being React, Vue, and Angular.

### Web Components
Web platform Application Programming Interface nad technologies like ES Modules (ECMAScript Modules) and component libraries
group together to form web components. With these web components developers and create custom HTML elements with their own
particular behavior adn styling. This helps promote component based architecture leading to more modular and maintainable 
web applications

### JavaScript Code Integration Example

```
<script src="/js/js.js"></script>
  <head>
	<meta enctype="utf-8">
	<title>Cuenta Atras</title>
	<script>

		// 
		function marchaAtras() {
			// Esta instrucci�n ejecuta c�digo condicional.
			// La parte del 'if' si se cumple la condici�n y 
			// la del 'else' si no se cumple.
			if(n>0) n = n-1;
				else n = 9;
			// Cambiamos parte de la p�gina usando DOM
			document.getElementById("cuenta").src = n + ".png";
		}
	</script>
  </head>
<body onload="cuentaAtras()">
	<div id="numeros">
		<img src="9.png" id="cuenta">
	</div>
</body>
```

Here we can see JS being inserted into our HTML both as an external file and an internal script.

## Programming Tools

Thankfully things have advanced and developers don't have to make entire applications through the command console alone. 
We now have more advanced and user-friendly tools.

#### IDE
Integrated Development Environments combine several capabilities such as text editing, debugging, building, testing, and
packaging all into one application. Visual Studio Code, WebStorm, and IntelliJ are all prime examples.

#### Version Control
This is essential. Version control allows developers to track and maintain changes made to an application. They can also
check out and modify certain versions of an application to be able te develop and make changes to later reincorporate, giving time
and space to est for compatability and any issues that could arise from the changes made. Any issues or errors found can 
always be rectified by returning to a previous stable version and from that point continuing forward whilst correcting errors.
Git would be an example, it is everywhere and it is all-seeing.

#### Browser Testing
Since there are difference in compatability among browsers browser testing is a crucial part of the development process. 
Features developed in the environment of a specific browser may work fine there but once it moves away from home to a different
browser unexpected behavior or irregularities could crop-up. To prevent this browser testing tools such as selenium aid 
in the testing of application functionality across a number of browsers.

#### Browser Development tools

These are built in features in a browser that help developers inspect, debug, and optimize web applications.
Features such as the debugger panel that allow developer to set breakpoints and step through code. Network panels that 
help keep track of requests made by a web page. As well as the elements panel that allows developers to inspedct and manipulate
the DOM structure in real time to keep track of changes and effects.

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

Author - Maurice Darner
