# html and css notes

## html tags

| tag                              | description                      |
| -------------------------------- | -------------------------------- |
| `<doctype html>`                 |                                  |
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
| `<a href="mypage.html">link</a>` |                                  |
| `<article>`                      |                                  |
| `<img src="image.jpg"/>`         |                                  |
| `<p>`                            |                                  |
| `<strong>`                       |                                  |
| `<b>`                            |                                  |
| `<em>`                           |                                  |
| `<ol>`                           | numbered list                    |
| `<ul>`                           | bullet list                      |
| `<li>`                           | bullet (inside `<ul>` or `<ol>`) |
| `<footer>`                       |                                  |
| `<aside>`                        |                                  |
| `<button>`                       |                                  |
| `<h1 style="color: blue">`       |                                  |
| `<style>`                        | css                              |
| `footer`                         |                                  |

## css tags

| tag                          | description                                                                  |
| ---------------------------- | ---------------------------------------------------------------------------- |
| `font-size`                  | size of font e.g. 20px                                                       |
| `font-family`                | font e.g. `sans-serif`                                                       |
| `text-transform`             | lowercase, uppercase etc.                                                    |
| `font-style`                 | italic, bold, etc                                                            |
| `text-align`                 | left, center, right, etc                                                     |
| `line-height`                | spacing between lines e.g for `<p>`                                          |
| `list-style`                 | square, circle, number                                                       |
| `background-color`           | background color for area                                                    |
| `border`                     | border                                                                       |
| `border-top`                 | top border                                                                   |
| `border-bottom`              | bottom border                                                                |
| `border: 5px solid black`    | 5px solid black border                                                       |
| `* {}`                       | whole document                                                               |
| `body {}`                    | whole body tag                                                               |
| `margin`                     | sets the margin area on all four sides of an element                         |
| `margin: 1px 2px`            | vertical-horizontal margin                                                   |
| `margin: 1px 2px 3px`        | top-horizontal-bottom margin                                                 |
| `margin: 1px 2px 3px 4px`    | top-right-botton-left margin                                                 |
| `margin-bottom: 1px`         | botton margin                                                                |
| `margin-left: 1px`           | left margin                                                                  |
| `margin-top: 1px`            | top margin                                                                   |
| `margin-right: 1px`          | right margin                                                                 |
| `text-align:`                | alignement of text                                                           |
| `text-transform:`            | e.g. `uppercase` or `lowercase`                                              |
| `padding:`                   | sets the padding area for all four sides of an element                       |
| `font-weight:`               | e.g. `bold`                                                                  |
| `text-decoration`            | e.g. `underline`, `none`. used with links                                    |
| `cursor:`                    | sets the mouse cursor at hoover                                              |
| `<a hre... class="x">x</a>`  | please see below - css and links                                             |
| `.x:hover {}`                | style at hoover in class `x`                                                 |
| `.x:active {}`               | style at link click                                                          |
| `.x:link {}`                 | link style                                                                   |
| `.x:visited {}`              | link style when visited                                                      |
| `<ul class="list">`          | see blow for styling                                                         |
| `.list{list-style: square;}` | squared bullets in list                                                      |
| `.list li {}`                | styling of each bullet e.g. `margin-left:`                                   |
| `if <p id="test">`           | use then `#test {}`                                                          |
| `if <p>`                     | use then `p {}`                                                              |
| `if <p class="test">`        | use then `.test{}`                                                           |
| `position:`                  | e.g. `absolute`, `relative`                                                  |
| `.x{position: relative}`     | offset relative to itself with (see: position below)                         |
| `.x{position: absolute}`     | removed from normal flow of document (see: position below)                   |
| `width`                      | sets an elements width                                                       |
| `li:first-child {}`          | first bullet                                                                 |
| `li:last-child {}`           | last bullet                                                                  |
| `li:nth-child(even)`         | even numbered bullets                                                        |
| `display:`                   | e.g. `inline`, `inline-block`, `block`. (see:display)                        |
| `a:link {}`                  | style for links in `<a>` tags                                                |
| `a:hover {}`                 | style for links in `<a>` when hoovered                                       |
| `a:active {}`                | style for links in `<a>` when clicked                                        |
| `nav a:link {}`              | style for links in `<a>` which itself is in a `<nav>` tag                    |
| `nav a:link:last-child {}`   | last link in `<a>` -> `<navb>`                                               |
| `button {}`                  | design for a `<button>` tag.                                                 |
| `h3 + p {}`                  | style the `<p>` directly after `h3` (see: + operator)                        |
| `h3 + p::first-line {}`      | style the first line of the paragraph which lies after `<h3>`                |
| `h1::first-letter {}`        | style the first letter in `<h1>`                                             |
| `element::after {}`          | see ::after and ::before                                                     |
| `element::before {}`         | see `::after` and `::before`                                                 |
| `float:`                     | let the element float e.g. `float: left;`                                    |
| `clear:`                     | clear the float e.g. `clear: both` if there is floats both on left and right |
| `box-sizing:`                | e.g. `border-box` or `content-box`                                           |

