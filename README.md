<html>
 <head>
  <body>
 <body>
        <span id="width" class="width-container"></span>
        <header class="wrapper">
            <a href="#" class="logo">tastybites</a>
            <nav>
                <ul>
                    <li><a href="#">home</a></li>
                    <li><a href="#">about</a></li>
                    <li><a href="#">contact</a></li>
                </ul>
            </nav>
        </header>
        
        <div class="hero-left wrapper">
            <h1>Absolutely Tasty Bites</h1>
            <p>Get all of the best food without tasting their nastiness</p>
            <a href="#" class="cta-btn">Download app</a>
        </div>
        <img src="https://i.imgur.com/8bWsRYr.jpg">
        
        <section class="wrapper">
            <ul class="testimonials">
                <li>
                    <blockquote>
                        <p>"Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor"</p>
                        <footer>- John Doe</footer>
                    </blockquote>
                </li>
                <li>
                    <blockquote>
                        <p>"Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor"</p>
                        <footer>- John Doe</footer>
                    </blockquote>
                </li>
                <li>
                    <blockquote>
                        <p>"Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor"</p>
                        <footer>- John Doe</footer>
                    </blockquote>
                </li>
            </ul>
        </section>
        <script src="index.js"></script>
    </body>
  </body>

 <script>
let width = document.getElementById('width');
var onresize = function() {
   //your code here
   //this is just an example
   width.innerText = document.body.clientWidth;
   width.classList.add('display-width');
   setTimeout(() => {
       width.classList.remove('display-width');
   }, 2000)
}
window.addEventListener("resize", onresize);

    </script>


   <style>
@import url('https://fonts.googleapis.com/css?family=Nunito:400,700&display=swap');

html, body {
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Nunito', sans-serif;
}

.wrapper {
    padding: 1em;
}

a {
    text-decoration: none;
}

img {
    width: 100%;
    position: absolute;
    z-index: -1;
}

a.logo {
    color: #C500FF;
    font-weight: bold;
    font-size: 1.2em;
}

ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}
 nav ul {
     display: flex;
     margin-top: 1em;
 }
 
 nav li {
     margin-right: .5em;
 }
 
 nav li a {
     color: black;
     font-weight: bold;
     padding: .3em .7em;
     background-color: #E6E6E6;
     border-radius: 1em;
 }
 
 .hero-left {
     text-align: center;
 }
 
 h1 {
     font-size: 2.5em;
     width: 80%;
     margin: 1.5em auto 0;
 }
 
 .hero-left p {
     font-size: 1.2em;
     width: 80%;
     margin: 1em auto;
 }
 
 a.cta-btn {
     color: white;
     background: #C500FF;
     padding: .8em 1.5em;
     border-radius: 2em;
     font-weight: bold;
     margin: 1em 0 3em;
     display: inline-block;
 }
 
 ul.testimonials {
     margin-top: 3em;
 }
 
 ul.testimonials li {
     background: white;
     padding: 2em;
     margin-bottom: 1em;
     text-align: center;
     box-shadow: 10px 10px 18px 0px rgba(0,0,0,.09);
 }
 
 blockquote, blockquote p {
     margin: 0;
 }
 footer {
     font-weight: bold;
     display: block;
     margin-top: 1em;
 }
 blockquote p {
     line-height: 1.4em;
 }
 
 @media (min-width: 390px) {
     header {
         display: flex;
         justify-content: space-between;
     }
     nav ul {
         margin-top: .2em;
     }
     nav ul li:nth-of-type(3) {
         margin-right: 0;
     }
 }
 
@media (min-width: 600px) {
     
     ul.testimonials {
         display: grid;
         grid-template-columns: repeat(2,auto);
         grid-template-rows: repeat(2,auto);
         grid-gap: 1em;
     }
     ul.testimonials li {
         margin: 0;
     }
     
     ul.testimonials li:nth-of-type(3) {
         grid-area: 2 / 1 / 2 / 3;
     }
     
     img {
         clip-path: polygon(0 0, 100% 0, 100% 33%, 0 33%);
     }
     
 }
 
 /*

- White Space
- Color 
- Contrast 
- Scale
- Alignment
- Typography
- Visual Hierarchy

*/

/* For the width display, ignore this */

.width-container {
    display: none;
}

.display-width {
    display: block;
    position: absolute;
    right: 0;
    top: 0;
    background-color: #E6E6E6;
    padding: .3em;
    font-size: .85em;
}
 @media (min-width: 1000px) {
     
     .hero-left {
         text-align: left;
         width: 30%;
         margin-left: 4em;
     }
     
     h1, .hero-left p {
         width: 100%;
     }
     
     img {
         top: 0;
         right: 0;
          clip-path: none;
     }
h1 {
         font-size: 3rem;
     }
     ul.testimonials {
         display: flex;
     }
     ul.testimonials  li {
         margin-right: 1em;
     }
ul.testimonials li:nth-of-type(3) {
         margin-right: 0;
     }

    </style>
    
  </head>
</html>
