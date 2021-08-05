# PyBrowser

Build a web browser using PyQt5

##Web browser 
is a software application for accessing information on the World Wide Web. When a user requests a web page from a particular website, the web browser retrieves the necessary content from a web server and then displays the page on the screen.

##PyQt5 
is cross-platform GUI toolkit, a set of python bindings for Qt v5. One can develop an interactive desktop application with so much ease because of the tools and simplicity provided by this library.

###GUI Implementation steps :
1. Create a main window
2. Create a QWebEngineView object and add it as the central widget to the main window
3. Add Status bar to the main window
4. Create a toolbar and add navigation button and the line edit to show the url, below is hot the toolbar will look like


###Back-End Implementation Steps :
1. Add update url action to QWebEngineView object when url is changed.
2. Inside the update url action change the url of url bar and change cursor position
3. Add another update title action to the QWebEngineView object when loading is finished
4. Inside the update title method update the title of the window as the page title
5. Add actions to the navigation buttons using the build-in functions of the QWebEngineView object for reload, back, stop and forward buttons
6. Add action to the home button and inside the action change the url to google.com
7. Add action to the line edit when return key is pressed
8. Inside the line edit action get the text and covert this text to the QUrl object and set the scheme if it is null and set this url to the QWebEngineView object