### position

#### relative

the element is positioned according to the normal flow of the document, and then offset relative to itself based on the values of top, right, bottom, and left. the offset does not affect the position of any other elements; thus, the space given for the element in the page layout is the same as if position were static.

#### absolute

the element is removed from the normal document flow, and no space is created for the element in the page layout. it is positioned relative to its closest positioned ancestor, if any; otherwise, it is placed relative to the initial containing block. its final position is determined by the values of top, right, bottom, and left.

#### static

the element is positioned according to the normal flow of the document. the top, right, bottom, left, and z-index properties have no effect. this is the default value.

### display

the display css property sets whether an element is treated as a block or inline element and the layout used for its children, such as flow layout, grid or flex.

formally, the display property sets an element's inner and outer display types. the outer type sets an element's participation in flow layout; the inner type sets the layout of children. some values of display are fully defined in their own individual specifications; for example the detail of what happens when display: flex is declared is defined in the css flexible box model specification

#### block

the element generates a block element box, generating line breaks both before and after the element when in the normal flow.

#### inline

the element generates one or more inline element boxes that do not generate line breaks before or after themselves. in normal flow, the next element will be on the same line if there is space.

#### inline-block

the element generates a block element box that will be flowed with surrounding content as if it were a single inline box (behaving much like a replaced element would).

### + operator

the “+” sign selector is used to select the elements that are placed immediately after the specified element but not inside the particular elements.

### `::after` and `::before`

example:

![::after](999-img/2021-08-26-21-20-16.png)

example:

![::afterv1](999-img/2021-08-26-21-22-13.png)

### float

e.g. `float: none`, `float: left;` or `float:right`.

the float css property places an element on the left or right side of its container, allowing text and inline elements to wrap around it. the element is removed from the normal flow of the page, though still remaining a part of the flow (in contrast to absolute positioning).

example of `float:right`:

![float:right](999-img/2021-08-28-14-02-46.png)

### `border-box`

the box-sizing css property sets how the total width and height of an element is calculated.

by default in the css box model, the width and height you assign to an element is applied only to the element's content box. if the element has any border or padding, this is then added to the width and height to arrive at the size of the box that's rendered on the screen. this means that when you set width and height, you have to adjust the value you give to allow for any border or padding that may be added. for example, if you have four boxes with width: 25%;, if any has left or right padding or a left or right border, they will not by default fit on one line within the constraints of the parent container.

the box-sizing property can be used to adjust this behavior:

- content-box gives you the default css box-sizing behavior. if you set an element's width to 100 pixels, then the element's content box will be 100 pixels wide, and the width of any border or padding will be added to the final rendered width, making the element wider than 100px.

- border-box tells the browser to account for any border and padding in the values you specify for an element's width and height. if you set an element's width to 100 pixels, that 100 pixels will include any border or padding you added, and the content box will shrink to absorb that extra width. this typically makes it much easier to size elements. box-sizing: border-box is the default styling that browsers use for the `<table>`, `<select>`, and `<button>` elements, and for `<input>` elements whose type is radio, checkbox, reset, button, submit, color, or search.

please note: it is often useful to set box-sizing to border-box to layout elements. this makes dealing with the sizes of elements much easier, and generally eliminates a number of pitfalls you can stumble on while laying out your content. on the other hand, when using position: relative or position: absolute, use of box-sizing: content-box allows the positioning values to be relative to the content, and independent of changes to border and padding sizes, which is sometimes desirable.

