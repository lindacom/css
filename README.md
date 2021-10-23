CSS page layout
===============

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

TUTORIALS
==========

Building a responsive grid CSS grid website layout from scratch (45mins 32)
https://www.youtube.com/watch?v=moBhzSC455o

Colour wheels
===============
select complimentary colours for the website from the colour wheel:

https://coolors.co/353535-3c6e71-ffffff-d9d9d9-284b63
Colour wheel - https://www.canva.com/colors/color-wheel/
contrast checker - https://webaim.org/resources/contrastchecker/
Accessibility tool - AXE (google chrome extension)
