# ic4-fonts-sizing-backgrounds-positiong

## Colors
Colors are specified using predefined color names, or RGB, HEX, HSL values. RGB and HSL can be specified with or without alpha channel (% of transparency).
  - predefined color names:
    - red
    - green
    - blue
    - salmon
    - cyan
    - ...
    - gray
    - lightgray
  - RGB values:
    - rgb(red, green, blue)
  - HEX values:
    - #rrggbb
  - HSL values:
    - hsl(hue, saturation, lightness)

## Text

### color
The color property is used to set the color of the text. The color is specified by:
  - predefined color names
  - RGB values
  - HEX values
  - HSL values

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
