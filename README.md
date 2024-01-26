# ICA Fonts, Sizing, Backgrounds Positioning
This In-Class Activity will take you through the basics of writing CSS and some of the elementary the different ways to style your HTML elements. The specific instructions for the Activity will be listed first in this README, with the full guide of CSS following.

---

## ICA Instructions
  1. create 3 heading elements of the same type with different text sizes, using different sizing techniques
  2. create 3 heading elements of the same type with different colors, using different coloring techniques
  3. create 1 paragraph, 1 quote, and 1 blockquote element that have different font families font font stylings
  4. create 5 div tags, each of which are classed uniquely, and are sized using three different sizing techniques
  5. now for each of these div tags, color them uniquely
  6. create 3 div tags, each of which are classed uniquely, and give them three unique border styles (width, color, radii)
  7. recreate the image of the CSS box model using three embedded div tags
  8. Create a new page titled positioning.html. Add in the appropriate boilerplate with a link to ica4.css
  9. Create a container div of type `.position-practice`
  10. Create 5 divs inside of the container div, each of which are classed uniquely. These divs should represent each positioning technique with different styles

> [!TIP]
> CSS is a very powerful tool, but the learning curve can be extrememly steep. It's important to have a solid foundational understanding of the core properities used in CSS. Try mixing things up as you go along with the Activity instructions. Try to use different sizing techniques, different colors, different fonts, etc. to get a feel for how CSS works; the more you stretch your understanding of CSS, the easier it will be to learn more advanced techniques.

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
  ```css
    p {
      color: red;
    }
  ```
   ```html
    <p color: rgb(255,0,0);>This is a paragraph.</p>
  ```
  - `text-align` → used to set the horizontal alignment of a text, within it's parent element. Justified means that the text is aligned to both the left and right margins.
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
  - `text-decoration` → used to set or remove decorations from text.
    - none
    - underline
    - overline
    - line-through
  ```css
    .text-underline {
      text-decoration: underline;
    }
  ```
  - `text-transform` → used to specify uppercase and lowercase letters in a text.
    - none
    - capitalize
    - uppercase
    - lowercase
  ```css
    .uppercased-div {
      text-transform: uppercase;
    }
  ```
 
 ---
## Fonts
In CSS there are five generic font families:
  - Serif 				    → have a small stroke/curve at the edges of each letter.
  - Sans-serif 			  → fonts have clean lines (no small strokes attached).
  - Monospace fonts 	→ all the letters have the same fixed width. 
  - Cursive 				  → imitate human handwriting.
  - Fantasy 				  →  are decorative/playful fonts.

All the different font names belong to one of the generic font families. It's important to understand the difference between the different font families, as they are used for different purposes.

> [!TIP]
> Sans vs. Sans-serif
> Sans-serif fonts are fonts which don't have the small strokes at the end of each character. The word "sans" means "without" in French. Sans-serif fonts is normally used for shorter texts (e.g. headlines or captions), as it's the preferred, more readable format on webpages.
 
This activity will cover the following font properties:
  - `font-family` → used to specify the font to be used for an element.
  ```css
    p {
      font-family: "Times New Roman", Times, serif;
    }
  ```
  Here, the browser will first attempt to use the font "Times New Roman". If it's not available, it will attempt to use the font "Times", and the same pattern for using the generic font family serif.
  - `font-size` → used to specify the size of the font.
  ```css
    p {
      font-size: 20px;
    }
  ```
  Font size can only be specified in px (pixels), em (relative to the font-size of the element), or rem (relative to the font-size of the root element).
  - `line-height` → used to specify the space between lines.
  ```css
    p {
      line-height: 1.5;
    }
  ```
  Line height can be points, pixels, ems, and rems.
  - `font-style` → used to specify the degree of italicization of a font.
    - normal
    - italic
    - oblique
  ```css
    p {
      font-style: italic;
    }
  ```
  - `font-weight` → used to specify how thick or thin characters in a text should be displayed.
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

---
## Sizing
Elements can be sized using a number of different number representations.
  - auto, the browser calculates the size
  - pixel, exact pixel count (`px`)
  - point, 1/72 of an inch (`pt`)
  - element measure, relative to the font-size of the element (`em`)
  - root element measure, relative to the font-size of the root element (`rem`)
  - percentage, relative to the parent element (`%`)
  - viewport height & width, relative to 1% the viewport (`vh`, `vw`, `vmin`, `vmax`)

This activity will cover the following sizing properties:
  - `width`, `max-width`, `min-width` → defines the width of an element, or the minimum/maximum width of an element.
  ```css
    div {
      width: auto;
      max-width: 500px;
    }
  ```
  - `height`, `max-height`, `min-height` → defines the height of an element, or the minimum/maximum height of an element.
  ```css
    div {
      height: 30%;
      min-height: 50px;
    }
  ```
  - `aspect-ratio` → defines the aspect ratio of an element. This is used most often for images and videos, and should be used in conjunction with `width` or `height` being set as a dynamic number.
  ```css
    div {
      aspect-ratio: 16 / 9;
    }
  ```
  - `margin` → defines the space between the border of an element and its neighboring elements.
  ```css
    div {
      margin: 10px;
    }
  ```
  - `padding` → defines the space between the border of an element and its content.
  ```css
    div {
      padding: 10px;
    }
  ```
    
