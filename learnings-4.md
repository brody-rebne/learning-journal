[Home](https://zx37.github.io/learning-journal/)

# HTML Basics and Structure

**HTML Basics**

HTML is a markup language made ubiquitous by its role as the provider of raw content for every webpage and webapp in the modern world. It is a very structured language, concerned less with the details, appearance, and functionality of a page's content, and more with its core definitions and hierarchical relationships.

HTML creates a relatively blank canvas, providing only the necessary structural definitions of content, allowing its companion languages CSS and JavaScript to focus on the styling and functionality of the content respectively.

---

**Structure Within HTML**

HTML follows a straightforward set of defaults in order to structure itself if it for any reason lacks CSS styling. Every element is treated like a rectangular block, except for some inline elements used for things like italic text or images. Each block is placed beneath the one written above it in the source code, and aligned to the left. Elements like headers, anchors, and unordered lists are provided with some basic styling as well, although this hardly interferes with the elements' structure.

---

**Structuring With CSS**

There are a few basic CSS selectors that provide the basic structuring of HTML elements on any webpage or app. These include:

- `positioning`, which determines how the elements flow together on the page, as well as how they are placed within the page.
- `float`, which determines to which side elements are by default  shifted to.
- `z-index`, which determines how elements are stacked on top eachother, similar to how layers are used in design tools.

There are many more tools beyond these for manipulating HTML elements in CSS, including the box model which is used to control the more subtle positionings of elements.

---

**Layouts**

There are two general philosophies for laying out pages, each with benefits and downsides.

The first, known as the Liquid layout, is a responsive layout build to maximize its width within whatever window size is available. It allows for a theoretically much higher information density, but can be excessively wide without a reasonable `max-width`. Generally liquid layouts size items by %, and set a `max-width` in px.

The second, the Fixed layout, is a more predictable and straightforward layout which sizes items by a set %. The fixed layout can be restrictive, but it allows the designer to align everything on the page to a grid, creating a pleasant and consistent framework to display content in. However, fixed layouts often need to use more complicated methods to be as responsive as a simple liquid layout.