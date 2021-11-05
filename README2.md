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
