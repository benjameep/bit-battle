# BitBattle
Create your own bitbot to battle against others

## Week 1 - *Set up enviroment*
- Github
- Webpack
- ejs
- babel
- client-side libraries (d3-zoom)

## Week 3 - *Create HTML/CSS templates*
#### Nav Bar
Need a nav across all pages to make page navigation
easy. Nav Bar should include 3 icons for build page,
test page, and another for a dropdown menu of settings.
#### Rule Editor
The 3x3 grid where the user creates the rules by
toggling each cell to the status that cell should
be in for that rule to be activated. 
#### Test Enviorment
Have the canvas take up the page, with the nav bar
across the top. And a couple buttons across the bottom,
for step-back, play, step-forward, and reset.

### Week 6 - *Add functionality to Bot creator*
#### Rule Builder
Give the rule builder functional. With the cells togglable,
maybe even possible to drag between multiple cells to copy
and paste
#### Load Rule
Able to select a rule previously made in a scrollable list,
which will load the rule into the rule builder. At the bottom
of the scrollable list should be a create new rule button.
#### Auto-Save
Have modifications made to the rules automatically save to
the rule library.
#### Make rules re-orderable, deletable
Rules need to be re-orderable because their order is important
to their prioritization. 

### Week 9 - *Rust Algorithm*
#### Learn Rust
I have never programmed in rust before, only gone through their
documentation a little bit. So I need to familiarize my self
with how to program in Rust.
#### Create rule search algorithm in rust
I have created the search algorithm in javascript, but the assumption
is that it would never be able to run fast enough in javascript. So
I need to figure out how to recreate that algorithm in Rust
#### Manage frame updating in Rust
Rust needs to store the "frames" of the game so that it can calculate
the next one. It also needs to store data previous frames inorder
for the 'step-backward' button to have functionality.

### Week 11 - *Canvas Enviroment*
#### Create a cell grid API
Updating a cell grid gets messy fast as I have learned in previous
projects. So care needs to be taken to make the Grid and Cell
Objects as clean as possible. To avoid a lot of messy math converting
from the cell position to pixel position and such.
#### Make grid pannable and zoomable (probably with d3-zoom)
I have implemented pan and zoom before, but it is awful. You have to 
save the postion of the origin temporarily set the origin to the top-left
corner of the screen the scale the cell size, then set the origin in the
new calculated postion. D3-zoom will handle that messy math for me, and
also handle the multi-touch zoom.
#### Add Grid drawability combatible with Rust
Make the Grid api accessable to the Rust side, and of
course hook the Rust side up to those end points. So that
the rust algorithm can now directly draw to the grid.

### Week 13 - *Finish Off*
#### Connect all the components together
Connect all of the buttons to the endpoints of the Rust side,
and page navigation, and whatever else needs to be connected up.
#### Get Game running
Finish off whatever needs to happen to get the game is running.
