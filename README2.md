Flexbox and CSS grid
=======================
page structure
-------------

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
<header class="header">
    <article class="hero">
        <h1>My store</h1>
    </article>
</header> 

<main><article class="main"></article></main>


<aside class="sidebar1"></aside> 
<aside class="sidebar2"></aside>

<footer>
    <section class="frmfooter"></section></footer>

<body>
    </body>
    </html>
```
Styling
----------
```
/* Apply colours to elements  e.g background-color: var(--yellow); */

/* CSS Variables */

:root {
  --black: #242423;
--green: #3C6E71;
--white: #FFFFFF;
 --grey: #D9D9D9;
 --indigo: #284B63;
  --shadow: 0 1px 5px rgba(104, 104, 104, 0.8);
}
.header {
    height: 200px;
    padding: 20px;
    text-align: center;
   /* background-color: var(--green); */
    background-image: linear-gradient(to right, var(--indigo) , var(--grey));
    color: var(--white); 
    font-size: 30px;
    position: relative;
  }
  footer {
  background-color: var(--black); 
}
```
Flexbox and CSS grid
---------
Mobile first design

Large screen sizes:
```
/* larger screen sizes */
@media(min-width: 768px) {
  main {
      flex-direction: row;
      }

      aside {
        flex: 0 0 10%;  }

              .sidebar1 {
                order: -1; 
              }
  ```
  Mobile sizes:
 
 ```
 body { 
  background-color: var(--grey); 
  font-family: Arial,Helvetica Neue,Helvetica,sans-serif;

  display:flex; 
  min-height: 100vh; // vertical height
  flex-direction:column;
 } 
 ```
 hide in mobile view 
 ```
 aside {
 display:none; /* hidden on mobile */
  }
  ```
  
To images in a grid with caption text on top
============================================
```
/*container size - two columns*/
              .promo {
                display:grid;
                grid-template-columns: 450px 450px;
                grid-gap: 1rem;
                justify-content: center;
              }
              
/* two rows - for image and caption - total = the height of the image */
              figure {
                display: grid;
                grid-template-rows: 150px 100px;
              }

              #myImage {
height:250px;
width:450px;
              }

              #myImage1 {
               height:250px;
width:450px;

              }
```
CSS grid column layout:
three column layout used for products display 
```

.container { 
  max-width: 900px; 

 display:grid;
 grid-template-columns: repeat(3, 1fr); // three columns taking one fraction each 
 
 }
```
  two column container used on payment page 

```
 .pmtContainer { 
  max-width: 900px; 
  display:grid;
 grid-template-columns: 600px 300px // two column with set widths

 }
 ```
 Radio buttons panel using flexbox and css grid
 -------------------------------------------------
```
<main>
    <article class="main">
       <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed eu turpis euismod</p>
           <div class="shop-filters">              
        <div>
            <h2 class="shop-filters-title">Categories</h2>            
            <p><a class="shop-filters-sub-title" href="store.html">Clear categories</a></p></div>
            <div  class="radioBtns"> 
            <input class="category" type="radio" id="meat" name="food" value="meat">
            <label class="shop-filters-label" for="meat">Meat</label>
            <input class="category" type="radio" id="sweets" name="food" value="sweets"> <label
                for="sweets">Sweets</label>
            <input class="category" type="radio" id="fruit" name="food" value="fruit"> <label
                for="fruit">Fruit</label>
            <input class="category" type="radio" id="drinks" name="food" value="drinks"> <label
                for="drinks">Drinks</label>
            </div> 
            </div>
        </div>
    </article>
</main>

```
