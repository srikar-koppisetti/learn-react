## Inception 

### Emmet VSCode
- It helps in creating abbreviations using shortcuts.
- No extension is required for vscode it comes default.
- We can use it to write HTML and CSS

### CDN - Content Delivery Network
- Geographically distributed group of servers which work together to provide fast delivery of Internet content.
- A CDN allows for the quick transfer of assets needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

### Crossorigin
We add to crossorigin attribute to React and ReactDOM script tags because let's say our app in running on a certain domain we want to access CDN url which is on other domain. In order to overcome errors we add crossorigin attribute.

### Async VS Differ
*Async*
- Here when we are parsing HTML and we come across script tag, HTML parsing is stopped. Then immediately the scripts are downloaded and as soon as the script is downloaded it get's executed and once the script is executed then HTML parsing is continued.
- This might not help in good performance of the script as some of the functionality might be dependant on HTML which is not parsed. This will cause errors while rendering.

*Differ*
- In order to over come above issue, we can use deffer. In this when we are parsing the HTML and we come across script tag, it downloaded the script and in parallel it will not stop rendering HTML. Once the HTML rendering is done that is when script will be executed.
- This will not cause any issues while executing script as HTML is rendered and all DOM elements will be available.