## semantic html

semantic html: in addition to function, tags also have a meaning.

## css

cascading style sheets

### inline css

writing css code inside element e.g. `<h1 style="color: blue">this text is blue</h1>`. not recommended!

### internal css

writing css code inside `<style>` brackets. the `<style>` tags shall be in the
`<header>` section i.e.

```html
<html>
  <head>
    <title>title</title>
    <style>
      h1 {
        color: blue;
      }
    </style>
  </head>
  <body></body>
</html>
```

### external css

create a new file `style.css` like:

```css
h1 {
  color: blue;
}
```

and link the file `style.css` in the html file within the `<head>` segment with
the following code tag: `<link href="style.css" rel="stylesheet">`.

### inheritance

if you style `<p>`, all the tags within the `<p>` tag will follow. i.e.
if you have `<p>hey <strong>you</strong></p>` and you style `<p>`, then
`<strong>` will inherit the style.

### combining selectors

you can use the same properties for many selecters at the same time e.g.,

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

modify `<p>` tags only in the `<footer>` - use then:

```css
footer p {
  font-size: 10px;
}
```

same for `<p>` tags in headers - use then

```css
header p {
  font-style: italic;
}
```

following code formats `<p>` tags which is inside a `<header>` tag which itself
is in a `<article>` tag.

### classes and id-selectors

comment in css: `/* comment */`

comment in vs-code: `<c-/>`:

working with id's in css:

- specify id in a html tag like `<p id="copyright>` or `<p id="author">` and
  then use `#author {}` and `#copyright{}` in the css file for styling. make sure
  that there can only be 1 id in the html file. if you want to use the styling in
  several different places you need to use classes. these are specified in the
  same way i.e. `<p class="related-author">` and then `.related-author{}` in the
  css file.

disable bullet points: `ul {list-style = none;}`

you should use classes and not id's.

color can be specified as `rgb(x,y,z)` or `#hexvalue`. `rgba()` also specifies
transparancy.

selectors are additive.

you can basically give an area a name i.e. `<header>`and then only choose to
style it with `header {background-color: black;}` if you have similar areas of
`<header>`, you can basically add a class to it.

if you want to add a background color to whole document, just add `body {background-color: blue;}`

two methods set the first bullet list to another style than the rest of them:

1. set class "first-li" to all first `<li>` tags in a list i.e. `<li class="first-li">`
2. without modifying the html code, you can write following code in the `css`
   file `li:first-child {font-weight: bold;}` this is called pseudo-classes.

### pseudo-classes

examples of pseudo classe
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

/* second list element */
li:nth-child(2) {
  color: red;
}

/* all odd list elements */
li:nth-child(odd) {
  color: black;
}
```

another example that will not work which is a common missconseption on how
pseudo classes works.

for example, if we have this html code:

```html
<article>
  <header>
    <h2>the basic language of the web: html</h2>

    <img
      src="img/laura-jones.jpg"
      alt="headshot of laura jones"
      height="50"
      width="50"
    />

    <p id="author">
      posted by <strong>laura jones</strong> on monday, june 21st 2027
    </p>
  </header>
</article>
```

and we are using the following `css` code:

`article p:first-child {color:red}` will not work since `<p>` is not the first
child of `<article>`, it is header which is the first child of `<article>` will
not work since `<p>` is not the first child of `<article>`, it is header which
is the first child of `<article>`. so what would work in this case is only
`artcile header { color:purple;}`.

in the following html code we see that `<p>` is the last child of `<article>`,
here we could use: `article p:last-child { color: red;}` to style that.

### styling hyperlinks

```css
/* styling hyperlinks */
a:link {
  color: #1098ad;
  text-decoration: none; /* no underline on links */
}

