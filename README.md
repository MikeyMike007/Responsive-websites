# HTML and CSS Notes

## HTML tags

| Tag                              | Description                      |
| -------------------------------- | -------------------------------- |
| `<DOCTYPE html>`                 |                                  |
| `<html>`                         |                                  |
| `<head>`                         |                                  |
| `<body>`                         |                                  |
| `<title>`                        |                                  |
| `<header>`                       |                                  |
| `<h1>`                           |                                  |
| `<h2>`                           |                                  |
| `<h3>`                           |                                  |
| `<h4>`                           |                                  |
| `<h5>`                           |                                  |
| `<h6>`                           |                                  |
| `<nav>`                          |                                  |
| `<a href="mypage.html">Link</a>` |                                  |
| `<article>`                      |                                  |
| `<img src="image.jpg"/>`         |                                  |
| `<p>`                            |                                  |
| `<strong>`                       |                                  |
| `<b>`                            |                                  |
| `<em>`                           |                                  |
| `<ol>`                           | Numbered list                    |
| `<ul>`                           | Bullet list                      |
| `<li>`                           | Bullet (inside `<ul>` or `<ol>`) |
| `<footer>`                       |                                  |
| `<aside>`                        |                                  |
| `<button>`                       |                                  |
| `<h1 style="color: blue">`       |                                  |
| `<style>`                        | Css                              |
| `footer`                         |                                  |

## CSS tags

| Tag                          | Description                                                                  |
| ---------------------------- | ---------------------------------------------------------------------------- |
| `font-size`                  | Size of font e.g. 20px                                                       |
| `font-family`                | Font e.g. `sans-serif`                                                       |
| `text-transform`             | Lowercase, Uppercase etc.                                                    |
| `font-style`                 | Italic, bold, etc                                                            |
| `text-align`                 | Left, center, right, etc                                                     |
| `line-height`                | Spacing between lines e.g for `<p>`                                          |
| `list-style`                 | Square, circle, number                                                       |
| `background-color`           | Background color for area                                                    |
| `border`                     | Border                                                                       |
| `border-top`                 | Top border                                                                   |
| `border-bottom`              | Bottom border                                                                |
| `border: 5px solid black`    | 5px solid black border                                                       |
| `* {}`                       | Whole document                                                               |
| `body {}`                    | Whole body tag                                                               |
| `margin`                     | Sets the margin area on all four sides of an element                         |
| `margin: 1px 2px`            | vertical-horizontal margin                                                   |
| `margin: 1px 2px 3px`        | top-horizontal-bottom margin                                                 |
| `margin: 1px 2px 3px 4px`    | top-right-botton-left margin                                                 |
| `margin-bottom: 1px`         | Botton margin                                                                |
| `margin-left: 1px`           | Left margin                                                                  |
| `margin-top: 1px`            | Top margin                                                                   |
| `margin-right: 1px`          | Right margin                                                                 |
| `text-align:`                | Alignement of text                                                           |
| `text-transform:`            | E.g. `uppercase` or `lowercase`                                              |
| `padding:`                   | Sets the padding area for all four sides of an element                       |
| `font-weight:`               | E.g. `bold`                                                                  |
| `text-decoration`            | E.g. `underline`, `none`. Used with links                                    |
| `cursor:`                    | Sets the mouse cursor at hoover                                              |
| `<a hre... class="x">x</a>`  | Please see below - Css and links                                             |
| `.x:hover {}`                | Style at hoover in class `x`                                                 |
| `.x:active {}`               | Style at link click                                                          |
| `.x:link {}`                 | Link style                                                                   |
| `.x:visited {}`              | Link style when visited                                                      |
| `<ul class="list">`          | See blow for styling                                                         |
| `.list{list-style: square;}` | Squared bullets in list                                                      |
| `.list li {}`                | Styling of each bullet e.g. `margin-left:`                                   |
| `if <p id="test">`           | Use then `#test {}`                                                          |
| `if <p>`                     | Use then `p {}`                                                              |
| `if <p class="test">`        | Use then `.test{}`                                                           |
| `position:`                  | E.g. `absolute`, `relative`                                                  |
| `.x{position: relative}`     | Offset relative to itself with (see: position below)                         |
| `.x{position: absolute}`     | Removed from normal flow of document (see: position below)                   |
| `width`                      | Sets an elements width                                                       |
| `li:first-child {}`          | First bullet                                                                 |
| `li:last-child {}`           | Last bullet                                                                  |
| `li:nth-child(even)`         | Even numbered bullets                                                        |
| `display:`                   | E.g. `inline`, `inline-block`, `block`. (See:display)                        |
| `a:link {}`                  | Style for links in `<a>` tags                                                |
| `a:hover {}`                 | Style for links in `<a>` when hoovered                                       |
| `a:active {}`                | Style for links in `<a>` when clicked                                        |
| `nav a:link {}`              | Style for links in `<a>` which itself is in a `<nav>` tag                    |
| `nav a:link:last-child {}`   | Last link in `<a>` -> `<navb>`                                               |
| `button {}`                  | Design for a `<button>` tag.                                                 |
| `h3 + p {}`                  | Style the `<p>` directly after `h3` (see: + operator)                        |
| `h3 + p::first-line {}`      | Style the first line of the paragraph which lies after `<h3>`                |
| `h1::first-letter {}`        | Style the first letter in `<h1>`                                             |
| `element::after {}`          | See ::after and ::before                                                     |
| `element::before {}`         | See `::after` and `::before`                                                 |
| `float:`                     | Let the element float e.g. `float: left;`                                    |
| `clear:`                     | Clear the float e.g. `clear: both` if there is floats both on left and right |
| `box-sizing:`                | E.g. `border-box` or `content-box`                                           |

