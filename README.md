# Webmaster Content Notes
## Session 1 on Feb 13

#### Internet & Web
- Internet is a big Collection of Computers and Cables 
- Web is a big collection of HTML Pages on the Internet

#### Computer Network
- A network is a structure linking computers together for the purpose of sharing information and services.
- The best-known computer network is the Internet.

#### Client & Server
- Users typically access a network through a computer called a node or host
- A host that provides information or a service is called a **server**
- A computer or other device that receives a service is called a **client**
- One of the most commonly used designs is the client-server network

#### LAN vs WAN
- LAN is Local Area Network 
- WAN is Wide Area Network

##### New Definitions of LAN & WAN:
- LAN is a network using LAN Connections
	- LAN connections can only operate in a local area which is usually not any bigger then a house, or a floor in an office building. (Limited to Small Area)
	- **Ethernet** and **Wi-Fi** are the two primary ways to enable LAN connections
- WAN is a network using WAN connections
	- WAN connections are available from house to house, city to city, and country to country. (Can cover near infinite geographical distance)
	- **Modem** and **Satellite** are the two primary ways to enable WAN connections
- The Largest example of WAN is Internet

#### Histroy of WEB and HTML
- Timothy Berners Lee Team laid the foundations for the **World Wide Web**, or the **Web**, in 1989
- They Developed a system of interconnected **hypertext documents** that allowed their users to easily navigate from one topic to another

### Introducing HTML 
- A web page is a text file written in **hypertext Markup Language**
- A **markup language** is a language that describes the content and struture of a document by identifying/tagging different elements in the documents.


#### Hypertext
- Hypertext is a method of organization in which data sources are interconnected through a series of links or hyperlinks that users can activate to jump from one piece of information to another

#### WebPage/ Web Server/ Web Browser
- Web page: Each document on the World Wide Web
- Web pages store on **Web Servers** 
- A Web browser retrieves the page from the Web server and renders it on the user’s computer or other device

Example: This is a [My First HTML Page](./HTML/act1_feb13.html)

### HTML elements/tags
Most elements are coded as a pair of tags: an opening tag and a closing tag. Tags are enclosed in angle brackets, "<" and ">" symbols.
- `<h1></h1>` to `<h6></h6>` 6 heading tags
- `<p></p>` paragraph tag
- `<ul> </ul>` unordered list tag creates a list with indentation
- `<ol> </ol>` ordered list with numbers
- `<li></li>` is used inside `<ul></ul>` or `<ol></ol>`
- if we use `<li></li>` without `<ul>` or `<ol>`, there will be bullets without indentation
- `<!DOCTYPE html>` helps browser to open the file properly on different divces 
- `<a href="./act1_feb13.html">Go to Page 1</a>` Anchor tag helps to create a hyperlink.
- `<blockquote></blockquote>` specifies a section that is quoted from another source. Browsers usually indent `<blockquote>` elements
- `<strong></strong>` Defines important text in bold text
- `<br>` line break, it gives a big space. it has no end tag
- `<dl></dl>` defines a description list. It's used toger with `<dt>` and `<dd>` inside. 
- `<dt>` (defines terms/names), it shows on the left.
- `<dd>` (describes each term/name), it shows on the right.
```
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```
- HTML Trademark Symbol: `&trade` &trade;
- HTML Coperight Symbol: `&copy` &copy;

### Adding Styles to a page
- add style or format inline by using the "style" attribute in each opening tag
	- style = "style_name: style_value;"
	- `<p style = "color:darkblue;">example<p>`


## Session 2 on Feb 14

### What is CSS
- Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language.
- CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.

#### Three Ways to Insert CSS
- **Inline style sheet**
	– An inline style may be used to apply a unique style for a single element.
	- Try to not use Inline CSS because it's hard to modify
- **Embedded/Internal Style sheet**
	– Internal styles are defined within the `<style>` element, inside the `<head>` section of an HTML page.
- **External style sheet**
	– Create an external style sheet file and link it to web pages.

#### Defining a Style Rule
- The general syntax of a CSS style rule is: 
	```
	selector {
		property1: value1; 
		property2: value2; 
		property3: value3;
	}
	```

- The selctor could be a Tag, for example: 
	  ```p{
            color:darkgreen;
            font-size: 25px;
        }```
- The selectror can be a **#id** which was assigned to a single tag, e.g.:
	    ```#item{
	            color:darkorange;
	        }```
	    where the #item id was assigned to a `<p>` tag in HTML:
	    `<p id="item">We're practicing CSS today!</p>`
- The selector can be a **.class** which was assigned to a groups of elements:
	- Step1: Declase a class for a group of tags
		```
		<p class="yellowItems">Paragraph 11</p>
		<p class="yellowItems">Paragraph 12</p>
		<p class="yellowItems">Paragraph 13</p>
		```
	- Step2: Declare style using **.class_name**
    	```
    	.yellowItems{
			color:yellowgreen;
		}
		```
    	

#### External style sheet
- Link a HTML to a CSS file :
	- Use a link tag inside the head tag:
	`<link rel="stylesheet" type="text/css" href="mystyle.css">`

#### Add images to a page
- The **`<img>`** tag defines an image in an HTML page.
- The **alt** attribute defines an **alternative** text description of the image when images is not showed.
- The **src** attribute specifies the URL/path of an image

	`<img src="./images/image1.jpg" alt="party1 description" height="150" >`

