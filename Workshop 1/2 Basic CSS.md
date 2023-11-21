Cascading Style Sheets
Adding styles to html elements

## Basic Syntax

```
Selector {
	property1: value;
	property2: value;
}
```

What can you style? There's a lot!
Check out the MDN Docs: https://developer.mozilla.org/en-US/docs/Web/CSS 

Selectors: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_selectors

## Importing CSS
- Inline
	- Style attribute in the html tag
	- ```<div style="color: red; text-decoration: underline;"></div>```
- Internal
	- Styles added in the head part of the html file
	- Example:
	```
	<head>
		<style>
		     h2{
	            text-decoration: underline;
	            font-weight: 500;
	            color: darkgreen;
	        }
	        p{
	            font-weight: bold;
	        }
	        .section{
	            background-color: lightgrey; border: 2px solid black;
	        }
	        #form{
	            background-color: lightcoral; border: 0px dotted black;
	        }
		 </style>
	</head>
	```

- External
	- Import styles from a .css file
	- Done in the head of the html file
	- ```<link rel="stylesheet" href="basic-HTML.css">``` 
## Specificity
Certain selectors take precedence over other selectors
Selectors:
- Element (h1, div) - 1
- Class (.thing, .thing2) - 10
- ID (#id1) - 100
- Inline - 1000
Website for specificity: https://specificity.keegan.st

## The Box Model
Every element is contained within a box
That box, has multiple parts:
- Content
	- The actual content of the element (ex. the text in a paragraph)
- Padding
	- Space between the content and the border
- Border
	- The border of the content
- Margin
	- Space between the element and other elements
Padding: https://developer.mozilla.org/en-US/docs/Web/CSS/padding
Border: https://developer.mozilla.org/en-US/docs/Web/CSS/border
Margin: https://developer.mozilla.org/en-US/docs/Web/CSS/margin

## Units (Absolute and Relative)
- Both used in font sizes, positioning, widths, and many more!
- Absolute
	- Units with set sizes
	- Common absolute units
		- **px (pixels)**
		- in (inches)
		- cm (centimeters)
- Relative
	- Size of the unit depends on other factors
	- Common relative units
		- em (font size of the element)
		- rem (font size of the root element)
		- vh (1% of the viewport's height)
		- vw (1% of the viewport's width)
	- Some stuff to know about relative units:
		- Root element
			- The ```<Html>``` tag in an html file
		- Viewport
			- The size of the screen
			- Depends on the device
			- Ex. Most laptops have a viewport of 1024px (width) by 837px (heigth) 
- Units and Values: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Values_and_Units


## Layout and Positioning
Absolute
- You set the position manually, it stays there no matter what
- Removed from normal document flow 
Relative
- Normal flow of the document (normal html positioning)
- Offset is set relative to itself
Sticky
- Relative up until a certain point
- Then it will "stick" with the screen
Positioning: https://developer.mozilla.org/en-US/docs/Web/CSS/position


## Typography (font and text properties)
Fonts
- You can get them from google fonts (cool website :3)
- Choose a font you like, pick the font weights, copy the provided code, and paste
- Then style the element with font-family:  "name of your font", sans-serif;

Example code that imports "Ubuntu" and its 8 styles and uses the font (only uses the bold and light styles)

```
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin
<link href="https://fonts.googleapis.com/css2?family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap" rel="stylesheet">

<style>
	body {
		font-family: 'Ubuntu', sans-serif;
	}
	.text::first-line{
		font-size: 20px;
		font-weight: bold;
		font-style: italic;
		line-height: 1.5;
		margin: 20px;
		}
	.text{
		font-size: 20px;
		font-weight: light;
		line-height: 1.5;
		margin: 20px;
		}
</style>
```

Text properties
- You can style text from the font to if they are italicized or underlined, and many more!
- Text-Decoration
	- This is a shorthand for multiple CSS properties
		- text-decoration-color (color of the line)
			- Check the color section of the notes :3
		- text-decoration-line (the type of line to be added)
			- none
			- underline
			- overline (line over the text)
			- line-through
		- text-decoration-style (style of the line)
			- solid
			- double
			- dotted
			- dashed
			- wavy
		- text-decoration-thickness (thickness of the line)
			- Use units
	- Used with one or more *<u>space-seperated</u>* values
	- example template: ```text-decoration: <line> <style> <color> <thickness>;```
		- The style doesn't have to follow the template (color can go first etc.)

References
- Fonts: https://developer.mozilla.org/en-US/docs/Web/CSS/font
- Text-Decoration: https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration
- Google Fonts: https://fonts.google.com
- Text-Transform: https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform


## Backgrounds and Borders
Backgrounds
- Color
	- Keyword ``` red, blue, gray, etc. ```
	- Rgb ``` rgb(value-red, value-green, value-blue) ```
		- Combination of Red, Green, and Blue colors 
		- Value goes from 0 - 255
	- Hex ``` #adc75a ```
		- Just use a color picker online XD
	- hsl ```hsl(0 80% 50% / 25%);```
		- Combination of Hue, Saturation, and Lightness
		- Once again, le color picker onlinee 
- Image
	- Url(image)
	- gradient
Borders
- Style
	- Dotted
	- Wavy
	- Solid
- Size
- Color
```
border: 5px double #32a1ce;
```

Borders: https://developer.mozilla.org/en-US/docs/Web/CSS/border
Backgrounds: https://developer.mozilla.org/en-US/docs/Web/CSS/background