### Position

#### Relative

The element is positioned according to the normal flow of the document, and then offset relative to itself based on the values of top, right, bottom, and left. The offset does not affect the position of any other elements; thus, the space given for the element in the page layout is the same as if position were static.

#### Absolute

The element is removed from the normal document flow, and no space is created for the element in the page layout. It is positioned relative to its closest positioned ancestor, if any; otherwise, it is placed relative to the initial containing block. Its final position is determined by the values of top, right, bottom, and left.

#### Static

The element is positioned according to the normal flow of the document. The top, right, bottom, left, and z-index properties have no effect. This is the default value.

### display

The display CSS property sets whether an element is treated as a block or inline element and the layout used for its children, such as flow layout, grid or flex.

Formally, the display property sets an element's inner and outer display types. The outer type sets an element's participation in flow layout; the inner type sets the layout of children. Some values of display are fully defined in their own individual specifications; for example the detail of what happens when display: flex is declared is defined in the CSS Flexible Box Model specification

#### block

The element generates a block element box, generating line breaks both before and after the element when in the normal flow.

#### inline

The element generates one or more inline element boxes that do not generate line breaks before or after themselves. In normal flow, the next element will be on the same line if there is space.

#### inline-block

The element generates a block element box that will be flowed with surrounding content as if it were a single inline box (behaving much like a replaced element would).

### + operator

The “+” sign selector is used to select the elements that are placed immediately after the specified element but not inside the particular elements.

### `::after` and `::before`

Example:

![::after](999-img/2021-08-26-21-20-16.png)

Example:

![::afterv1](999-img/2021-08-26-21-22-13.png)

### Float

E.g. `float: none`, `float: left;` or `float:right`.

The float CSS property places an element on the left or right side of its container, allowing text and inline elements to wrap around it. The element is removed from the normal flow of the page, though still remaining a part of the flow (in contrast to absolute positioning).

Example of `float:right`:

![float:right](999-img/2021-08-28-14-02-46.png)

### `border-box`

The box-sizing CSS property sets how the total width and height of an element is calculated.

By default in the CSS box model, the width and height you assign to an element is applied only to the element's content box. If the element has any border or padding, this is then added to the width and height to arrive at the size of the box that's rendered on the screen. This means that when you set width and height, you have to adjust the value you give to allow for any border or padding that may be added. For example, if you have four boxes with width: 25%;, if any has left or right padding or a left or right border, they will not by default fit on one line within the constraints of the parent container.

The box-sizing property can be used to adjust this behavior:

- content-box gives you the default CSS box-sizing behavior. If you set an element's width to 100 pixels, then the element's content box will be 100 pixels wide, and the width of any border or padding will be added to the final rendered width, making the element wider than 100px.

