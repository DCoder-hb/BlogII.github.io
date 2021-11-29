# BlogII.github.io
First blog page
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- -------- -------- -->
    <!-- ----x--- ---x---- -->
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>H. H. Bonaparte: Blog</title>
    <style>
        /* used to set root font-size to 10 px */
        /* for easier calculation of rem sizes */
        html {font-size: 62,5%;}
        
        body {
            font-family: candara, optima, verdana;
            font-size: 1.25rem;
            background: #E6DADA;  /* fallback for old browsers */
            background: -webkit-linear-gradient(to right, #274046, #E6DADA);  /* Chrome 10-25, Safari 5.1-6 */
            background: linear-gradient(to right, #274046, #E6DADA); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
            
        }

        h1,
        h2,
        h3,
        h4,
        h5,
        h6 {
	        clear: both;
            font-family: 'Patua One', serif;
            letter-spacing: 2px;
        }

        h1 {
            font-size: 2.5rem;
            color: #00161a;
            text-align: center;
        }

        h2 {
            font-size: 1.6rem;
            color: #007489;
        }

        h3 {
            font-size: 1.5rem;
            color: #00161a;
            text-align: center;
        }

        p {
            margin-bottom: 1.5em;
            color: #00161a;
            text-align: left;
        }
        
        /*  Comment  */
        /*  ---------- Comment ----------   */
        /*  ----x----- Comment -----x----   */

        /* --------------- Navigation --------------- */ 

        /* Large */
        .navigation {
            /*  Flex items are placed in a horizontal row  */
            display: flex;
            /*  It flows to the right until it can't do so anymore, at which point it makes a new row  */
            flex-flow: row wrap;
            /* Aligns items to the end line on main-axis */
            justify-content: flex-end;
            /*  removes dots  */
            list-style: none;
            margin: 0; 
            background: #E6DADA;  /* fallback for old browsers */
            background: -webkit-linear-gradient(to right, #274046, #E6DADA);  /* Chrome 10-25, Safari 5.1-6 */
            background: linear-gradient(to right, #274046, #E6DADA); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

        }

        /* Link Styles */
        .navigation a {
            text-decoration: none;
            display: block;
            padding: 1em;
            color: #00161a;
        }


        /* Link hover effect */
        .navigation a:hover {
            background: #1565C0;
            color: white;
        }


        /* Medium screens */
        @media all and (max-width: 800px) {
            .navigation {
                /* When on medium sized screens, to center it by evenly distributing empty space around items */
                justify-content: space-around;
            }
        }


        /* Small screens */
        @media all and (max-width: 600px) {
            .navigation {
             /* On small screens, no longer use row direction but column */
                flex-flow: column wrap;
                padding: 0;
            }

            .navigation a { 
                text-align: center; 
                padding: 10px;
                border-top: 1px solid rgba(255, 255, 255,0.3); 
                border-bottom: 1px solid rgba(0, 0, 0, 0.1); 
            }

            .navigation li:last-of-type a {
                border-bottom: none;
            }
        }


/* -------x------- Navigation -------x------- */
        
        /*  ---------- Blog Card ----------   */
        
        img {
            /*  to take up as much horizontalas they can  */
            display: block;
            border: 0;
            /*  image don't exceed container width  */
            /*  
                if width is % and height = auto the image is responsive  
            */
            width: 100%;
            height: auto;
            
        }

        #hhb {
            width: 500px;
            margin: auto;
        }

        .main p {
            color: #00161a;
        }
              
        .card {
            background: white;
            margin-bottom: 2em;
        }
        
        .card a {
            color: black;
            text-decoration: none;
        }
        
        .card a:hover {
            box-shadow: 3px 3px 8px hsl(0, 0, 80%);
        }
        
        .card-content {
            padding: 1.4rem;
        }
        
        .card-content h2 {
            margin-top: 0;
            margin-bottom: 0.5em;
        }
        
        .card-content p {
            font-size: 80%;
        }
        
        
        
        
        /*  ---------- Media Queries ----------   */
        
        
        /* 
            specified breakpoint will ensure that content is displayed properly on all screens.
        */
    
       /* Flexbox stuff */

        /* 
            min-width 640px, mobile-only styles, use when QAing mobile issues
        */
        @media screen and (min-width: 40em) {
            .cards {
                /*  Flex items are placed in a horizontal row  */
                display: flex;
                /*  make flex items wrap underneath each other  */
                flex-wrap: wrap;
                /*  align flex items with even space  */
                justify-content: space-between;
            }

             .card {
                flex: 0 1 calc(50% - 1em);
            }
        }

        /* min-width 960 */
        @media screen and (min-width: 60em) {

            .card {
                /*  
                    browser will grab 25% of space and will remove 1em from it to make the cards slightly smaller
                    the 1em is distributed evenly between items
                */
                 flex: 0 1 calc(25% - 1em);
            }
        }

        /* Flexbox stuff oneven pages */
        /* Flexbox stuff */

        .cards {
            display: flex;
            flex-wrap: wrap;
        }

        .card {
             flex: 1 0 500px;
             box-sizing: border-box;
             margin: 1rem .25em;
        }

        @media screen and (min-width: 40em) {
            .card {
                 max-width: calc(50% -  1em);
            }
        }

        @media screen and (min-width: 60em) {
            .card {
                max-width: calc(25% - 1em);
            }
        }

        .centered {
              margin: 0 auto;
              padding: 0 1em;
        }

        @media screen and (min-width: 52em) {
             .centered {
                  max-width: 52em;
                }
        }
        
        /*  ----x----- Media Queries -----x----   */
            
        
        
        
        /*  ----x----- Blog Card -----x----   */


        /*  ---------- Footer ----------   */


        .footer {
            /*  Flex items are placed in a horizontal row  */
            display: block;
            /*  It flows to the right until it can't do so anymore, at which point it makes a new row  */
            flex-flow: row wrap;
            text-align: center;
            background: #E6DADA;  /* fallback for old browsers */
            background: -webkit-linear-gradient(to right, #274046, #E6DADA);  /* Chrome 10-25, Safari 5.1-6 */
            background: linear-gradient(to right, #274046, #E6DADA); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
            justify-content: center;
            clear: both;
        }


        /*  ----x----- Footer -----x----   */
            
        </style>
        
        <body>
        <!-- ---------- Comment ---------- -->
        <!-- ----x----- Comment -----x---- -->

        <!-- ---------- Header ---------- -->


        <header class="header">
            <!-- --------- Navigation ------------ -->
            <div>
                <ul class="navigation">
                    <li><a href="index.html">Home</a></li>
                    <li><a href="gallery.html">Gallery</a></li>
                    <li><a href="#">Archives</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </div>
            <!-- ----x---- Navigation ------x----- -->
          </header>


        <!-- ----x----- Header -----x---- -->
        
        <!-- ---------- Blog Card ---------- -->
        <div class="main-area">
            <div class="centered" id="hhb"></div>
            <h1>Hugo's blog</h1>

             

             <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6c/Graphics_Designer.jpg/800px-Graphics_Designer.jpg" alt="Designer">

             <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga error corrupti, consectetur tempora excepturi esse quidem iste explicabo eum neque et quo dolor id ullam odit sit quis illo nemo aliquam omnis repellat odio ut ea. Natus quia iusto suscipit!</p>
            </div>
             <div class="centered">

                <section class="cards">

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Today i started with coding my first blog page. As a startpoint to get better in making pages.</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Content for card one</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card one -->

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card two  -->

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card three -->

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Content for card one</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card four  -->
                </section>
                
                <section class="cards">

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Content for card one</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card one -->

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card two  -->

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card three -->

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Content for card one</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card four  -->

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card three -->

                    <article class="card">
                        <a href="#">
                            <p class="thumbnail">
                                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Ethan_Marcotte_-_Responsive_webdesign.jpg/800px-Ethan_Marcotte_-_Responsive_webdesign.jpg" alt="responsive webdesign"> 
                            </p>
                            <div class="card-content">
                            <h2>First Post</h2>
                            <p>Not shure what to say. But this is gonna be the first. In many more to come...</p>
                            <p>Content for card one</p>
                            </div>
                        </a>
                        
                    </article><!-- Content for card four  -->
                    
                </section>
                
            </div>
         
        </div>    
        <!-- ----x----- Blog Card -----x---- --> 
        
        <div class="centered">
            <section class="contact">

            </section>
        </div>
        
        
        
        
        <h1>___'s blog</h1>

        <h3>Contents</h3>
        <ul>
            <li>First post!</li>
        </ul>
        
        <h2>First post</h2>
        <h6>Posted on some date in some year</h6>
        
        <p>Something excited happened.</p>

        <footer class="footer">
            <div class="footer">Made by Napo</div>
        </footer>
    
</body>
</html>
