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
Inline
Internal
External

## Specificity
Certain selectors take precedence over other selectors
Selectors:
- Element (h1, div) - 1
- Class (.thing, .thing2) - 10
- ID (#id1) - 100
- Inline - 1000
Check this website out: https://specificity.keegan.st

## The Box Model
Every element is contained within a box
That box, has multiple parts:
- Content
- Padding
- Border
- Margin
Padding: https://developer.mozilla.org/en-US/docs/Web/CSS/padding
Border: https://developer.mozilla.org/en-US/docs/Web/CSS/border
Margin: https://developer.mozilla.org/en-US/docs/Web/CSS/margin

## Units (Absolute and Relative)
Both used in font sizes, positioning, widths, and many more!
Units and Values: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Values_and_Units


## Layout and Positioning
Absolute
- You set the position manually, it stays there no matter what
Relative
- Normal flow of the document (normal html positioning)
Sticky
- Relative up until a certain point
- Then it will "stick" with the screen
Positioning: https://developer.mozilla.org/en-US/docs/Web/CSS/position


## Typography (font and text properties)
Fonts
- You can get them from google fonts (cool website :3)
- Choose a font you like, pick the font weights, copy the provided code, and paste
- Then style the element with font-family:  "name of your font", sans-serif;

Fonts: https://developer.mozilla.org/en-US/docs/Web/CSS/font
Text-Decoration: https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration
Google Fonts: https://fonts.google.com
Text-Transform: https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform


## Backgrounds and Borders
Backgrounds
- Color
	- Keyword
	- Rgb
	- Hex
	- hsl
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
