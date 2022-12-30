## Inception 

### Emmet VSCode
- It helps in creating abbreviations using shortcuts.
- No extension is required for vscode it comes default.
- We can use it to write HTML and CSS

### Difference between library and framework
*Library*
- Performs well defined, specific operations
- Ex: image manipulation, string utilities, regular expression evaluation, math. 

*Framework*
- Its a skeleton. It defines the meat of the application.
- There is work to fill the skeleton but the most of the boilerplate work is done by the the framework.
- The framework defines the concept but the application defines the fundamental functionality that end-users care about.
- Ex: Angular, Spring. 

### CDN - Content Delivery Network
- Geographically distributed group of servers which work together to provide fast delivery of Internet content.
- A CDN allows for the quick transfer of assets needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

### Crossorigin
We add to crossorigin attribute to React and ReactDOM script tags because let's say our app in running on a certain domain we want to access CDN url which is on other domain. In order to overcome errors we add crossorigin attribute.

### Difference between React and ReactDOM
- React library was created to build applications across all the platforms. Web, mobile, desktop etc. So, in order to support different platforms react came up with a core library for all platforms and a platform specific library. So for web, in order to build applications using React library we need *React* the core library and *ReactDOM* which is a web library.

### Difference between react.development.js and react.production.js files via CDN?
In building an application we have two phases 1. Development phase and 2. Release to users for consumption. If we are building web applications using React library. 

Here in the first phase which is development we need more understanding of the library methods and more help with debugging the code when developer comes across any issues. In that case using a developer friendly version of the library is helpful which is *react.development.js*. This helps in reading the methods, understanding and debugging. It's very readable code. The code size is huge.

In the second phase where we are deploying code to production or for the users to use. We have crossed the phase of development we no longer need the detailed code, hence we use a minified version which has same functionality. Here the code size is small and it's not readable. This helps in the fast download of the application and rendering. In a way increases user experience.

### Async VS Differ
*Async*
- Here when we are parsing HTML and we come across script tag, HTML parsing is stopped. Then immediately the scripts are downloaded and as soon as the script is downloaded it get's executed and once the script is executed then HTML parsing is continued.
- This might not help in good performance of the script as some of the functionality might be dependant on HTML which is not parsed. This will cause errors while rendering.

*Differ*
- In order to over come above issue, we can use deffer. In this when we are parsing the HTML and we come across script tag, it downloaded the script and in parallel it will not stop rendering HTML. Once the HTML rendering is done that is when script will be executed.
- This will not cause any issues while executing script as HTML is rendered and all DOM elements will be available.
