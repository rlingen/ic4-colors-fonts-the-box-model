# ICA Fonts, Sizing, Backgrounds Positioning
This In-Class Activity will take you through the basics of writing CSS and some of the elementary the different ways to style your HTML elements. The specific instructions for the Activity will be listed at the end of this README.

---

## CSS
CSS, or Cascading Style Sheets, is a fundamental technology in web development. Its primary purpose is to separate the structure and content of a webpage from its presentation. By using CSS, developers can control the visual styling of HTML elements, such as fonts, colors, spacing, and layout. This separation enhances maintainability and allows for consistent styling across a website.

In CSS, rules are created to apply styles to HTML elements. A CSS rule consists of a selector, which targets an HTML element, and a declaration block containing one or more declarations. Declarations consist of properties and values.

```css
selector {
  property: value;
}
```
The Selector is the HTML element that you want to style. The Property is the type of style you want to apply to the element. The Value is the value of the property you want to apply to the element. Selectors can be designated by addressing the specific `element`, the `.class`, the `#id`, or `*` (all elements).

CSS can be written in three ways:
  - Inline → directly in the HTML element as a style attribute
  ```html
    <p style="color: red;">all of this text is red.</p>
  ```
  ```
  - Internal → contained with the <html></html> tags of the document
  ```html
    <body>
      <style>
        p {
          font-size: 16px;
        }
      </style>
      <p>all of this text has font size 16px.</p>
    </body>
  ```
  ```
  - External → contained in a separate file, and linked to the HTML document
  ```css
    p {
      font-size: 16px;
    }
  ```
  ```html
    <head>
      <link rel="stylesheet" href="style.css">
    </head>
    <body>
      <p>all of this text has font size 16px.</p>
    </body>
  ```
> [!TIP]
> It's important to understand the difference between the three ways of writing CSS. Inline CSS is the least preferred method, as it is the least maintainable. Internal CSS is situational. External CSS is the preferred method, as it is the most maintainable and allows for the most flexibility.

---

## Colors in CSS
Colors are useful for styling your HTML elements. There are a number of different ways to specify colors in CSS. Colors are specified using predefined color names, or RGB, HEX, HSL values. RGB and HSL can be specified with or without alpha channel (% of transparency).
  - predefined color names:
    - `red`
    - `green`
    - `blue`
    - `salmon`
    - `cyan`
    - ...
    - `gray`
    - `lightgray`
  - HEX values:
    - `#rrggbb`
  - RGB values:
    - `rgb(red, green, blue)`
    - (where red, green, and blue are integers between 0 and 255)
  - HSL values:
    - `hsl(hue, saturation, lightness)` 
    - (where hue is a degree on the color wheel (from 0 to 360), saturation is a percentage value (0% being a shade of gray and 100% the full color), and lightness is also a percentage value (0% is black, 100% is white))
RGB and HSL values can be specified with or without alpha channel (% of transparency). 
---

## Text
Text can be styled in a number of different ways. This activity will cover the following text properties:
  - `color` → used to set the color of the text. The color can be specified by the rules set in the Colors section above.
    - ```css
        p {
          color: red;
        }
      ```
    - ```html
        <p color: rgb(255,0,0);>This is a paragraph.</p>
      ```
  - `text-align` → used to set the horizontal alignment of a text, within it's parent element. Justified means that the text is aligned to both the left and right margins.
    - left
    - center
    - right
    - justify
    - ```css
        h1 {
          text-align: center;
        }
        h3 {
          text-align: right;
        }
      ```
  - `text-decoration` → used to set or remove decorations from text.
    - none
    - underline
    - overline
    - line-through
    - blink
    - ```css
        .text-underline {
          text-decoration: underline;
        }
      ```
  - `text-transform` → used to specify uppercase and lowercase letters in a text.
    - none
    - capitalize
    - uppercase
    - lowercase
    - ```css
        .uppercased-div {
          text-transform: uppercase;
        }
      ```

  - font-family
  - font-size
  - line-height
  - font-style
  - font-weight


### color
The `color` property is used to set the color of the text. The color can be specified by the rules set in the Colors section above.
```css
p {
  color: red;
}
```
```html
<p color: rgb(255,0,0);>This is a paragraph.</p>
```

### text-align
The text-align property is used to set the horizontal alignment of a text, within it's parent element.
  - left
  - center
  - right
  - justify
```css
h1 {
  text-align: center;
}
h3 {
  text-align: right;
}
```

### text-decoration
The text-decoration property is used to set or remove decorations from text.
  - none
  - underline
  - overline
  - line-through
  - blink
```css
.text-underline {
  text-decoration: underline;
}
```

### text-transform
The text-transform property is used to specify uppercase and lowercase letters in a text.
  - none
  - capitalize
  - uppercase
  - lowercase
```css
.uppercased-div {
  text-transform: uppercase;
}
```

## Fonts
In CSS there are five generic font families:
  - Serif 				    → have a small stroke/curve at the edges of each letter.
  - Sans-serif 			  → fonts have clean lines (no small strokes attached).
  - Monospace fonts 	→ all the letters have the same fixed width. 
  - Cursive 				  → imitate human handwriting.
  - Fantasy 				  →  are decorative/playful fonts.
All the different font names belong to one of the generic font families.
### Sans vs. Sans-serif
Sans-serif fonts are fonts which don't have the small strokes at the end of each character. The word "sans" means "without" in French. Sans-serif fonts is normally used for shorter texts (e.g. headlines or captions), as it's the preferred, more readable format on webpages.

### font-family
The font-family property is used to specify the font to be used for an element.
```css
p {
  font-family: "Times New Roman", Times, serif;
}
h2 {
  font-family: Arial, Helvetica, sans-serif;
}
```
### font-size
The font-size property is used to specify the size of the font.
```css
p {
  font-size: 20px;
}
```
### line-height
The line-height property is used to specify the space between lines.
```css
p {
  line-height: 1.5;
}
```

### font-style
The font-style property is used to specify whether the font should be italic, oblique, or normal.
  - normal
  - italic
  - oblique
```css
p {
  font-style: italic;
}
```

### font-weight
The font-weight property is used to specify how thick or thin characters in a text should be displayed.
  - normal
  - bold
  - bolder
  - lighter
  - 100
  - 200
  - ...
  - 900
```css
p {
  font-weight: bold;
}
```

## Sizing
Elements can be sized using a number of different number representations.
  - px (exact pixel count)

### width
The width property is used to specify the width of an element.
```css
div {
  width: 300px;
}
```
### height
The height property is used to specify the height of an element.
```css
div {
  height: 300px;
}
```
### max-width
The max-width property is used to set the maximum width of an element.
```css
div {
  max-width: 500px;
}
```
### max-height
The max-height property is used to set the maximum height of an element.
```css
div {
  max-height: 500px;
}
```
### min-width
The min-width property is used to set the minimum width of an element.
```css
div {
  min-width: 300px;
}
```