a:visited {
  color: #1098ad; /* same color on links*/
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

### chrome dev tools

you can do some testing under following link without changing any code:

`right click->inspect->elements`

### conflicts between selectors

1. should not be used: declaration marked `!important`.
2. should not be used: inline style (style attribute in html)
3. highest priority: id selector (last selector gets applied)
4. class (.) or pseudo class (:) selector
5. element selector (p, div, li, etc)
6. universal selector

### inheritance and the universal selector

inheritance comes from parent tags.

style `a (link)` and `p` tags within `a` nav tag:

`nav a:link, nav p { font-size: 18px; }`

or you could just do: `nav { font-size: 18px;}` which basically is the same if
there is only a `<a>` and `<p>` tag inside the `<nav>`.

universal selector: `* {}`, you could also use `body {}`.

### box model

following codes are equal:

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

### collapsing margins

something about the how css adds upp margins between two boxes.

### images

set the width or height to what is specified in the html tag, use:

`.post-img { width: 100%; height: auto;}`

the `width: 100%` is making the width of the pciture dynamic.

### centering our page

add container of what you want to center line `<div class="container">`.
add following in the css `.container {width: 700px}; margin-left: auto; margin-right: auto;}` this centers the page and is dynamic.

### different types of boxes

- inline boxes: dont create any vertical space outside the element i.e. the
  margin: i.e. `nav a: link {margin: 20px; }` wont work since it does not create any vertical space. the padding will
  indeed work since it is inside the box i.e. `nav a:link {padding: 20px;}`. to
  change it to an block level element with `nav a:link {margin:20px; padding:20px; display: block;}`. this will get the `margin` to work..

- block level elements:

- inline block element: combination of inline element and box element e.g. `nav a: link {margin-top:30px; display:inline-block;}`

- images are inline-block elements.

### absolute positioning

if you want to add a **like button** in the botton of the page (right). you can
first add a `<button>` tag in the html code then in the css code you can
specify: `button { position: absolute; bottom: 50px; right: 50px;}` and then in
the body you can add `body {position:relative;}`. you can also put the
`relative` position in a container.

should only be used for single elements.

### pseudo elements

style first letter in `<h1>` directly from css:

```css
h1::first-letter {
  font-style: normal;
  margin-right: 10px;
}
```

style first line in all `<p>` tags:

```css
p::first-line {
  color: red;
}
```

style the first line in a paragraph directly after a `<h3>` tag:

```css
h3 + p::first-line {
  color: darkorchid;
}
```

add a cool "top box" next to a `<h2>` header:

```css
h2 {
position:relative;
}
h2::after {
content: "top";
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

### centering

one ususal misstake that people do is that they try to center e.g. text inside
inline elements. for example, you have:

```html
<nav>
  <a href="blog.html">blog</a>
  <a href="#">challenges</a>
  <a href="#">flexbox</a>
  <a href="#">css grid</a>
</nav>
```

and then you want to center the links with:

```css
nav a:link {
  text-align: center;
}
```

this will not work since inline elements dont have any space over for what it
contains.

the solution is that you should place the `text-align:center;` property to its
parent.

the solution is that you should place the `text-align:center;` property to its
parent i.e.

```css
nav {
  text-align: center;
}
```

## layouts

three types of layouts:

1. floats
2. flexbox
3. grid

### float

if a container, header, or whatsoever contains child elements which all are floated, then the height of the container will collapse.
you can clear floats by adding a `<div class="clear"></div>` element into the container and in the css code state: `.clear {clear: both};`.

you could also add a class called `clearfix` to the parent element and then add a new last child element with `.clearfix::after { clear: both; content:''; display: block}`

if the contents dont fit in a flow dynamic based on the components weights, you can use the `box-sizing: border-box;`. if you want this box model be applied to all elements on the page, just put it in the universal selector `* {}`. you cannot put it in the body section since `box-sizing:` doesnt get inherited.

## flexbox

### introduction

#### base code

following code gives:

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta http-equiv="x-ua-compatible" content="ie=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>flexbox</title>
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
        /* starter */
        font-family: sans-serif;
        background-color: #ddd;
        font-size: 34px;
        margin: 40px;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="el el--1">html</div>
      <div class="el el--2">and</div>
      <div class="el el--3">css</div>
      <div class="el el--4">are</div>
      <div class="el el--5">amazing</div>
      <div class="el el--6">languages</div>
      <div class="el el--7">to</div>
      <div class="el el--8">learn</div>
    </div>
  </body>
</html>
```

following output:

![flexbox-1](999-img/2021-08-29-12-30-33.png)

please note that all child elements of the `<div class="container">` will be affected of the `flex` configuration.

#### configuring flexbox

##### base configuration

adding:

```css
.container {
  display: flex;
}
```

activates flexbox. this gives the output:

![](999-img/2021-08-29-12-36-58.png)

please note that:

- the grey color is the background color of the container (the empty part of the container).
- horizontally, each element takes up the exactly space to fit its content.
- vertically, all the elements takes the size of the tallest element. in this case the `css` box which has a height of 250 px.

##### `align-items: center`

adding:

```css
.container {
  display: flex;
  align-items: center;
}
```

you will basically align all the boxes at the center of the container. elements will be at their true height. please see below:

![](999-img/2021-08-29-16-40-13.png)

##### `align-items: flex-start`

```css
.container {
  display: flex;
  align-items: flex-start;
}
```

aligns all the boxes at the start of the container. elements will be at their true height. please see below:

![](999-img/2021-08-29-16-43-59.png)

##### `align-items: flex-end`

```css
.container {
  display: flex;
  align-items: flex-end;
}
```

aligns all the boxes at the end of the container. elements will be at their true height. please see below:

![](999-img/2021-08-29-16-46-26.png)

##### `align-items: stretch`

```css
.container {
  display: flex;
  align-items: stretch;
}
```

stretches the boxes to match the height of the tallest element in the container. the width will be exactly so that it fits its content of each box.

![](999-img/2021-08-29-16-50-10.png)

##### `justify-content: center`

centers the elements in the container in the middle

```css
.container {
  display: flex;
  justify-content: center;
}
```

please see image below:

![](999-img/2021-08-29-16-53-26.png)

##### `justify-content: space-between`

sets equal space among the elements to match the horizontal size of container.

```css
.container {
  display: flex;
  justify-content: space-between;
}
```

please see image below:

![](999-img/2021-08-29-16-55-52.png)

### spacing and aligning flex items

`align-items:` vertical alignment
`justify-content:` horizontal alignment

using following css code for the container:

```css
.container {
  /* starter */
  font-family: sans-serif;
  background-color: #ddd;
  font-size: 34px;
  margin: 40px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
```

this means that all elements are aligned like following:

![](999-img/2021-08-29-17-20-46.png)

#### overriding `align-items:` for elements with `align-self:`

you can override this for several or one element with the `align-self:` attribute.

example 1:

```css
.el--1 {
  align-self: flex-start;
}
```

will give you:

![](999-img/2021-08-29-17-26-39.png)

example 2:

```css
.el--5 {
  align-self: stretch;
}
```

will give you the following output:

![](999-img/2021-08-29-17-31-27.png)

#### rearranging individual elements with `order:`

example 1:

```css
.el--6 {
  order: -1;
}
```

which will give you:

![](999-img/2021-08-29-17-50-13.png)

example 2:

```css
.el--5 {
  order: 1;
}
```

will give you:

![](999-img/2021-08-29-17-57-15.png)

#### adding space between items with `gap:`

example:

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

### the `flex` property

the default property of flex is:

```css
.el {
  flex-grow: 0;
  flex-shrink: 1;
  flex-basis: auto;
}
```

#### `with` of elements with flex

with `flex`, you should not use the `width:` property, you should instead use `flex-basis:`.

example:

```css
.el {
  flex-basis: 100px;
}
```

this will give following output:

![](999-img/2021-08-29-18-56-03.png)

#### `flex-shrink:` property

please note that with `flex-basis:`, normally, the width of the elements will extend to 100px. but if them content in the element has larger size than specified, e.g. 100px as in the prior example, the `flex-basis:` proprty will extend 100px until it fits its contents. this is actually a feature of the `flex-grow:` property.

another note is that if you give the elements a really big size, lets say for example 200px. the elements will extend to so its fits its container, not more. so the ultime width of its element will be smaller if 200px is to large. the browsert will calibrate the width so the elements exactly fits its container. this feature is coming from the default value of `flex-shrink:1`.

so, as an example:

```css
.el {
  /* default flex portperties */
  /* flex-grow: 0;
  flex-shrink: 1;
  flex-basis: auto; */

  flex-basis: 200px;
}
```

will give the following output:

![](999-img/2021-08-29-19-04-55.png)

if we now edit the default property of `flex-shrink:1` to `flex-shrink: 0`. this gives:

```css
.el {
  /* default flex portperties */
  /* flex-grow: 0;*/
  flex-shrink: 0;
  /* flex-basis: auto; */

  flex-basis: 200px;
}
```

this gives the output:

![](999-img/2021-08-29-19-11-12.png)

this basically forces every element to 200px even if it extends beyond the container.

#### `flex-grow:` property

the following code:

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

the `flex-grow:1` property divides the maxiumum space in the container evenly among the elements inside the container.

if you set the `flex-grow:1` property for an individual element, the other elemenhts will fill up its content and the element that has the property `flex-grow:1` will fill up the rest of the empty space isnide the container.

```css
.el--1 {
  flex-grow: 1;
}
```

gives: ;

![](999-img/2021-08-29-19-47-49.png)

the value of `flex-grow:` is also relative to the rest of the elements. for example, if we in the container have `.el {flex-grow:1}` and in a single element have `.el--1 { flex-grow:2}`. this means that the element 1 will have 2 times the size of the available space as compared to the rest of the elements.

#### the `flex:` property

`flex:` property is a short for `flex-grow:`, `flex-shrink:` and `flex-basis:`. so for example, `flex: 0 0 200px;` actually means:

```css
.el {
  flex-grow: 0;
  flex-shrink: 0;
  flex-basis: 200px;
}
```

you should always use `flex:` and not the other three ones.

## flex grid:

```css
.container{
  display: grid;
  grid_template-columns: 250px 150px /* two columns, one 250px wide and one 150px wide */
  grid-template-rows: 300px 200px; /* two rows, first row 300px and second 200px */
  gap: 30px; /* creates between the items in the grid */
  /* you can also use following */
  column-gap: 30px; /* creates a gap between the column */
  row-gap:60px; /* creates a gap between the rows */
}
```

when you need a one dimensional layout: use flexbox
when you need a two dimensional layout: use flex grid

create a grid container by setting `display: grid` to an container. the the items / containers in this container becomes the grid items.

grid-lines surrounds the grid cells.

gutters is a css word for gaps.

grid track is basically a row or column.

```css
display:grid;
grid-tempplate-columns: 200px 200px 1fr 100px; /* 1fr fills the rest of the empty space */
```

```css
display:grid;
grid-tempplate-columns: 200px 200px 1fr 1fr; /* both 3 and 4 column fill out the empty space */
```

```css
display:grid;
grid-tempplate-columns: 1fr 1fr 1fr 1fr; /* all columns fill out thte empty spacew */
```

```css
display:grid;
grid-tempplate-columns: 1fr 2fr 3fr 4fr; /* relative sizong */
```

```css
display:grid;
grid-tempplate-columns: 1fr 1fr 1fr auto; /* 4th column fills out the empty space.
```

```css
display:grid;
grid-tempplate-columns: repeat(4, 1fr); /* short for 1fr 1fr 1fr 1fr */
```

all the same as above implies for rows.

### palacing and and spanning grid items

```css
.el--8 {
  grid-column: 2 / 3; /* grid item should start at the beginning of column nr 2 and end at column 3 */ 
  grid-row: 1 / 2;
}

.el--2 {
  grid-column: 1; /* also possible */
  grid-row: 2; /* also possible */
}

.el--4 {
  grid-column: 1 / 3; /* spans over three columns */
  grid-row: 2; /* also possible */
}

.el--4 {
  grid-column: 1 / span 4; /* another syntax - same as above */
  grid-row: 2;
}

.el--4 {
  grid-column: 1 / -1; /* from the first column to the last column */
  grid-row: 2;
}
```

spanning works exactly the same with rows i.e. `grid-row`.

### aligning grid items

```css
/* CSS GRID */
display: grid;
grid-template-column: 125px 200px 125px;
grid-template-rows: 250px 100px;
gap: 50;

/* Aligning tracks inside container:
distribte empty spaces:*/

justify-content: center;

/* justify-content: flex-between; */

align-content: center;
/* align-content:  flex-between; */
/* align-content: end; //Like flex-end in flex-box */
/* align-content: start; //Like flex-start in flex-box */

/* Align items inside cells: moving items around inside cells */
aling-items: center;
justify-items: center;

/* Overriding settings in the main container */
.el--3 {
  align-selg: end;
  justify-self: end;
}
```

### Building a simple CSS grid layout