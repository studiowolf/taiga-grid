Taiga Grid
====================

Taiga Grid is a semantic fluid grid bases on SASS.

* Basic HTML5/CSS3 Grid;
* Using SASS;
* Semantic fluid grid;
* Responsive, using em units;
* Everything is border-box;

Website is http://taigaboilerplate.com or Github https://github.com/AljanScholtens/Taiga

Set up Taiga
---------------------

You don't need a lot, just install SASS and you're almost ready to go.

* Install SASS, read the instructions on http://sass-lang.com/
* Watch the stylesheet in the root of Taiga with the following command: sass --watch stylesheets:stylesheets --style compressed
* Check types.html in the root to see a simple demo

You can find a few variables in styles.scss that sets the basics of your web application or website. 
Mixins can be found in the _mixins.scss and are very simple to keep them flexible.

Grid
---------------------

Taiga has a semantic fluid grid based on columns. Standard you have 48 columns (adjustable).
It works with percentages and em units to make it fluid and more responsive.

Remember, Taiga works with box-sizing: border-box, this means you don't have to nest several block elements to get your padding right and border right. 
Just change your padding on your block element and you don't have to change the width.

* Use '@include grid(12, 2)' on your article or section to make a column. 
* The first unit (12) is the column count.
* The second unit (2) is the margin on both sides.
* The margin will be automatically subtracted from the column count, so you don't have to recalculate the column width if you change your margin.
* To set different margins on both sides use '@include grid(12, 2, 3)'.
* You can also use negative margins.

Thanks
---------------------
Taiga was inspired by these awesome people: Miller Medeiros, Paul Irish, Olav Bjorkoy and Emil Loer.
If you have any questions or suggestions, e-mail me at aljan@studiowolf.nl or ask it on github. 