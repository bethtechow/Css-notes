# Css-notes
p {
	color: red;
}

span {
	color:blue;
}

p {
    font-size: 100px;
}

span {
	font-family: cursive;

}

<--put css in html file -->
<!DOCTYPE html>
<html>
	<head>
		<style>
			p {
				color: purple;
			}
		</style>
		<title>Result</title>
	</head>
	<body>
		<p>Check it out! I'm purple!</p>
	</body>
</html>

<-- or link html file to css -->
<!DOCTYPE html>
<html>
	<head>
	    <link type="text/css" rel="stylesheet" href="stylesheet.css"/>
		<title>Result</title>
		</link>
	</head>
	<body>
		<p>I want to be SIZE 44 font!</p>
	</body>
</html>

<-- Link tags are self closing like img  thus <link type="??"/>

more info cssis diff than html
selector {
    property: value;
}
example is
p {
    color: red;
}

/*You can do this! Write your CSS below.*/
h3 {
    color: red;
}
p {
    font-family: Courier;
}
span {
    background-color: yellow;
    {
comments in css look like this
/*I'm a comment!*/

link for hyml to css goes inside head <link type="text/css" rel="stylesheet" href="stylesheet.css"/>

fun colors
Search for "hex color palette" or "hex color picker" with your favorite web browser to find a bunch of options!

Hex values always start with a pound sign (#), are up to six "digits" long, and are case-insensitive: that is, they don't care about capitalization. #FFC125 and #ffc125 are the same color.

ems like px but change with size of screen
he font-size unit em is a relative measure: one em is equal to the default font size on whatever screen the user is using. That makes it great for smartphone screens, since it doesn't try to tell the smartphone exactly how big to make a font: it just says, "Hey, 1em is the font size that you normally use, so 2em is twice as big and 0.5em is half that size!"

h1 {
    font-family: serif;
    }
h2 {
    font-family: sans-serif;
    }
h3 {
    font-family: cursive;
    }

style blocks in css example

/*Add your CSS below!*/
div {
    background-color: #cc0000;
    height: 100px;
    width: 100px;
}

<!DOCTYPE html>
<html>
	<head>
	<link type="text/css" rel="stylesheet" href="stylesheet.css"/>
		<title>Result</title>
	</head>
	<body>
		<div></div>
	</body>
</html>

/*Add your CSS below!*/
td {
    height: 50px;
    border: 1px dashed blue;
}
table {
    border: 1px solid black;
}

<!DOCTYPE html>
<html>
	<head>
		<link type="text/css" rel="stylesheet" href="stylesheet.css"/>
		<title></title>
	</head>
	<body>
		<table>
			<thead>
				<th colspan="3">Nine Blocks!</th>
			</thead>
			<tbody>
				<tr>
					<td></td>
					<td></td>
					<td></td>
				</tr>
				<tr>
					<td></td>
					<td></td>
					<td></td>
				</tr>
				<tr>
					<td></td>
					<td></td>
					<td></td>
				</tr>
			</tbody>
		</table>
	</body>
</html>
<!DOCTYPE html>
<html>
	<head>
		<link type="text/css" rel="stylesheet" href="stylesheet.css"/>
		<title>About Me</title>
	</head>
	<body>
		<img src="https://s3.amazonaws.com/codecademy-blog/assets/46838757.png"/>
		<p>We're Codecademy! We're here to help you learn to code.</p><br/><br/>
		<div>
		<a href="http://www.google.com">Click this <span>BUTTON</span></a>
		</div>
	</body>
</html>
img {
	display: block;
	height: 100px;
	width: 300px;
	margin: auto;
}

p {
	text-align: center;
	font-family: Garamond, serif;
	font-size: 18px;
}

/*Start adding your CSS below!*/
div {
    Height: 50px;
    width: 120px;
    border-color: #6495ED;
    background-color: #BCD2EE;
    Border-radius: 5px;
    margin: auto;
    text-align: center;
}
a {
    text-decoration: none;
    font-family: Arial;
   }

span {
    font-family: Cursive;
}

Remember, you can reach an element that is a child of another element like this:

div div p { /* Some CSS */ }
where in this case, we'd be grabbing any <p> that is nested somewhere inside a <div> that is nested somewhere inside another <div>. If you want to grab direct children—that is, an element that is directly nested inside another element, with no elements in between—you can use the > symbol, like so:

div > p { /* Some CSS */ }
This only grabs <p>s that are nested directly inside of <div>s; it won't grab any paragraphs that are, say, nested inside lists that are in turn nested inside <div>s.

html file
<!DOCTYPE html>
<html>
	<head>
		<link type="text/css" rel="stylesheet" href="stylesheet.css"/>
		<title>Ultimate Text Challenge</title>
	</head>
	<body>
		<p>Introduction: Cascading with CSS</p>
		<div>
			<p>Synopsis: When you set a property of a selector like 'p' to a certain value, that value applies to <em>all</em> p tags.
			If, however, you change that same property to a different value for a more specific instance of p,
			that change will <em>override</em> the 'general rule'.
			</p>
			<ul>
				<li><p>If you say p { font-family: Garamond}, all 'p's will have the font Garamond.</p></li>
				<li><p>BUT if you say li p {font-family: Verdana}, 'p's outside of 'li's will be
					   in Garamond, and 'p's INSIDE 'li's will be in Verdana.
				</p></li>
				<li><p>The more specific your selectors are, the higher importance CSS gives to the styling you apply!</p></li>
			</ul>
		</div>
		<p>Summary: Greater specificity makes CSS prioritize that particular styling.</p>
	</body>
</html>
now css connected to that file

/*Add your CSS below!*/
p {
    font-family: garamond;
}
p {
    font-weight: bold;
}
body > div > p {
    color: #7AC5CD;
}
li p {
    color: #000000; text-decoration:underline;
}

text on classes 
Classes are assigned to HTML elements with the word class and an equals sign, like so:

<div class="square"></div>
<img class="square"/>
<td class="square"></td>
Classes are identified in CSS with a dot (.), like so:

.square {
    height: 100px;
    width: 100px;
}
This allows you to take elements of different types and give them the same styling.

text on IDs
ID, please!
IDs, on the other hand, are great for when you have exactly one element that should receive a certain kind of styling.

IDs are assigned to HTML elements with the word id and an equals sign:

<div id="first"></div>
<div id="second"></div>
<p id="intro"></p>
IDs are identified in CSS with a pound sign (#):

#first {
    height: 50px;
}

#second {
    height: 100px;
}

#intro {
    color: #FF0000;
}
This allows you to apply style to a single instance of a selector, rather than all instances.

text on pseudo class selectors
You've learned about class selectors. Now it's time to learn about pseudo-class selectors.

A pseudo-class selector is a way of accessing HTML items that aren't part of the document tree (remember the tree structure we talked about earlier?). For instance, it's very easy to see where a link is in the tree. But where would you find information about whether a link had been clicked on or not? It isn't there!

Pseudo-class selectors let us style these kinds of changes in our HTML document. For example, we saw we could change a link's text-decoration property to make it something other than blue and underlined. Using pseudo selectors, you can control the appearance of unvisited and visited links—even links the user is hovering over but hasn't clicked!

The CSS syntax for pseudo selectors is

selector:pseudo-class_selector {
    property: value;
}
It's just that little extra colon (:).

how to change color if you hover over a link
css page
a:hover {
	color: #cc0000;
	font-weight: bold;
	text-decoration: none;
}

a:link {
    text-decoration: none; color: #008B45;
}
a:hover {
    color: #00FF00;
}
a:visited {
    color: #EE9A00
}
First child
Another useful pseudo-class selector is first-child. It's used to apply styling to only the elements that are the first children of their parents. For instance:

p:first-child {
    color: red;
}
Would make all paragraphs that are the first children of their parent elements red.

Nth child
Well done! You can actually select any child of an element after the first child with the pseudo-class selector nth-child; you just add the child's number in parentheses after the pseudo-class selector. For example,

p:nth-child(2) {
    color: red;
}
Would turn every paragraph that is the second child of its parent element red.

The element that is the child goes before :nth-child; its parent element is the element that contains it.

<!DOCTYPE html>
<html>
	<head>
		<link type="text/css" rel="stylesheet" href="stylesheet.css"/>
		<title></title>
	</head>
	<body>
		<div>
			<p>I'm the first child!</p>
			<p>We're not.</p>
			<p>We're not.</p>
			<p>We're not.</p>
			<p>We're not.</p>
			<p>We're not.</p>
			<p>We're not.</p>			
		</div>
	</body>
</html>

/*Add your CSS below!*/
p:first-child {
    font-family: cursive;
}
p:nth-child(2) {
    font-family: Tahoma;
}
p:nth-child(3) {
    color: #CC0000;
}
p:nth-child(4) {
    background-color: #00FF00;
}
p:nth-child(5) {
    font-size: 22px;
}

