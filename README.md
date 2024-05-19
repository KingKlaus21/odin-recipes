# odin-recipes
Website for Recipe

In this project I was able to showcase my HTML skills.  I used commands such as "em" and "strong" to emphasize text, used "img" to put images of some delicious pastries, used "h1-h3" to express titles, "p" for paragraphs, "ul" and "ol" for lists, and other basic concepts such as linking to website pages and images.  I also made good use of the git commands.


Old CSS:


* {
    font-family: "Courier New", monospace;
}

h1,
#hometitle {
    margin: 20px;
    /*font-family: "Courier New", monospace;*/
    color: rgb(248, 220, 243);
    font-weight: bold;
    text-shadow: 5px 5px rgb(255, 0, 212);
    text-align: center;
    display: block;
}

#hometitle {
    font-size: 140px;
}

h1 {
    font-size: 80px;
}

h2 {
    font-size: 50px;
    color: white;
    text-shadow: 3px 2px rgb(255, 0, 212);
    text-align: center;   
}

h3 {
    font-size: 35px;
    color: white;
    text-align: left;

}

p {
    font-size: 30px;
    color: white;
    text-align: center;
    font-weight: 600;
    line-height: 1.3;
}

ul,
ol {
    font-size: 30px;
    color: white;
    text-align: left;
    font-weight: 600;
}

.ulIndent {
    padding-left: 24em;
    line-height: 1.2;
}
/* Padding left used to indent to move entire list to the center including dots */
/* Line height to change how close together lines of text are (called leading) */

.olIndent {
    padding-left: 3.5em;
    line-height: 1.2;
}

body {
    background-color: black;
    color: rgb(248, 220, 243);
}

img {
    height: auto;
    border: 3px solid;
    border-radius: 4px;
    border-color: rgb(255, 214, 246) rgb(255, 121, 233) rgb(255, 121, 233) rgb(255, 214, 246);
    position: absolute;
    top: 300px;
    left: 630px;
}

#OdinCakeImg {
    width: 400px;
    left: 300px;
}

#OdinCupcakeImg {
    width: 265px;
    left: 770px;
}

#OdinDonutImg {
    width: 490px;
    left: 1100px;
}

.pagePos {
    position: relative;
    top: 60px;
}

.pagePos.CupcakePos {
    left: 730px;
}

.pagePos.DonutEdit {
    width: 770px;
    left: 560px;
}

#ReturnHome {
    position: fixed;
    top: 10px;
    left: 10px;
    border: 0px solid;
    width: 40px;
}

span {
    color: rgb(238, 255, 0);
    font-size: 20px;
}

.Emoji {
    font-size: 30px;
    font-weight: bolder;
    /* Used for caution signs on cupcake disclaimer */
}




 -------------------------------------------
                Odin Cake
    ___________
   |           |    Description: Blah
   |           |    blah blah blah                       This looks good
   |           |    blah blah blah
   -------------

                Ingredients

        Wet:                    Dry:                     
      *Item                     *Item                    Needs work
      *Item                     *Item

               Instructions

    1. Blah blah blah blah blah blah blah
    2. Blah blah blah blah blah blah blah                Might be okay
    3. Blah Blah Blah blah blah blah blah


                   Home                                  Remeber to make this larger
 -------------------------------------------- 


squish the page towards middle with auto margins
center everything and stick stuff in boxes





Header in case you mess up bad:

HTML:

<!-- <header class="header">
        <!-- odin desserts should be 729px from either side (smaller on left) -->
        <ul class="left-links">
          <li><a href="https://www.youtube.com/watch?v=PbTjAVDqdXU">ASMR</a></li>
          <!-- do <a href> -->
          <!--Make drop down-->
          <li><a href="#">Shows</a></li>
        </ul>
        <h1 class="hometitle"><a href='../index.html'>Odin Desserts</a></h1>
        <!-- MAKE THIS RETURN HOME -->
        <ul class="right-links">
          <li><a href="#">Sweepstakes</a></li>
          <li><a href="#">Chefs</a></li>
        </ul>
      </header> -->

CSS:

.header {
    display: flex;
    flex-direction: row;
    align-items: center;
    background: #2b282b;
    height: 80px;
    box-shadow: 0 0 3px 2px rgb(75, 73, 73);
    
    /* make height larger */
    /* add subtle border design */
}

.left-links {
    margin-right: auto;
    flex-grow: 1;
}

.right-links {
    margin-left: auto;
    flex-grow: 1;
}

.left-links li:nth-child(n+2){
    /* 1 is first in list and n starts at 0 so order goes
       x     0    1     2     3
       y     2    3     4     5*/
    padding-left: 5%;
    display: flex;
    flex-direction: row;
    margin-right: auto;
    margin-left: auto;
    /* both of these are used so the list items
       could spread out evenly inside the parent,
       keep the end items from moving, and allow
       the page to remain reactive */
    
}

.right-links li:nth-last-child(n+2){
    /*  */
    padding-right: 5%;
    display: flex;
    flex-direction: row;
    margin-left: auto;
    margin-right: auto;
}



        <ul class="left-links">
          <li><a href="https://www.youtube.com/watch?v=PbTjAVDqdXU">ASMR</a></li>
          <!-- do <a href> -->
          <!--Make drop down-->
          <li><a href="#">Shows</a></li>
        </ul>
        <h1 class="hometitle"><a href='../index.html'>Odin Desserts</a></h1>
        <!-- MAKE THIS RETURN HOME -->
        <ul class="right-links">
          <li><a href="#">Sweepstakes</a></li>
          <li><a href="#">Chefs</a></li>
        </ul>




New left/right thing

.left-links {
    padding-right: 5%;
    display: flex;
    flex-direction: row;
    /* justify-self: flex-start; */
    /* margin-left: auto;
    margin-right: auto; */

}

.right-links {
    padding-left: 5%;
    display: flex;
    flex-direction: row;
    /* justify-self: flex-end; */
    /* justify-content: space-between;
    width: inherit; */
}