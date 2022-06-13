# HTML & CSS Fundamentals study guide

Included within this document is a list of fundamental concepts regarding two of the web's core building blocks - HTML and CSS.
Links to further materials and resources are provided within each subsection.
Once you have worked your way through this document, it is expected that you will have a grasp on the core concepts of HTML and CSS.

## HTML

HTML (HyperText Markup Language) defines the structure and content of a web page. Ultimately, it consists of a series of elements
which you use to wrap different parts of a web page's content to make it appear or behave in a certain way.
Within this section is a brief breakdown of the core HTML fundamentals.

A good place to start learning about HTML is MDN's [HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics#so_what_is_html),
which outlines the basic building blocks of HTML. You can read up until the Images section to get a good idea of how to define
an HTML element, nesting elements inside one another, what empty elements are, as well as the basic anatomy of an HTML document.

### HTML Elements

#### Defining HTML Elements

Looking through the HTML Basics article above, you would have seen that a typical HTML element is defined using tags,
and that there are two types of HTML elements: open and closed elements.

Example of a paragraph element, defined by it's open &lt;p> tag, the text content in the middle of the two tags, and the 
closing &lt;p\>:
```html
  <p>This is an example of an open paragraph element</p>
```

Example of a closed input element, defined only by its &lt;input> tag:
```html
  <input>
```

Another great resource to work through is CodeAcademy's [Elements and Structure course](https://www.codecademy.com/learn/learn-html/modules/learn-html-elements). 
CodeAcademy offers a free platform to learn the basics of HTML, CSS & JavaScript and offer short courses that will teach you theory and reinforce concepts with
short practical based questions. The Elements and Structure course is a good place to get a deeper look at concepts touched on in the MDN article above.

#### Element Types

There are an incredible amount of elements, each with their own rules and purposes. Below are some of the more common HTML elements which are useful to know:

- [body](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body): Represents the content of an HTML document. There can only ever be one body element in a document.
- [main](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/main): Used to represent the dominant content of the [&lt;body>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body) of a document.
- [div](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/div): Arguably the web's most used and generic element. The div does not inherently represent anything, but is used as a container to group and divide content. It is important to note the div element is only used when there are no other [semantic HTML elements](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#semantics_in_html) that will represent the content being surrounded in a more appropriate manner.
- [span](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/span): Another one of the web's most used generic element. Like the div, the span is also a generic container, however they differ in how they affect the HTML content they surround. Div elements are inherently [block-level](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements) whereas spans are referred to as being [inline elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Inline_elements). This will be discussed further in the CSS section to come, but it is an important distinction to make. Like Divs, spans should be used only when no other semantic element is appropriate
- [p](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p): Represents a paragraph element. Usually represented as blocks of text.
- [ul](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul): Represents an unordered list of items, typically rendered as a bulleted list.
- [ol](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol): The ordered list represents a list of ordered items, typically rendered as a numbered list.
- [li](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/li): The list item element is used to represent an item in a list. They are typically placed within the &lt;ul> and &lt;ol> elements.
- [input](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input): Used to create an interactive control for the web. There are different types of input elements which can be specified using their type attribute. More on this when we talk about attributes.
- [select](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/select): Also an interactive element that provides a menu of options
- [option](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/option): Used to define an item contained in &lt;select>, [&lt;optgroup>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/optgroup), and [&lt;datalist>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/datalist) elements
- [button](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button) An interactive element that can be activated by the user and performs a programmable action.
- [a](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a): Know as an anchor element and used to create a hyperlink that can link to anything a URL can address (i.e. web pages, email addresses, locations on the same web page etc.)
- [nav](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav): The navigation section element is used to represent a section of the page used to provide navigational links either within the current document, or to other documents.
- [header](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header): Represents introductory content, usually a group of introductory navigational aids. 
- [h1-h6](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements): The &lt;h1> to &lt;h6> elements represent the various levels of section headings, &lt;h1> being the highest, and &lt;h6> being the lowest.
- [footer](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer): Contains information about the author of the section, copyright data or links to related documents.
- [section](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/section): Represents a generic standalone section of a document that doesn;t have a more specific element to represent it. They should usually have an associated heading.
- [article](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article): Represents a self-contained item of content in a document, page, application or site, which is intended to be independently distributable or reusable.
- [aside](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/aside): A portion of a document whose content is only indirectly related to the document's main content.
- [svg](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/svg): A powerful element that ultimately allows you to define SVG documents, or to embed an SVG fragment inside an SVG or HTML document.
- [template](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/template): Provides a mechanism for holding HTML that is not rendered when the page is initially loaded, but can be created at runtime using Javascript.

For a breakdown on all the HTML elements available, you can refer to MDN's [HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).
This is a great resource to bookmark as it provides each HTML tag, a link to the documentation of that element, and a short description of what that element represents.

#### Element Attributes and Properties

#### Accessibility
- aria-label
- roles
- tabindex
- kieran to fill in link to aria guide

#### HTML document structure
  - script element
  - style element
  - head, body elements
  - link to mdn document structure

  - Dev tools elements inspector
      - what is it
      - how to use it
      - link to dev tools info for elements
## CSS
- What is CSS
- Inline style vs style element and style sheet
- CSS selectors
- css display property e.g display block
- margin and padding properties
- colors background etc
- sizing elements
- border property
- pseudo class e.g :hover, :focus
- media rules / queries
- css flexbox
- css grid