#### HTML Tabels
- An HTML table is defined with the `<table>` tag.
	- Each table row is defined with the `<tr>` tag. A table header is defined with the `<th>` tag. By default, table headings are bold and centered. A table data/cell is defined with the `<td>` tag.
- Table header 	`<th>` gives a bold centered text. 
- Adding a Border by using the **border** attribute:
	- add border attribute to the table tag
	```
	<table border="1">
        <tr>
            <td>Row1 Column1</td>
            <td>Row1 Column2</td>
        </tr>
        <tr>
            <td>Row2 Column1</td>
            <td>Row2 Column2</td>
        </tr>
    </table>
    ```
    <table>
        <tr>
            <td>Row1 Column1</td>
            <td>Row1 Column2</td>
        </tr>
        <tr>
            <td>Row2 Column1</td>
            <td>Row2 Column2</td>
        </tr>
    </table>
- The border attribute of `<table>` is not supported in HTML5. Use CSS border property instead:
	```
	<style>
	    table,tr,th,td{
	        border: 1px solid black;
	        border-collapse: collapse;
	    }   
	</style>
	```

#### Styling a table by CSS
- nth-child selector: For zebra-striped tables, use the **nth-child()** selector and add a background-color to all even (or odd) table rows:
	`tr:nth-child(even) {background-color: #f2f2f2;}`

## Session 3 on Feb 18
### Layout
- Page layout is the part of web design that deals in the arrangement of visual elements on a page.
- Design layout by using HTML Layout :
	- `<div>` Elements
	- HTML Tables
	- HTML5 elements
		-use `<header>`, `<nav>`, `<section>`, `<footer>`, etc. Will talk after midterm

- The `<div>` element is often used as a layout tool, because it can easily be positioned with CSS.
		- The `<div>` element is a block level element used for grouping HTML elements.
		- It's a container unit that encapsulates other page elements and divides the HTML document into sections.
		- Web developers use `<div>` elements to group together HTML elements and apply CSS styles to many elements at once.

- Pixel is the unit of measurement. In digital imaging, a pixel, pel, or picture element is a physical point in a raster image. It is the smallest controllable element of a picture represented on the screen. The normal screen size is about 1400 × 800 px.

- Styling CSS properties:
	- background-color, color; 
	- text-align: center;
	- height: auto;
	- width: auto;
	- **margin** is the space between the element and the screen. 
	- **padding** is the space between the border and the content.
	- use **float** to place divs side by side.
	- font-size, font-style

## Session 3 on Feb 19
### HTML 5 LAYOUT ELEMENTS
Instead of using `<div>` and assign id to it, HTML5 offers new semantic elements that define the different parts of a web page:
- `<header>` - Defines a header for a document or a section.
- `<nav>` - Defines a container for navigation links.
- `<main>` - Specifies the main content of a document.
- `<section>` - Defines a section in a document.
- `<article>` - Defines an independent self-contained article.

#### Add Multimedia to Web Page
- Adding HTML5 Audio, where url1, url2, etc. are the possible sources of the audio clip.
	```
	<audio>
		<source src=”url1” /> 
		<source src=”url2” />
	</audio>
	```
- Adding Video in HTML5
	```
	<video>
		<source src=”url1” /> <source src=”url2” /> ...
	</video>
	```

- `<audio>` tag Attributes:
	- autoplay: Specifies that the audio will start playing as soon as it is ready
	- controls: Specifies that audio controls should be displayed (such as a play/pause button etc)
	- loop: Specifies that the audio will start over again, every time it is finished
	- muted: Specifies that the audio output should be muted

### Web Form Feb 20
Web forms collect information from Web site visitors.
- HTML supports the following control elements:
	- Inputboxes
	- Option buttons 
	- Selection lists 
	- Check boxes
	- Text areas

#### How to Process/Collect form data?
To collect/process form data, a server-side or client-side program is is required
- Server-side programs are written in many languages including PHP, Python, ASP, ...
- Client-side programs are written in JavaScript, ReactJS, ...

```
<form attributes> 
	content
</form>
```
- HTML Input Types
Here are the different input types you can use in HTML form:
	- `<input type="text">`
	- `<input type="date">`
	- `<input type="email">`
	- `<input type="number">`
	- `<input type="submit" value="Register">` gives a Register button
	- by giving **name** attribute to `<input>`, user can ONLY select one radio button
	- The input **value** attribute specifies an initial value for an input field:
	```
	        <p>Do u need extra insurance: 
            <input type="radio" name="insurance" value="y">Yes
            <input type="radio" name="insurance" value="n">No
        	</p>
	```


[Learn more about web form](https://www.w3schools.com/html/html_forms.asp)

- HTML 5 standard: for self closing tag, it's better to have a / before > `<input type="email"/`
- Creat a comment box using `<textarea>`
	- The `<textarea>` tag defines a multi-line text input control.
	- The size of a text area can be specified by the **cols** and **rows** attributes, or even better; through CSS' height and width properties.
	- **placeholder** attribute specifies a short hint that describes the expected value of a text area
-  `<select>` Tag create a drop-down list with options
	- The `<option>` tags inside the `<select>` element define the available options in the list.
	```
    <select name="city" id="city">
        <option value="Chongqing">Chongqing</option>
        <option value="Toronto">Toronto</option>
        <option value="NewYork">New York</option>
    </select>
    ```




	