- border-box tells the browser to account for any border and padding in the values you specify for an element's width and height. If you set an element's width to 100 pixels, that 100 pixels will include any border or padding you added, and the content box will shrink to absorb that extra width. This typically makes it much easier to size elements. box-sizing: border-box is the default styling that browsers use for the `<table>`, `<select>`, and `<button>` elements, and for `<input>` elements whose type is radio, checkbox, reset, button, submit, color, or search.

Please note: It is often useful to set box-sizing to border-box to layout elements. This makes dealing with the sizes of elements much easier, and generally eliminates a number of pitfalls you can stumble on while laying out your content. On the other hand, when using position: relative or position: absolute, use of box-sizing: content-box allows the positioning values to be relative to the content, and independent of changes to border and padding sizes, which is sometimes desirable.

## Semantic HTML

Semantic HTML: In addition to function, tags also have a meaning.

## CSS

Cascading Style Sheets

### Inline CSS

Writing css code inside element e.g. `<h1 style="color: blue">This text is blue</h1>`. NOT RECOMMENDED!

### Internal CSS

Writing Css code inside `<style>` brackets. The `<style>` tags shall be in the
`<header>` section i.e.

```html
<html>
  <head>
    <title>Title</title>
    <style>
      h1 {
        color: blue;
      }
    </style>
  </head>
  <body></body>
</html>
```

### External Css

Create a new file `style.css` like:

```css
h1 {
  color: blue;
}
```

and link the file `style.css` in the html file within the `<head>` segment with
the following code tag: `<link href="style.css" rel="stylesheet">`.

### Inheritance

If you style `<p>`, all the tags within the `<p>` tag will follow. i.e.
if you have `<p>hey <strong>you</strong></p>` and you style `<p>`, then
`<strong>` will inherit the style.

### Combining selectors

You can use the same properties for many selecters at the same time e.g.,

```css
h1,
h2,
h3,
h4,
li,
p {
  font-family: sans-serif;
}
```

Modify `<p>` tags only in the `<footer>` - use then:

```css
footer p {
  font-size: 10px;
}
```

Same for `<p>` tags in headers - use then

```css
header p {
  font-style: italic;
}
```

Following code formats `<p>` tags which is inside a `<header>` tag which itself
is in a `<article>` tag.

### Classes and id-selectors

Comment in css: `/* comment */`

Comment in VS-code: `<C-/>`:

Working with ID's in CSS:

- Specify id in a html tag like `<p id="copyright>` or `<p id="author">` and
  then use `#author {}` and `#copyright{}` in the css file for styling. Make sure
  that there can only be 1 id in the html file. If you want to use the styling in
  several different places you need to use classes. These are specified in the
  same way i.e. `<p class="related-author">` and then `.related-author{}` in the
  css file.

Disable bullet points: `ul {list-style = none;}`

You should use classes and not id's.

color can be specified as `rgb(x,y,z)` or `#hexvalue`. `rgba()` also specifies
transparancy.

Selectors are additive.

You can basically give an area a name i.e. `<header>`and then only choose to
style it with `header {background-color: black;}` If you have similar areas of
`<header>`, you can basically add a class to it.

If you want to add a background color to whole document, just add `body {background-color: blue;}`

Two methods set the first bullet list to another style than the rest of them:

1. Set class "first-li" to all first `<li>` tags in a list i.e. `<li class="first-li">`
2. Without modifying the html code, you can write following code in the `css`
   file `li:first-child {font-weight: bold;}` This is called pseudo-classes.

### Pseudo-classes

Examples of pseudo classe
s

```css
/* first list element */
li:first-child {
  font-weight: bold;
}

/* last list element */
li:last-child {
  font-style: italic;
}

/* Second list element */
li:nth-child(2) {
  color: red;
}

/* all odd list elements */
li:nth-child(odd) {
  color: black;
}
```

Another example that will not work which is a common missconseption on how
pseudo classes works.

For example, if we have this html code:

```html
<article>
  <header>
    <h2>The Basic Language of the Web: HTML</h2>

    <img
      src="img/laura-jones.jpg"
      alt="Headshot of Laura Jones"
      height="50"
      width="50"
    />

    <p id="author">
      Posted by <strong>Laura Jones</strong> on Monday, June 21st 2027
    </p>
  </header>
</article>
```

