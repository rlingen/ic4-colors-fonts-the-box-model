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

## Text and Fonts

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


