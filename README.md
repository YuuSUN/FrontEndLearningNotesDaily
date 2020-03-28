# FrontEndLearningNotesDaily
## Menu 

Week | Mon | Tue | Wed | Thu | Fri | Sat | Sun  
:-: | :-: | :-: | :-: | :-: | :-: | :-: | :-:
March 16-22  | | | [1](https://github.com/YuuSUN/FrontEndLearningNotesDaily#20200318day-one-html-basics)| [2](https://github.com/YuuSUN/FrontEndLearningNotesDaily#20200319day-two-html-semantic-elements) | | | | 
March 23-29 | | [3](https://github.com/YuuSUN/FrontEndLearningNotesDaily/blob/master/README.md#20200324day-three-css-basics) | [4](https://github.com/YuuSUN/FrontEndLearningNotesDaily/blob/master/README.md#20200325day-four-styling-design) | | | [5]()| |  

- [Day One: HTML Basics](https://github.com/YuuSUN/FrontEndLearningNotesDaily#20200318day-one-html-basics)
- [Day Two: HTML Semantic Elements](https://github.com/YuuSUN/FrontEndLearningNotesDaily#20200319day-two-html-semantic-elements)
- [Day Three: CSS Basics](https://github.com/YuuSUN/FrontEndLearningNotesDaily/blob/master/README.md#20200324day-three-css-basics)
- [Day Four: Styling Design](https://github.com/YuuSUN/FrontEndLearningNotesDaily/blob/master/README.md#20200325day-four-styling-design)
- [Day Five: List, Link, Selector]()


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
- A simple HTML document: Only the content inside the ``` <body>```  section is displayed in a browser.
``` 
<head>
<title>Page Title</title>
</head>
``` 


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

### 【2020/03/24】Day Three: CSS Basics
#### 1. What is CSS 
- CSS is used to style and lay out web pages such as alter the font, spacing of the content, split it into multiple columns or add animations or other decorative features. 
- A browser is sometimes called a user agent, which basically means a computer program that represents a person inside a computer system. Browsers are the main type of user agent we think of when talking about CSS, however, it is not the only one. There are other user agents available — such as those which convert HTML and CSS documents into PDFs to be printed.

#### 2. CSS syntax 
```
h1 {
    color: red;
    font-size: 5em;
}
```
- The rule opens with a selector. It selects the HTML element that we are going to style. In this case we are styling level one headings h1.
- We then have a set of curly braces ``` { }```. Inside those will be one or more declarations, which take the form of **property** and **form** pairs. Each pair specifies a property of the element we are selecting, then a value that we'd like to give the property. 
- Before the colon, we have the property, and after the colon, the value. 
- A CSS selector is part of a CSS rule that describes what element in a document the rule will match. 
```
p {
  color: green;
}

div.warning {
  width: 100%;
  border: 2px solid yellow;
  color: white;
  background-color: darkred;
  padding: 0.8em 0.8em 0.6em;
}

#customized {
  font: 16px Lucida Grande, Arial, Helvetica, sans-serif;
}
```
```
<p>This is happy text.</p>

<div class="warning">
  Be careful! There are wizards present, and they are quick to anger!
</div>

<div id="customized">
  <p>This is happy text.</p>

  <div class="warning">
    Be careful! There are wizards present, and they are quick to anger!
  </div>
</div>
```
- A property paired with a value is called a CSS declaration.
- "div.warning" (which makes any div element with the class "warning" look like a warning box), and "#customized", which sets the base font of the element with the ID "customized" to 16-pixel tall font.
- You can target multiple selectors at once, by separating the selectors with a comma. ```p, li { }```

#### 3. Adding css to our document 
- Create a file in the same folder as your HTML document and save it as styles.css. The .css extension shows that this is a CSS file.
- To link **styles.css** to **index.html** add the following line somewhere inside the ```<head>``` of the HTML document:
```
<link rel="stylesheet" href="styles.css">
```
- This ```<link> ```element tells the browser that we have a stylesheet, using the rel attribute, and the location of that stylesheet as the value of the href attribute. 

#### 4. Adding a class
- You want to select a subset of the elements without changing the others. 
- In HTML document add a class attibute: ```<li class="special">Item two</li>```
- In CSS document you can target the class of **special** by creating a selector that starts with a full stop character: ```.special { }```

#### 5. Styling things based on their location in a document 
- descendant combinator（后代选择器）: A selector to select an element that is nested inside an another element. ```li em { }```
- adjacent sibling combinator（相邻选择器）: A selector to select an element directly after an another element at the same hierarchy. ```h1 + p { }```
- More ways to target elements: [CSS selector summary](https://www.w3cschool.cn/css/css-selector.html)

#### 6. Styling things based on state
- a straightforward example of this is when styling links. When we style a link we need to target ```<a>```(anchor) element. This has different states depends on whether it is unvisited, visited, being hovered over, focused via the keyboard, or in the process of being clicked (activated)
```
a:link {
  color: pink;
}

a:visited {
  color: green;
}
```
#### 7. How CSS is structured
- External Stylesheet 
```
<!-- Inside a subdirectory called styles inside the current directory -->
<link rel="stylesheet" href="styles/style.css">

<!-- Inside a subdirectory called general, which is in a subdirectory called styles, inside the current directory -->
<link rel="stylesheet" href="styles/general/style.css">

<!-- Go up one directory level, then inside a subdirectory called styles -->
<link rel="stylesheet" href="../styles/style.css">
```
- Internal Stylesheet: An internal stylesheet is where you don't have an external CSS file, but instead place your CSS inside a ```<style>``` element contained inside the HTML ```<head>```.
```
<head>
    <meta charset="utf-8">
    <title>My CSS experiment</title>
    <style>
      h1 {
        color: blue;
        background-color: yellow;
        border: 1px solid black;
      }
    </style>
  </head>
```
- Inline styles. They are css declarations that affect one element only, contained within a **style** attribute. 
```<h1 style="color: blue;background-color: yellow;border: 1px solid black;">Hello World!</h1>```
- Valid selectors
```
h1
a:link
.manythings
#onething
*
.box p
.box p:first-child
h1, h2, .intro
```
#### 8. which rule will win in the event of a collision
- These are called cascade or specificity. The paragraph ends up being colored blue. This is because the declaration that sets it to blue appears later in the stylesheet, and later styles override earlier ones. This is the cascade in action.
- However, the class will win the element over, even though it appears earlier in the stylesheet. A class is described as being more specific, or having more specificity than the element selector, so it wins.

### 【2020/03/25】Day Four: Styling Design
#### 1. Function
- While most values are relatively simple keywords or numeric values, there are some possible values which take the form of a function.
- calc() function. This function allows you to do simple math from within your CSS.
- ```width: calc(90% - 30px); ```Asking for the width of this box to be 90% of the containing block width, minus 30 pixels.
![image](https://github.com/YuuSUN/FrontEndLearningNotesDaily/blob/master/Images/pic1.png?raw=true)
- transform: rotate(0.8turn)
#### 2. @rules
- Some **@rules** are simple with the rule name and a value. For example, to import an additional stylesheet into your main CSS stylesheet you can use **@import**: ``` @import 'styles2.css';```
- One of the most common @rules you will come across is **@media**, which allows you to use media queries to apply CSS only when certain conditions are true (e.g. when the screen resolution is above a certain amount, or the screen is wider than a certain width).
#### 3. Shorthands
- Some properties like font, background, padding, border, and margin are called shorthand properties — this is because they allow you to set several property values in a single line, saving time and making your code neater in the process.
```/* In 4-value shorthands like padding and margin, the values are applied
   in the order top, right, bottom, left (clockwise from the top). There are also other 
   shorthand types, for example 2-value shorthands, which set padding/margin
   for top/bottom, then left/right */
padding: 10px 15px 15px 5px;
```
#### 4. How does CSS actually work
- The browser converts the HTML into a DOM (Document Object Model). The DOM represents the document in the computer's memory.
- The browser then fetches most of the resources that are linked to by the HTML document, such as embedded images and videos ... and linked CSS! JavaScript is handled a bit later on in the process.
- The browser parses the fetched CSS, and sorts the different rules by their selector types into different "buckets", e.g. element, class, ID, and so on. Based on the selectors it finds, it works out which rules should be applied to which nodes in the DOM, and attaches style to them as required (this intermediate step is called a render tree).
- The render tree is laid out in the structure it should appear in after the rules have been applied to it.
- About the DOM. A DOM has a tree-like structure. Each element, attribute, and piece of text in the markup language becomes a DOM node in the tree structure. The nodes are defined by their relationship to other DOM nodes. Some elements are parents of child nodes, and child nodes have siblings.
- How a real HTML snippet is converted into a DOM:
```
<p>
  Let's use:
  <span>Cascading</span>
  <span>Style</span>
  <span>Sheets</span>
</p>
```
- In the DOM, the node corresponding to our ```<p>``` element is a parent. Its children are a text node and the three nodes corresponding to our``` <span> ```elements. The SPAN nodes are also parents, with text nodes as their children:
```
P
├─ "Let's use:"
├─ SPAN
|  └─ "Cascading"
├─ SPAN
|  └─ "Style"
└─ SPAN
   └─ "Sheets"
```
- Applying CSS to the DOM: The browser will apply that rule to each one of the three ```<span>```s, then paint the final visual representation to the screen. 
- What happens if a browser encounters css it doesn't understand: It does nothing and just moves on to the next bit of css.

#### 5. Text and font styling
- Bear in mind that the text inside an element is all affected as one single entity. You can't select and style subsections of text unless you wrap them in an appropriate element (such as a ```<span>``` or ```<strong>```), or use a text-specific pseudo-element like ::first-letter (selects the first letter of an element's text), ::first-line (selects the first line of an element's text), or ::selection (selects the text currently highlighted by the cursor.)
- px (pixels): The number of pixels high you want the text to be. This is an absolute unit — it results in the same final computed value for the font on the page in pretty much any situation.
- **em**s: 1 em is equal to the font size set on the parent element of the current element we are styling (more specifically, the width of a capital letter M contained inside the parent element.) This can become tricky to work out if you have a lot of nested elements with different font sizes set, but it is doable, as you'll see below. Why bother? It is quite natural once you get used to it, and you can use **em** to size everything, not just text. You can have an entire website sized using em, which makes maintenance easy.
- **rem**s: These work just like **em**, except that 1 **rem** is equal to the font size set on the root element of the document (i.e. ```<html>```), not the parent element. This makes doing the maths to work out your font sizes much easier, although if you want to support really old browsers, you might struggle — rem is not supported in Internet Explorer 8 and below.
- **Text-transform**: **Capitalize** transforms all words to Have The First Letter Capitalized.
- **Text-align**: **justify** makes the text spread out, varing the gaps in between the words so that all lines of text are the same width. If you are going to use this, you should also think about using something else along with it, such as **hyphens**, to break some of the longer words across lines.
**letter-spacing** and **word-spacing** improve the legibility of a particularly dense font. apply it to the first line: ```p::first-line {}```
**Opacity**: When using the opacity property to add transparency to the background of an element, all of its child elements **inherit the same transparency**. This can make the text inside a fully transparent element hard to read.