---
## Borders
Elements can be styled with borders. Borders can be styled with a number of different properties.
  - `border-style` → defines the style of the border.
    - There are many different preset styles of borders, some of which are: none, dotted, dashed, solid, ridge, inset, outset.
  ```css
    div {
      border-style: solid;
    }
  ```
  - `border-width` → defines the width of the border.
    - can be defined by description: thin, medium, thick
    - or px
  ```css
    div {
      border-width: 5px;
    }
  ```
  - `border-color` → defines the color of the border. Same color rules apply as in the Colors section above.
  ```css
    div {
      border-color: red;
    }
  ```
  - `border-radius` → defines the radius (degree of curvature) of the border.
  ```css
    div {
      border-radius: 5px;
    }
  ```

While it's imporant to know all the individual styling properties for borders, a much more common way is the short-hand form of just declaring the `border` property:
```css
  div {
    border: size style color;
  }
```
---
## The Box Model
The CSS box model is a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below shows the box model:

![The CSS Box Model](https://miro.medium.com/v2/resize:fit:424/1*lBtbo05WfLoc_mBLDQfqkw.png)

> [!IMPORTANT]
> The box model is one of the most key nuances of CSS to understand, as it is the basis for all layout in Web Dev. The box model is the reason why you can't set the width of an element to 100% and have it fill the entire width of the page. Make sure you have this down!
---
## Backgrounds
Background colors and images are the core concept of visual connection in Web Development. Backgrounds can be styled with a number of different properties.
  - `background-color` → defines the color of the background. Same color rules apply as in the Colors section above.
  ```css
    div {
      background-color: red;
    }
  ```
    - background colors can be set to be `transparent`, which will allow the background color of the parent element to show through.
    - you can also set the background color to a `linear-gradient`, which will create a gradient of colors. The gradient direction can be set by specifying the direction of the gradient, with `to direction` or an angle (like `90deg`).
  ```css
    div {
      background-color: linear-gradient(to right, red, blue);
    }
  ```
  - `background-image` → defines the image to be used as the background. The image can be a URL to an image, or a local file path.
  ```css
    div {
      background-image: url("url/to/image.png");
    }
  ```
  - `background-repeat` → defines how the background image should be repeated.
    - repeat (the background image is repeated both vertically and horizontally)
    - repeat-x
    - repeat-y
    - no-repeat
  ```css
    div {
      background-repeat: no-repeat;
    }
  ```
  - `background-position` → defines the position of the background image.
    - specified by two values: horizontal and vertical position. if only one value is specified, the other value will be set to center. Possible values are: 
    - top 
    - bottom
    - left
    - right
    - center
  ```css
    div {
      background-position: center center;
    }
  ```
  - `background-attachment` → defines whether the background image should scroll or be fixed.
    - scroll
    - fixed
  ```css
    div {
      background-attachment: fixed;
    }
  ```
  - `background-size` → defines the size of the background image.
    - auto
    - cover
    - contain
  ```css
    div {
      background-size: cover;
    }
  ```
---
## Positioning
Positioning is the most important aspect of CSS. Positioning is what allows you to layout your HTML elements in a specific way. There are five different positioning techniques:
  - Static
  - Relative
  - Absolute
  - Fixed
  - Sticky
The most common are Static, Relative, and Absolute. Fixed and Sticky are used less often, but are still important to know.

### How to Position
To position an element, you must first set the `position` property of the element. Then, you can use the `top`, `bottom`, `left`, and `right` properties to specify where you want the element to be positioned. The `top` and `bottom` properties specify the vertical position, and the `left` and `right` properties specify the horizontal position.
  - left: 20px; → the element is positioned 20px from the left edge of the browser window
  - right: 30em; → the element is positioned 30em from the right edge of the browser window
  - top: 50%; → the element is positioned 50% of the height of the browser window
  - bottom: 10vh → the element is positioned 10% of the viewport height from the bottom of the browser window
```css
  div {
    position: relative;
    top: 30px;
    left: 50px;
  }
```

### Static
Static positioning is the default positioning of an element. It is always positioned according to the normal flow of the page. Static positioned elements are not affected by the top, bottom, left, and right properties.

### Relative
Relative positioning is the positioning of an element relative to its normal position. Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.

### Absolute
Absolute positioning is the positioning of an element relative to its parent element. The element is positioned relative to its first positioned (not static) ancestor element. If there is no such ancestor, it is positioned relative to the document body. Absolutely positioned elements can have margins, and they do not affect the position of other elements.

### Fixed
Fixed positioning is the positioning of an element relative to the browser window. The element is removed from the normal document flow, and no space is created for the element in the page layout. It is positioned relative to the screen's viewport and doesn't move when scrolled.

### Sticky
Sticky positioning is a hybrid of relative and fixed positioning. The element is treated as relative positioned until it crosses a specified threshold, at which point it is treated as fixed positioned.

> [!TIP]
> Fixed and Sticky positioning are often used primarily for navigation bars, as they allow the navigation bar to stay in the same position on the page, even when the user scrolls. This will be a handy technique to know for styling pages on a larger scale.


