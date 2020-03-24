# FrontEndLearningNotesDaily
## Menu 

Week | Mon | Tue | Wed | Thu | Fri | Sat | Sun  
:-: | :-: | :-: | :-: | :-: | :-: | :-: | :-:
March 16-22  | | | [1](https://github.com/YuuSUN/FrontEndLearningNotesDaily#20200318day-one-html-basics)| [2](https://github.com/YuuSUN/FrontEndLearningNotesDaily#20200319day-two-html-semantic-elements) ||||

- [Day One: HTML Basics](https://github.com/YuuSUN/FrontEndLearningNotesDaily#20200318day-one-html-basics)
- [Day Two: HTML Semantic Elements](https://github.com/YuuSUN/FrontEndLearningNotesDaily#20200319day-two-html-semantic-elements)


### 【2020/03/18】Day One: HTML Basics
#### 1. What is HTML  

- Hypertext Markup Language. e.g. If you want to publish the content of rich-text on the forum, you need some codes additionally. 

```html
[del]Arschloch[/del]
``` 
- The example indicates the text between labels should be deleted. Strikethrough effect will be added by default. 
- HTML and CSS(Cascading Style Sheet 层叠样式表)are two of the core technologies for building web pages. HTML builds the structure of page, CSS the layout. 
- retrieve online information via hypertext links, at the click of a button.
- With HTML, authors describe the structure of pages using markup. The elements of the language label pieces of content such as “paragraph,” “list,” “table,” and so on.

#### 2. What is XHTML
- XHTML is the variant of HTML that using the syntax of XML, the extensible markup language. XHTML has all the same elements as the HTML variant, but the syntax is slightly different. Because XHTML is a XML application, you can use other XML tools with it.

#### 3. What is CSS
- CSS is the language for describing the presentation of web pages, including colors, layout and fonts. It allows one to adapt the presentation to different types of devices. CSS is independent of HTML and can be used with any XML-based markup language. The separation of HTML from CSS makes it easier to maintain sites, share style sheets across pages, and tailor pages to different environments.

#### 4. What is Javascript 
- Tools for adding dynamic effects to web pages
- e.g. Creat a ```<div>```（块级元素）window when mouse hovering over the label.

#### 5. Examples
The following very simple example of a portion of an HTML document illustrates how to create a link within a paragraph. When rendered on the screen (or by a speech synthesizer), the link text will be “final report”; when somebody activates the link, the browser will retrieve the resource identified by “http://www.example.com/report”:
```
<p class="moreinfo">For more information see the
<a href="http://www.example.com/report">final report</a>.</p>
``` 
The class attribute on the paragraph's start tag (“```<p>```”) can be used, among other thing, to add style. For instance, to italicize the text of all paragraphs with a class of “moreinfo,” one could write, in CSS:    

``` 
  p.moreinfo { font-style: italic }
``` 
By placing that rule in a separate file, the style may be shared by any number of HTML documents.

#### 6. More Information
For more information about HTML and CSS, see [tutorials for HTML and CSS](https://www.w3.org/2002/03/tutorials.html#webdesign_htmlcss).  

For advanced document transformations and layout beyond CSS, see [XSLT](https://www.w3.org/standards/xml/transformation) & [XSL-FO](https://www.w3.org/standards/xml/publishing).



 

 
### 【2020/03/19】Day Two: HTML Semantic Elements 
#### 1. What are semantic elements
- Semantic elements = elements with a meaning 
- Semantic elements describes its meaning to both the browser and the developer.
- Examples of **none-semantic** elements: ``` <div>``` and ``` <span>``` - Tells nothing about its content.
- Examples of **semantic** elements: ``` <form>``` ,``` <table>``` and ``` <article>``` - Clearly defines its content.

#### 2. What is HTML5
- HTML5 is the newest standard of html, it has more abundant semantics, graphics and multimedia contents. 

#### 3. What is doctype 
- ```<!DOCTYPE>``` declaration help the browser show the web correctly. 
- HTML has many different versions. Only when the browser understand the exact version of html can it show the content correctly.

#### 4. HTML Emelments 
- An HTML element usually consists of **start** tag and an **end** tag. ```<tagname>content goes here</tagname>```
- The html element is everything from the start tag to the end tag. 
- HTML elements with no content are called empty elements. Empty elements do not have an end tag such as the ```<br>```element (which indicates a line break)
- HTML elements can be nested (elements can contain elements).
- The ```<html>``` element defines the whole document. Inside the ```<html>``` element is the ```<body>``` element. 
- HTML5 does not require empty elements to be closed. But if you want stricter validation, or if you need to make your document readable by XML parsers, you must close all HTML elements properly.
- HTML is Not Case Sensitive: ```<P>``` means the same as ```<p>```. 

#### 5. Semantic elements in html
- "A semantic Web allows data to be shared and reused across applications, enterprises, and communities."
- Many web sites contain HTML code like: ```<div id="nav"> <div class="header"> <div id="footer">``` to indicate navigation, header, and footer.
- ```<article> <aside> <details> <figcaption> <figure> <footer> <header> <main> <mark> <nav> <section> <summary> <time>```
- The ```<nav>``` element defines a set of navigation links.
- Notice that NOT all links of a document should be inside a ```<nav>``` element. The ```<nav>``` element is intended only for major block of navigation links.
- An image and a caption can be grouped together in a ```<figure>``` element. The purpose of a caption is to add visual explaination to an image. It speicifies self contained content, like illustrations, diagrams, photos, code listings, etc.
```
<figure>
  <img src="pic_trulli.jpg" alt="Trulli" style="width:100%">
  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption>
</figure>
```
- The ```<img>``` element defines the image. The ```<figcaption>``` element defines the caption.
- ```<details>``` defines additional details that the user can view or hide.
- ```<main>``` defines the main content of a document. 
- ```<mark>``` defines the marked or highlighted text.
- ```<summary>``` defines a visible heading for a ```<details>``` element.
  
#### 6. Nesting article in section or Vice Versa?
- The```<article>``` element specifies independent, self-contained content.
- The ```<section>``` element defines section in a document.
- You will also find pages with ```<section>``` elements containing ```<section>``` elements, and ```<article>``` elements containing ```<article>``` elements.
- Example for a newspaper: The sport ```<article>``` in the sport **section**, may have a technical **section** in each ```<article>```.
  
#### 7. HTML Links
- When you move the mouse over a link, the mouse arrow will turn into a little hand.
- A link does not have to be text. It can be an image or any other HTML element.
- Syntax: Hyperlinks are defined with the HTML ```<a>``` tag.
```<a href="url">link text</a>```
- The **href** attibute specifies the destination address of the link.
- The **Link text** is the visible part. 
- Note: Without a forward slash at the end of subfolder addresses, you might generate two requests to the server. Many servers will automatically add a forward slash to the end of the address, and then create a new request.
- A local link (link to the same web site) is specified with a relative URL (without https://www....).
```
<p><a href="html_images.asp">HTML Images</a> is a link to a page on this website.</p>
<p><a href="https://www.w3.org/">W3C</a> is a link to a website on the World Wide Web. An absolute URL (a full web address)</p>
```
- The ```<target>``` attribute specifies where to open the linked document. It has different values.
- ```_blank``` Opens the linked document in a new window or tab
- ```_self``` Opens the linked document in the same window/tab as it was clicked (this is default)
- ```_parent``` Opens the linked document in the parent frame
- ```_top``` Opens the linked document in the full body of the window
- framename - Opens the linked document in a named frame
```
<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
```
- Image as a link
```
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;border:0;">
</a>
```
- Button as a link. To use a html button as a link, you have to add some javascript code. Javascipt allows you to specify what happens at certain events, such as a click of a button.
```
<button onclick="document.location = 'default.asp'">HTML Tutorial</button>
```
- The **title** attribute specifies extra information about an element. The information is most often shown as a tooltip text when the mouse moves over the element.
```
<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>
```