and we are using the following `css` code:

`article p:first-child {color:red}` will not work since `<p>` is not the first
child of `<article>`, it is header which is the first child of `<article>` will
not work since `<p>` is not the first child of `<article>`, it is header which
is the first child of `<article>`. So what would work in this case is only
`artcile header { color:purple;}`.

In the following html code we see that `<p>` is the last child of `<article>`,
here we could use: `article p:last-child { color: red;}` to style that.

### Styling hyperlinks

```css
/* Styling hyperlinks */
a:link {
  color: #1098ad;
  text-decoration: none; /* NO UNDERLINE ON LINKS */
}

a:visited {
  color: #1098ad; /* SAME COLOR ON LINKS*/
}

a:hover {
  color: orange;
  font-weight: bold;
  text-decoration: underline dotted orangered;
}

a:active {
  background-color: black;
  font-style: italic;
}
```

### Chrome dev tools

You can do some testing under following link without changing any code:

`Right click->inspect->elements`

### Conflicts between selectors

1. SHOULD NOT BE USED: Declaration marked `!important`.
2. SHOULD NOT BE USED: Inline style (style attribute in HTML)
3. Highest priority: ID selector (Last selector gets applied)
4. Class (.) or pseudo class (:) selector
5. Element selector (p, div, li, etc)
6. Universal selector

### Inheritance and the universal selector

Inheritance comes from parent tags.

Style `a (link)` and `p` tags within `a` nav tag:

`nav a:link, nav p { font-size: 18px; }`

or you could just do: `nav { font-size: 18px;}` which basically is the same if
there is only a `<a>` and `<p>` tag inside the `<nav>`.

Universal selector: `* {}`, you could also use `body {}`.

### Box model

Following codes are equal:

```css
.main-header {
  padding: 20px;
  padding-left: 40px;
  padding-right: 40px;
}
```

```css
.main-header {
  padding: 20px 40px;
}
```

### Collapsing margins

Something about the how css adds upp margins between two boxes.

### Images

Set the width or height to what is specified in the html tag, use:

`.post-img { width: 100%; height: auto;}`

The `width: 100%` is making the width of the pciture dynamic.

### Centering our page

Add container of what you want to center line `<div class="container">`.
Add following in the css `.container {width: 700px}; margin-left: auto; margin-right: auto;}` This centers the page and is dynamic.

### Different types of boxes

- Inline boxes: Dont create any vertical space outside the element i.e. the
  margin: i.e. `nav a: link {margin: 20px; }` wont work since it does not create any vertical space. The padding will
  indeed work since it is inside the box i.e. `nav a:link {padding: 20px;}`. To
  change it to an block level element with `nav a:link {margin:20px; padding:20px; display: block;}`. This will get the `margin` to work..

- Block level elements:

- Inline block element: Combination of inline element and box element e.g. `nav a: link {margin-top:30px; display:inline-block;}`

- Images are inline-block elements.

### Absolute positioning

If you want to add a **Like Button** in the botton of the page (right). You can
first add a `<button>` tag in the html code then in the css code you can
specify: `button { position: absolute; bottom: 50px; right: 50px;}` and then in
the body you can add `body {position:relative;}`. You can also put the
`relative` position in a container.

Should only be used for single elements.

### Pseudo elements

Style first letter in `<h1>` directly from css:

```css
h1::first-letter {
  font-style: normal;
  margin-right: 10px;
}
```

Style first line in all `<p>` tags:

```css
p::first-line {
  color: red;
}
```

Style the first line in a paragraph directly after a `<h3>` tag:

```css
h3 + p::first-line {
  color: darkorchid;
}
```

Add a cool "top box" next to a `<h2>` header:

```css
h2 {
position:relative;
}
h2::after {
content: "TOP";
background-color: yellow;
color:black;
font-size: 16px;
font-weight: bold;
display: inline-block;
padding: 5px 10px;
position: absolute;
top:-15px;
right: -25px;
```

### Centering

One ususal misstake that people do is that they try to center e.g. text inside
inline elements. For example, you have:

```html
<nav>
  <a href="blog.html">Blog</a>
  <a href="#">Challenges</a>
  <a href="#">Flexbox</a>
  <a href="#">CSS Grid</a>
</nav>
```

and then you want to center the links with:

