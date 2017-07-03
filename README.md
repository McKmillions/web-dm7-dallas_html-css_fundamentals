# HTML &amp; CSS Fundamentals (web-dm7-dallas)


## Pre-Class
[https://www.codecademy.com/learn/learn-html-css](https://www.codecademy.com/learn/learn-html-css)

Using HTML & CSS is one of the most important things to learn. Employers judge your projects based on looks then functionality. If they see your project and it looks poorly designed they will less likely remember your project.

## Intro to HTML
HTML is not a programming language; it is a markup language. It's used to tell your browser how to structure the webpage. The browser (Chrome, Firefox, Safari) will parse the code then show on the screen. The markup code is referred to as an element or a tag.
HTML consists of elements that the web developer can use to make content appear and act a certain way.


**H** - `Hyper`
**T** - `Text`
**M** - `Markup`
**L** - `Language`

HTML5 is the current version

**Anatomy of an Paragraph Tag**
![alt tag](https://raw.githubusercontent.com/McKmillions/web-dm7-dallas_html-css_fundamentals/master/img/anatomy-of-an-paragraph-element.png)

1. The opening tag
⋅⋅* name of the element
⋅⋅* open and close angle Brackets < > wraps the element

2. The closing tag
⋅⋅* Same as opening but with a forward slash to state where the element ends

3. The content
⋅⋅* This is the content of the element

4. The element
⋅⋅* The opening tag, plus the closing tag, plus the content, equals the element.



## HTML Elements
* `p` - A paragraph or block of text. Paragraphs are block-level elements
* `footer`
* `header`
* `h1 - h6` - H1 is the biggest. H6 is the smallest. Only one H1 per page (SEO)
* `ul` - Bullets on document or used for navigation
* `li`
* `div` - Like a container

<details>
<summary>Block-level elements</summary>
HTML elements are usually either "block-level" elements or "inline" elements. A block-level element occupies the entire space of its parent element (container), thereby creating a "block." Browsers typically display the block-level element with a newline both before and after the element. You can visualize them as a stack of boxes.

<address> - Contact information.
<article> - Article content.
<aside> - Aside content.
<blockquote> - Long ("block") quotation.
<canvas> - Drawing canvas.
<dd> - Describes a term in a description list.
<div> - Document division.
<dl> - Description list.
<dt> - Description list term.
<fieldset> - Field set label.
<figcaption> - Figure caption.
<figure> - Groups media content with a caption (see <figcaption>).
<footer> - Section or page footer.
<form> - Input form.
<h1>, <h2>, <h3>, <h4>, <h5>, <h6> - Heading levels 1-6.
<header> - Section or page header.
<hgroup> - Groups header information.
<hr> - Horizontal rule (dividing line).
<li> - List item.
<main> - Contains the central content unique to this document.
<nav> - Contains navigation links.
<noscript> - Content to use if scripting is not supported or turned off.
<ol> - Ordered list.
<output> - Form output.
<p> - Paragraph.
<pre> - Preformatted text.
<section> - Section of a web page.
<table> - Table.
<tfoot> - Table footer.
<ul> - Unordered list.
<video> - Video player.
</details>

<details>
<summary>Inline elements</summary>
An inline element occupies only the space bounded by the tags that define the inline element. By default, inline elements do not begin with new line.

<a> - Anchor.
<b> - Boldface.
<big> - Makes text one font size bigger.
<i> - Italicize.
<small> - Makes text one font size smaller.
<tt> - Displays text in browser's default monotype font.
<abbr> - Abbreviation.
<cite> - Reference to a creative work.
<code> - Fragment of computer code.
<dfn> - Defining instance of a term.
<em> - Text that has stress emphasis.
<kbd> - User Input
<strong> - Gives text strong importance, and is typically displayed in bold.
<samp> - Element intended to identify sample output from a computer program.
<time> - Represents either a time on a 24-hour clock or a precise date in the Gregorian calendar
<var> - A variable in a mathematical expression or a programming context.
<bdo> - (bidirectional override) is used to override the current directionality of text.
<br> - Produces a line break in text (carriage-return).
<img> - Image in the document.
<map> - Defines an image map (a clickable link area).
<object> - External resource.
<q> - Indicates that the enclosed text is a short inline quotation.
<script> - Used to embed or reference an executable script.
<span> - A generic inline container for phrasing content. Used to group elements for styling.
<sub> - A span of text that should be displayed, lower, and often smaller, than the main span of text.
<sup> - A span of text that should be displayed, higher, and often smaller, than the main span of text.
<button> - Clickable button.
<input> - Used to create interactive controls for web-based forms in order to accept data from the user.
<label> - Caption for an item in a user interface.
<select> - A control that provides a menu of options.
<textarea> - Multi-line plain-text editing control.
</details>

An example of some of the above elements:
```html
<div class="section">
	<div class="header">
		<h1>I'm a Header</h1>
	</div>
	<div>
		<h1> Heading h1 </h1>
		<h2> Heading h2 </h2>
		<h3> Heading h3 </h3>
		<h4> Heading h4 </h4>
		<h5> Heading h5 </h5>
		<h6> Heading h6 </h6>
		<p> Paragraph : This is a paragraph </p>
		<ul>
			<li> List Item </li>
			<li> List Item </li>
			<li> List Item </li>
		</ul>
	</div>
</div>
```
But this way has a bunch of div's and can be harder to read

You can increase the readability of the html by using section tags.
```html
<section>
	<header> I'm a Header </header>
	<div>
		<h1> Heading h1 </h1>
		<h2> Heading h2 </h2>
		<h3> Heading h3 </h3>
		<h4> Heading h4 </h4>
		<h5> Heading h5 </h5>
		<h6> Heading h6 </h6>
		<p> Paragraph : This is a paragraph </p>
		<ul>
			<li> List Item </li>
			<li> List Item </li>
			<li> List Item </li>
		</ul>
	</div>
</section>
```

To further increase the readability of the elements you can use Main tag to put your navigation
```html
<!DOCTYPE html>
<html>
<head>
  <title>HTML &amp; CSS Fundamentals (web-dm7-dallas)</title>
	<link rel="stylesheet" type="text/css" href="css/style.css">
</head>
<body>
<main>
  <header>
    <nav>
      <ul>
        <li></li>
      </ul>
    </nav>
  </header>
  <section>
    <div>
      <h1> Heading h1 </h1>
      <h2> Heading h2 </h2>
      <h3> Heading h3 </h3>
      <h4> Heading h4 </h4>
      <h5> Heading h5 </h5>
      <h6> Heading h6 </h6>
      <p> Paragraph : This is a paragraph </p>
      <ul>
        <li> List Item </li>
        <li> List Item </li>
        <li> List Item </li>
      </ul>
    </div>
  </section>
</main>
<footer></footer>
</body>
</html>
```

## CSS properties
* `id (#) vs class(.) and specificity`
* `width px & %`
* `height px & %`
* `background-color`
* `background-image`
* `color`
* `font-size`
* `text-align: center`
* `line-height`
* `box-model (margin, padding, border)`
* `float`
* `clear`
