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


Tag | Description
------------ | -------------
&lt;address&gt; | Contact information.
&lt;article&gt; | Article content.
&lt;aside&gt; | Aside content.
&lt;blockquote&gt; | Long ("block") quotation.
&lt;canvas&gt; | Drawing canvas.
&lt;dd&gt; | Describes a term in a description list.
&lt;div&gt; | Document division.
&lt;dl&gt; | Description list.
&lt;dt&gt; | Description list term.
&lt;fieldset&gt; | Field set label.
&lt;figcaption&gt; | Figure caption.
&lt;figure&gt; | Groups media content with a caption (see &lt;figcaption&gt;).
&lt;footer&gt; | Section or page footer.
&lt;form&gt; | Input form.
&lt;h1&gt;, &lt;h2&gt;, &lt;h3&gt;, &lt;h4&gt;, &lt;h5&gt;, &lt;h6&gt; | Heading levels 1-6.
&lt;header&gt; | Section or page header.
&lt;hgroup&gt; | Groups header information.
&lt;hr&gt; | Horizontal rule (dividing line).
&lt;li&gt; | List item.
&lt;main&gt; | Contains the central content unique to this document.
&lt;nav&gt; | Contains navigation links.
&lt;noscript&gt; | Content to use if scripting is not supported or turned off.
&lt;ol&gt; | Ordered list.
&lt;output&gt; | Form output.
&lt;p&gt; | Paragraph.
&lt;pre&gt; | Preformatted text.
&lt;section&gt; | Section of a web page.
&lt;table&gt; | Table.
&lt;tfoot&gt; | Table footer.
&lt;ul&gt; | Unordered list.
&lt;video&gt; | Video player.
</details>

<details>
<summary>Inline elements</summary>

An inline element occupies only the space bounded by the tags that define the inline element. By default, inline elements do not begin with new line.


Tag | Description
------------ | -------------
&lt;a&gt; |Anchor.
&lt;b&gt; | Boldface.
&lt;big&gt; | Makes text one font size bigger.
&lt;i&gt; | Italicize.
&lt;small&gt; | Makes text one font size smaller.
&lt;tt&gt; | Displays text in browser's default monotype font.
&lt;abbr&gt; | Abbreviation.
&lt;cite&gt; | Reference to a creative work.
&lt;code&gt; | Fragment of computer code.
&lt;dfn&gt; | Defining instance of a term.
&lt;em&gt; | Text that has stress emphasis.
&lt;kbd&gt; | User Input
&lt;strong&gt; | Gives text strong importance, and is typically displayed in bold.
&lt;samp&gt; | Element intended to identify sample output from a computer program.
&lt;time&gt; | Represents either a time on a 24-hour clock or a precise date in the Gregorian calendar
&lt;var&gt; | A variable in a mathematical expression or a programming context.
&lt;bdo&gt; | (bidirectional override) is used to override the current directionality of text.
&lt;br&gt; | Produces a line break in text (carriage-return).
&lt;img&gt; | Image in the document.
&lt;map&gt; | Defines an image map (a clickable link area).
&lt;object&gt; | External resource.
&lt;q&gt; | Indicates that the enclosed text is a short inline quotation.
&lt;script&gt; | Used to embed or reference an executable script.
&lt;span&gt; | A generic inline container for phrasing content. Used to group elements for styling.
&lt;sub&gt; | A span of text that should be displayed, lower, and often smaller, than the main span of text.
&lt;sup&gt; | A span of text that should be displayed, higher, and often smaller, than the main span of text.
&lt;button&gt; | Clickable button.
&lt;input&gt; | Used to create interactive controls for web-based forms in order to accept data from the user.
&lt;label&gt; | Caption for an item in a user interface.
&lt;select&gt; | A control that provides a menu of options.
&lt;textarea&gt; | Multi-line plain-text editing control.
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
But this way has a bunch of div's and can be harder to read.

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

To further increase the readability of the elements you can use a **Main** tag to put your navigation in.
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
### Required elements for HTML

The declaration is not an HTML tag; it is an instruction to the web browser about what version of HTML the page is written in. When omitted, browsers tend to use a different rendering mode, the browser may decide to automatically go into Quirks or Strict Mode. In HTML5 this is the only doctype you'll need.

This is the first thing the browser looks for then it proceeds down
```html
<!DOCTYPE html>
```
Wraps the entire document
```html
<!DOCTYPE html>
<html>
</html>
```

Title
```html
<title>Look up at the top of the browser.</title>
```

Link tags
It's tandard to have stylesheets at the top for loading the styled page as quickly as possible
```html
<link rel="stylesheet" href="/css/style.css">
```

Script tags
To link to external javascript scripts. HTML reads top to bottom. It's standard to put these at the bottom of the document to increase the perceived load time of the page.
```html
<script type="text/javascript">

</script>
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
