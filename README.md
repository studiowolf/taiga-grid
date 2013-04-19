Taiga Grid
====================

Taiga Grid is a semantic fluid grid bases on SASS.

* Fluid & responsive
* Mobile first
* Semantic via Sass
* Customizable grid mixin
* Less nesting
* Relative sizing (em's)
* Modular with Smacss

Why Taiga Grid?
---------------------

Most grids are created for developers and are based on classes like span-6 or grid-12. They are predefined and not semantic. An example: let's say if I have a single aside element in my blog, I want to set the grid completely in the CSS and not in the HTML like aside.span-6. Scroll down to view the beautiful and easy solution.

Set up Taiga
---------------------

First, make sure you have Sass installed and that you are aware of the Sass basics like variables, nesting and mixins. The grid only has one .scss file which you need to compile with Sass. The grid.scss file exists of the following sections:

* Variables to set your basics like font-family, amount of columns and more
* The grid mixins which do the grid math
* Basic styles to normalize elements and set basics like fonts and colors on html and the body
* Layout rules which constructs the grid into an actual layout

Grid
---------------------

Taiga Grid is based on 48 columns (adjustable). That seems like a lot, but the difference is that margins are also expressed in columns. The example below will clear things up.

Let's say we want an article element to be half the width of our page. In the variables we set 48 columns for the whole grid, so this container needs to have 24 columns. The '1' at the end is the margin in columns on both sides. Note that this margin is subtracted from the width, so your content within the container will be 22 effective columns. If you want to have different margins on the left and right side, just separate it with a comma. That's it!

* Example with one column margin on both sides: `@include grid(24, 1)`
* Example with one column margin on the left and fice on the right: `@include grid(24, 1, 5)`

Thanks
---------------------
Taiga was inspired by these awesome people: Miller Medeiros, Paul Irish, Olav Bjørkøy and Jonathan Snook.
If you have any questions or suggestions, e-mail me at aljan@studiowolf.nl or ask it on github.

For more information: http://taigaboilerplate.com/taiga-grid