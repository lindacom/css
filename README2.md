Remove bullet styling
======================
```
.shop-item-details > ul  {
  list-style-type: none;
}
```
Icons
=====
Stars:

```
<span class="fa fa-star checked"></span>
```
Text colour red
===============

```
<p style="color:red;">Free shipping on orders over £30!!</p>
```
Gradient
=========
```
background-image: linear-gradient(to right, red , yellow);
```

Insert a horizontal line
=========================

```
<div class="col-md-2"> 
            <hr style="width: 1px; height: 500px; background: black; border: none;" />  
 </div>
 ```
Round button
============

```
button {
background: black;
color: white;
padding:10px;
border-radius:25px;
}
```

Centre a div in the page
==========================
```
<div style="margin: 50 auto;">
```

align items in a div
======================
```
<div style="display:flex;align-items:center;">
```

centre text in a page
----------------------

```
body {
display: flex;
align-items: center;
justify-content:center;
}
```
 Fix to top
 ===========
 Fix an element to the top of the browser.
 
 ```
 .classfix {
 position:fixed;
 top:0;
 width:100%
 z-index:10;
 }
 ```
 
 Position text in bottom right of image
 =======================================
 ```
  <div class="container" style="position: relative;
  text-align: center;
  color: white;">
  <img id="myImage" src="/images/avatar.jpg" style="width:100%;height:400px"/>
  <div class="bottom-right" style="position: absolute; bottom: 8px; right: 16px;">Bottom Right</div>
</div>
```

Align two images side by side
==============================
```
<div class="container" id="imgWrapper" style="position: relative;text-align: center;color: white;">
    <div style="width:100%;">
    <img id="mainImage" src="/images/avatar.jpg" style="width:43.33%;;height:400px;float:left;padding:5px"/>
  <img id="myImage" src="/images/avatar.jpg" style="width:43.33%;;height:400px;float:left;padding:5px"/></div>
  <div class="bottom-right" style="position: absolute; bottom: 8px; right: 16px;">Bottom Right</div>
</div>

  <h2 style="clear:both;">Button events</h2>
```

Position div fixed in bottom right of browser
=======================================
```
position: fixed;
     bottom: 0;
     right: 0;
     z-index: 1;
```

z-index
=======
The z-index property specifies the stack order of an element.

An element with greater stack order is always in front of an element with a lower stack order.

Note: z-index only works on positioned elements (position: absolute, position: relative, position: fixed, or position: sticky) and flex items (elements that are direct children of display:flex elements).

Note: If two positioned elements overlap without a z-index specified, the element positioned last in the HTML code will be shown on top. 

Creating a page border effect
======================
using multiple box-shadow styles at different y-offsets.
```
 box-shadow: 0 1px 0 #bdbdbd, 0 2px 0 #fff, 0 3px 0 #bdbdbd, 0 4px 0 #fff, 0 5px 0 #bdbdbd, 0 0 0 1px #bdbdbd;
 
 ```

TUTORIALS
==========

Building a responsive grid CSS grid website layout from scratch (45mins 32)
https://www.youtube.com/watch?v=moBhzSC455o
