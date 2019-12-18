[Home](https://zx37.github.io/learning-journal/)

# CSS Basics and Color

## Intro to CSS

CSS (Cascading Style Sheets) is a styling language used to apply in-depth visual designs to HTML code. CSS uses a straightforward syntax, with only 3 primary elements. A **selector** is used to determine which HTML element or elements the style will be applied to. Within the selector, **properties** determine what about the elements will be styled. Each property is given a **value**, which determines how that property is styled.

```css
h1 {
    color: #FF0000;
}
```

The above example shows a selector (h1) having its color property (color) set to a red hex value (#FF0000).

## Class, Id, Combined, and Virtual Selectors

There are 3 primary methods of selecting HTML elements. Within HTML, elements can be given a **class** (generic, generally multi-use) and/or **id** (specific, generally single-use). CSS selectors can target elements with a specific class or id, or target all elements of a certain type.

A non-prefixed selector (`h1 {}`) will select any elements of that type. Prefixing with a period (`.button`) will select any elements with that class, and prefixing with a hash (`#topmenu`) will select elements with that id.

Elements can be selected in more complex ways as well. You can select multiple sets of elements using a comma (`h1, .title`). Children of elements can be selected with a space (`ul li` or `ul *`), or with a right caret to select only only direct children (`ul>p`).

Virtual selectors are used to style elements with a certain manually or automatically defined state. This can include elements that have been clicked, that are hovered over, or that are "active".

## Color

One of the most basic and most impactful functionalities of CSS is manipulation of color in your design. Simple changes in color can impact the emotional impact and visual clarity of your content more than nearly anything else. Color can be applied to anything on the page - primarity fonts, backgrounds, and borders.

Color is usually set in CSS in one of 4 ways.

- **RGB** sets color by mixing the three primary colors (Red, Green, and Blue). The standard format (`rgb(123,123,123)`) sets how much of each color is represented, between 0-255 (allowing for 16,777,216 different colors). RGB can also have a 4th value appended for opacity, which creates an RGBA syntax (`rgba(123,123,123,.3)`).

- **Hexcodes** function the same way as RGB colors, but with a more space-efficient format. Using hexadecimal notation instead of decimal (going from 0-F), as well as using shorter syntax, hexcodes can express an color in around half the space as an rgb value. The standard format (`#FD036C`) expresses red, green, and blue values in 2 characters each, from 00 (0) to FF (256). If each color is expressed with 2 repeating characters, as is common with grays (`#DDDDDD`) or pure colors (`#FF0000`), the value can be shortened to 3 characters (`#DDD` or `#F00`).

- **HSL** looks similar in syntax to RGB, but expresses color much differently. The first value given assings a color based on position on a color wheel (sensibly ranged between 0-360). The second value provides the 0-100% saturation of that color, and the third provides it a 0-100% lightness (should be called "darkness"). HSL uses the syntax `hsl(270,30%,50%), and creates a range of 3,600,000 colors, covering a somewhat different color space than rgb.

- **Color Names** uses shorthand aliases to set basic rgb colors. They remain limited to the basics but are easy to use as placeholder or test values.