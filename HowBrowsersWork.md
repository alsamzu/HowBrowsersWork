# What is a browser?
A web browser is a software application whose main function is to present web recourse chosen, by requesting it from the server and displaying it in the browser window.The resource is usually an HTML document, but may also be a PDF, image, or some other type of content. The location of the resource is specified by the user using a URI (Uniform Resource Identifier).

### Examples of browsers include:
* Chrome
* Firefox
* Edge
* Safari

### The browsers have common user interface like the:

* Address bar for typing the URL
* Menu icon
* Home, refresh, forward and backward buttons

## The browser’s main components are:

1. **The user interface:** this includes the address bar, back/forward button, bookmarking menu, etc. Every part of the browser display except the window where you see the requested page.

2. **The browser engine:** marshals actions between the UI and the rendering engine.

3. **The rendering engine:** responsible for displaying requested content. For example if the requested content is HTML, the rendering engine parses HTML and CSS, and displays the parsed content on the screen.

4. **Networking:** for network calls such as HTTP requests, using different implementations for different platform behind a platform-independent interface.

5. **UI backend:** used for drawing basic widgets like combo boxes and windows. This backend exposes a generic interface that is not platform specific. Underneath it uses operating system user interface methods.

6. **JavaScript interpreter:** Used to parse and execute JavaScript code.

7. **Data storage:** This is a persistence layer. The browser may need to save all sorts of data locally, such as cookies. Browsers also support storage mechanisms such as localStorage, IndexedDB, WebSQL and FileSystem.

## Rendering Engine
A rendering engine is a software component that takes marked up content (such as HTML, XML, image files, etc.) and formatting information (such as CSS, XSL, etc.) and displays the formatted content on the screen.
Different browsers use different rendering engines: Internet Explorer uses Trident, Firefox uses Gecko, Safari uses WebKit. Chrome and Opera (from version 15) use Blink, a fork of WebKit.

### The main flow
The rendering engine will start getting the contents of the requested document from the networking layer. This will usually be done in 8kB chunks.
The rendering engine will start parsing the HTML document and convert elements to DOM nodes in a tree called the "content tree". The engine will parse the style data, both in external CSS files and in style elements. Styling information together with visual instructions in the HTML will be used to create another tree: **the render tree.**
A **DOM** is the object presentation of the HTML document and the interface of HTML elements to the outside world like JavaScript.
**Parsing*** a document means translating it to a structure the code can use. The result of parsing is usually a tree of nodes that represent the structure of the document. This is called a **parse tree** or a **syntax tree.**
Parsing can be separated into two sub processes: lexical analysis and syntax analysis.

**Lexical analysis:** The process of breaking the input into tokens. Tokens are the language vocabulary: the collection of valid building blocks.

**Syntax analysis:** The applying of the language syntax rules.

The render tree contains rectangles with visual attributes like color and dimensions. The rectangles are in the right order to be displayed on the screen.

After the construction of the render tree it goes through a "layout" process. This means giving each node the exact coordinates where it should appear on the screen. The next stage is painting–the render tree will be traversed and each node will be painted using the UI backend layer and hence we are able to view the requested output.

**How it actually works**
When we type in a URL or click on a link and hit the Go button.The web browser program sends a request to a web server program running on the remote computer, the server program, gathers the request from the web browser, tries to hunt for the web page and then formulates a response.




