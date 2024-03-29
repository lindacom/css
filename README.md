CSS page layout
===============
A three column page layout should have header main, article, aside, aside, footer

```
<!DOCTYPE html>
<html>

<head>
    <title>Test page</title>
    <link rel="stylesheet" href="test.css" />
    <link rel="shortcut icon" href="#" />
    <link rel="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" />
    <script src="https://use.fontawesome.com/releases/v5.0.8/js/all.js"></script>

</head>
<header></header> 
<main></main>
<article></article>
<aside></aside> 
<aside></aside>
<footer></footer>

<body>
    </body>
    </html>
```

header and nav
---------------

A website is often divided into headers, menus, content and a footer. A header is usually located at the top of the website (or right below a top navigation menu). It often contains a logo or the website name.

Aligning header and navbar - notice header has position relative and nav has position absolute. Left and top are set to 0 so the nav will be positioned right up
agains top left corner of the header.  The width has also been set to 100% of the header.

```
 <header class="header">
            <nav>
                <ul>
                    <li><a href="./index.html">HOME</a></li>
                    <li><a href="store.html">STORE</a></li>
                    <li><a href="payment.html">PAYMENT</a></li>
                    <li style="float: right;"><a href="#"><i class="fas fa-shopping-cart"></i>cart</a></li>

                    <li style="float: right;"><a href="#" alt="counts items in localstorage"><i class="fas fa-shopping-cart" 
                    style=" background-color:red;"></i>
                    <span class="badge" id="badge">0 </span></a></li>
                </ul>
            </nav>

            <h1>My store</h1>
           
        </header>
 ```
 
 ```
 .header {
  height: 200px;
  padding: 20px;
  text-align: center;
  background-color: #1abc9c;
  color: white;
  font-size: 30px;
  position: relative;
}

body {
  background-color: #f6f6f6;
 }

.header nav ul {
  list-style-type: none;

  position: absolute;
  left: 0;
  top: 0;

  margin: 0;
  padding: 0;
  width: 100%;
  overflow: hidden;
  background-color: #333;
}

.header nav li {
  float: left;
}

.header nav li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

.header nav li a:hover {
  background-color: #111;
}

```
Content
--------
You can include all content within a container.

```
.container {
  max-width: 900px;
  padding: 0 1.5em;
  margin: 0 auto;
}
```
Content can be one, two or three column layout. use margin: 0 auto to centre the content in the middle of the container width.

Colours
========
1. select complimentary colours for the website from the colour wheel:
2. Create CSS Variables - to apply colour
3. Apply colours to elements  e.g background-color: var(--yellow); 

```
/* CSS Variables */

:root {
  --primary: #ddd;
  --dark: #333;
  --light: #fff;
  --shadow: 0 1px 5px rgba(104, 104, 104, 0.8);
  --darkgrey: #CFDBD5;
  --lightgrey: #E8EDDF;
  --yellow: #F5CB5C;
  --black: #242423;
  --blackgrey: #333533;
```

icons
======
use font awesome
```
    <link rel="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" />
        <script src="https://use.fontawesome.com/releases/v5.0.8/js/all.js"></script>
```

Increase font awesome icon size e.g.

```
<i class="fas fa-window-close fa-2x"></i>
```

TUTORIALS
==========

Building a responsive grid CSS grid website layout from scratch (45mins 32)
https://www.youtube.com/watch?v=moBhzSC455o

CSS Grid starter layouts
https://css-tricks.com/snippets/css/css-grid-starter-layouts/


Colour wheels
===============


https://coolors.co/353535-3c6e71-ffffff-d9d9d9-284b63
Colour wheel - https://www.canva.com/colors/color-wheel/
contrast checker - https://webaim.org/resources/contrastchecker/
Accessibility tool - AXE (google chrome extension)
