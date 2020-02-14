# Webmaster Content Notes
## Session 1 on Feb 13

#### LAN vs WAN
LAN is Local Area Network 
WAN is Wide Area Network
- WAN is a network using WAN connections
- The Largest example of WAN is Internet

#### Histroy of WEB and HTML
- Timothy Berners Lee Team laid the foundations for the **World Wide Web**, or the **Web**, in 1989
- They Developed Hypertext documents

### Introducing HTML 
- A web page is a text file written in **hypertext Markup Language**
- A **markup language** is a language that describes the content and struture of a document by identifying/tagging different elements in the documents.


#### Hypertext

#### WebPage/ Web Server/ Web Browser
- Web page: Each document on the World Wide Web
- Web pages store on **Web Servers** 

Example: This is a [My First HTML Page](./myFirstPage.html)

### HTML tags
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
