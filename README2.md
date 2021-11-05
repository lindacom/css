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

```
/* larger screen sizes */
@media(min-width: 768px) {
  main {
   /* width: 80%; */
  /*  margin: 0 auto; */
    flex-direction: row;
      }

      aside {
        flex: 0 0 10%;/* grow shrink and settings.  will grow 1/5th of page and no more proportional to other elements (main and aside)
            */  }

              .sidebar1 {
                order: -1; /* appears before the main item in large view */
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