```css
nav a:link {
  text-align: center;
}
```

This will not work since inline elements dont have any space over for what it
contains.

The solution is that you should place the `text-align:center;` property to its
parent.

The solution is that you should place the `text-align:center;` property to its
parent i.e.

```css
nav {
  text-align: center;
}
```

## Layouts

Three types of layouts:

1. Floats
2. Flexbox
3. Grid

### Float

If a container, header, or whatsoever contains child elements which all are floated, then the height of the container will collapse.
You can clear floats by adding a `<div class="clear"></div>` element into the container and in the css code state: `.clear {clear: both};`.

You could also add a class called `clearfix` to the parent element and then add a new last child element with `.clearfix::after { clear: both; content:''; display: block}`

If the contents dont fit in a flow dynamic based on the components weights, you can use the `box-sizing: border-box;`. If you want this box model be applied to all elements on the page, just put it in the universal selector `* {}`. You cannot put it in the body section since `box-sizing:` doesnt get inherited.

## Flexbox

### Introduction

#### Base code

Following code gives:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Flexbox</title>
    <style>
      .el--1 {
        background-color: blueviolet;
      }
      .el--2 {
        background-color: orangered;
      }
      .el--3 {
        background-color: green;
        height: 250px;
      }
      .el--4 {
        background-color: goldenrod;
      }
      .el--5 {
        background-color: palevioletred;
      }
      .el--6 {
        background-color: steelblue;
      }
      .el--7 {
        background-color: yellow;
      }
      .el--8 {
        background-color: crimson;
      }

      .container {
        /* STARTER */
        font-family: sans-serif;
        background-color: #ddd;
        font-size: 34px;
        margin: 40px;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="el el--1">HTML</div>
      <div class="el el--2">and</div>
      <div class="el el--3">CSS</div>
      <div class="el el--4">are</div>
      <div class="el el--5">amazing</div>
      <div class="el el--6">languages</div>
      <div class="el el--7">to</div>
      <div class="el el--8">learn</div>
    </div>
  </body>
</html>
```

Following output:

![flexbox-1](999-img/2021-08-29-12-30-33.png)

Please note that all child elements of the `<div class="container">` will be affected of the `flex` configuration.

#### Configuring flexbox

##### Base configuration

Adding:

```css
.container {
  display: flex;
}
```

activates flexbox. This gives the output:

![](999-img/2021-08-29-12-36-58.png)

Please note that:

- The grey color is the background color of the container (the empty part of the container).
- Horizontally, each element takes up the exactly space to fit its content.
- Vertically, all the elements takes the size of the tallest element. In this case the `CSS` box which has a height of 250 px.

##### `align-items: center`

Adding:

```css
.container {
  display: flex;
  align-items: center;
}
```

You will basically align all the boxes at the center of the container. Elements will be at their true height. Please see below:

![](999-img/2021-08-29-16-40-13.png)

##### `align-items: flex-start`

```css
.container {
  display: flex;
  align-items: flex-start;
}
```

Aligns all the boxes at the start of the container. Elements will be at their true height. Please see below:

![](999-img/2021-08-29-16-43-59.png)

##### `align-items: flex-end`

```css
.container {
  display: flex;
  align-items: flex-end;
}
```

Aligns all the boxes at the end of the container. Elements will be at their true height. Please see below:

![](999-img/2021-08-29-16-46-26.png)

##### `align-items: stretch`

```css
.container {
  display: flex;
  align-items: stretch;
}
```

Stretches the boxes to match the height of the tallest element in the container. The width will be exactly so that it fits its content of each box.

![](999-img/2021-08-29-16-50-10.png)

##### `justify-content: center`

Centers the elements in the container in the middle

```css
.container {
  display: flex;
  justify-content: center;
}
```

Please see image below:

![](999-img/2021-08-29-16-53-26.png)

##### `justify-content: space-between`

Sets equal space among the elements to match the horizontal size of container.

```css
.container {
  display: flex;
  justify-content: space-between;
}
```

Please see image below:

![](999-img/2021-08-29-16-55-52.png)

### Spacing and aligning flex items

`align-items:` Vertical alignment
`justify-content:` horizontal alignment

Using following CSS code for the container:

```css
.container {
  /* STARTER */
  font-family: sans-serif;
  background-color: #ddd;
  font-size: 34px;
  margin: 40px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
```

This means that all elements are aligned like following:

![](999-img/2021-08-29-17-20-46.png)

#### Overriding `align-items:` for elements with `align-self:`

You can override this for several or one element with the `align-self:` attribute.

Example 1:

```css
.el--1 {
  align-self: flex-start;
}
```

will give you:

![](999-img/2021-08-29-17-26-39.png)

Example 2:

```css
.el--5 {
  align-self: stretch;
}
```

will give you the following output:

![](999-img/2021-08-29-17-31-27.png)

#### Rearranging individual elements with `order:`

Example 1:

```css
.el--6 {
  order: -1;
}
```

Which will give you:

![](999-img/2021-08-29-17-50-13.png)

Example 2:

```css
.el--5 {
  order: 1;
}
```

will give you:

![](999-img/2021-08-29-17-57-15.png)

#### Adding space between items with `gap:`

Example:

```css
.container {
  font-family: sans-serif;
  background-color: #ddd;
  font-size: 34px;
  margin: 40px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  /* gap: 30px; */
}
```

givea gap between the elements of 30px:

![](999-img/2021-08-29-18-08-59.png)

### The `flex` property

The default property of flex is:

```css
.el {
  flex-grow: 0;
  flex-shrink: 1;
  flex-basis: auto;
}
```

#### `with` of elements with flex

With `flex`, you should not use the `width:` property, you should instead use `flex-basis:`.

Example:

```css
.el {
  flex-basis: 100px;
}
```

This will give following output:

![](999-img/2021-08-29-18-56-03.png)

#### `flex-shrink:` property

Please note that with `flex-basis:`, normally, the width of the elements will extend to 100px. But if them content in the element has larger size than specified, e.g. 100px as in the prior example, the `flex-basis:` proprty will extend 100px until it fits its contents. This is actually a feature of the `flex-grow:` property.

Another note is that if you give the elements a really big size, lets say for example 200px. The elements will extend to so its fits its container, not more. So the ultime width of its element will be smaller if 200px is to large. The browsert will calibrate the width so the elements exactly fits its container. This feature is coming from the default value of `flex-shrink:1`.

So, as an example:

```css
.el {
  /* DEFAULT flex portperties */
  /* flex-grow: 0;
  flex-shrink: 1;
  flex-basis: auto; */

  flex-basis: 200px;
}
```

will give the following output:

![](999-img/2021-08-29-19-04-55.png)

If we now edit the default property of `flex-shrink:1` to `flex-shrink: 0`. This gives:

```css
.el {
  /* DEFAULT flex portperties */
  /* flex-grow: 0;*/
  flex-shrink: 0;
  /* flex-basis: auto; */

  flex-basis: 200px;
}
```

This gives the output:

![](999-img/2021-08-29-19-11-12.png)

This basically forces every element to 200px even if it extends beyond the container.

#### `flex-grow:` property

The following code:

```css
.el {
  flex-shrink: 0;
}
```

gives:

![](999-img/2021-08-29-19-38-10.png)

but extending the code with,

```css
.el {
  flex-shrink: 0;
  flex-grow: 1;
}
```

gives the output:

![](999-img/2021-08-29-19-40-30.png)

The `flex-grow:1` property divides the maxiumum space in the container evenly among the elements inside the container.

If you set the `flex-grow:1` property for an individual element, the other elemenhts will fill up its content and the element that has the property `flex-grow:1` will fill up the rest of the empty space isnide the container.

```css
.el--1 {
  flex-grow: 1;
}
```

gives: ;

![](999-img/2021-08-29-19-47-49.png)

The value of `flex-grow:` is also relative to the rest of the elements. For example, if we in the container have `.el {flex-grow:1}` and in a single element have `.el--1 { flex-grow:2}`. This means that the element 1 will have 2 times the size of the available space as compared to the rest of the elements.

#### The `flex:` property

`flex:` property is a short for `flex-grow:`, `flex-shrink:` and `flex-basis:`. So for example, `flex: 0 0 200px;` actually means:

```css
.el {
  flex-grow: 0;
  flex-shrink: 0;
  flex-basis: 200px;
}
```

You should always use `flex:` and not the other three ones.
# Responsive-websites
