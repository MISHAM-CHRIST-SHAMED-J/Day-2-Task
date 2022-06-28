Differences between Document and Window Objects

Document Object: The document object represent a web page that is loaded in the browser. By accessing the document object, we can access the element in the HTML page. With the help of document objects, we can add dynamic content to our web page. The document object can be accessed with a window.document or just document.

Syntax:
document.property_name;

Properties of document:

activeElement: It returns the currently active elements in the document.
body: It returns the contents of the body element.
anchors: It returns all <a> elements that have a name attribute.
cookie: It returns the cookie of the current document.
domain: It returns the domain name of the document server.
URL: It returns the complete URL of the document.
forms: It returns all the elements of the form.
title: It returns the title element of the document.
head: It returns the head element of the document.
links: It returns all <area> and <a> elements that have a href attribute.
images: It returns the collection of <img> elements in the document.
scripts: It returns all script elements present in the document.

Example: This example describes the implementation of the document.object. 

<!DOCTYPE html>
<html>
<body>
	
	<script>
		function myFunction() {
			var title = document.title;
			var domain = document.domain;
			var body = document.body;
			document.getElementById("demo").innerHTML =
			"the title of the document is : "
			+ title
			+ "<br>"
			+ "domain : "
			+ domain
			+ "<br>"
			+ "body : "
			+ body;
		}
	</script>
</body>

</html>
  
  
Window Object: The window object is the topmost object of the DOM hierarchy. It represents a browser window or frame that displays the contents of the webpage. Whenever a window appears on the screen to display the contents of the document, the window object is created. 

Syntax:
window.property_name;


Properties of the window:

console: It returns a reference to the console object which provides access to the browser’s debugging console.
controllers: It returns the XUL controller objects for the current Chrome window.
crypto: It returns the browser crypto object.
Document: It returns a reference to the document object of that window.
History: It provides information on the URLs visited in the current window.
Length: It represents the number of frames in the current window.
Location: It contains the URL of the current window.
innerHeight: It is used to get the height of the content area of the browser window.
innerWidth: It is used to get the width of the content area of the browser window.
Name: It contains the name of the referenced window.
Window: It returns the current window or frame.
Navigator: It returns a reference to the navigator object.
outerHeight: It will get the height of the outside of the browser window.
outerWidth: It will get the width of the outside of the browser window.
Status: It overrides the default status and places a message in the status bar.
Toolbar: It will result in the toolbar object, whose visibility can be toggled in the window.
Screen: It refers to the screen object

The methods of Window objects that are commonly used are listed in the below table:

alert(): It is used to display an alert box. It displays a specified message along with an OK button and is generally used to make sure that the information comes through the user.
blur(): It is used to remove focus from the current window.
prompt(): It is used to display a dialog with an optional message prompting the user to input some text
resizeBy(): It is used to resize a window by the specified amount.
resizeTo(): It is used to resize a window to the specified width and height.
scrollBy(): It is used to scroll the document by the given number of pixels.
scrollTo(): It is used to scroll to a particular set of coordinates in the document.
setInterval(): It repeats a given function at every given time interval.
setTimeout(): It executes a function, after waiting a specified number of milliseconds.
stop(): It is used to stop the window from loading resources in the current browsing context.

Example: This example describes the implementation of the window.object.
  
<!DOCTYPE html>
<html>
<body>
	<script>
		function show() {
			var h = window.innerHeight;
			var w = window.innerWidth;
			var l = window.location;
			var c = window.closed;
			document.getElementById("prop").innerHTML =
			"Frame's Height: "
			+ h + "<br>"
			+ "Frame's Width: "
			+ w + "<br>"
			+ "Window location:"
			+ l
			+ "<br>"
			+ "Window Closed: "
			+ c;
		}
	</script>
</body>

</html>

