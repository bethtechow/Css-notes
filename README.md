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

