CSS Grid Layout
==================
Hello, my name is Anna and the theme of my presentation is CSS Grid Layout

CSS Grid Layout (aka "Grid"), is a two-dimensional grid-based layout system that is able to completely change the way to design user interfaces. CSS has always been used to lay out our web pages, but it's never done a very good job of it. At the beginning we used ***tables***, then ***floats***, ***positioning and inline-block***, but all of these methods were the reason of hacking and left out a lot of important functionality behind (vertical centering, for example). ***Flexbox*** helped out, but it's intended for simpler one-dimensional layouts, not complex two-dimensional ones and Flexbox and Grid actually work very well together. Grid is the first CSS module created specifically to solve the layout problems we've all been hacking our way around for as long as we've been making websites.

I don't know how good my presentation language is, but before diving into the concepts of Grid it's important to understand this language, this ***terminology***. Since the terms used here are all conceptually similar, it's easy to confuse them with one another if you don't first memorize their meanings defined by the Grid specification. But don't worry, there is not so many here.

### Grid Container
This is the element on which display: grid is applied. It's the direct parent of all the grid items. In this example container is the grid container.

### Grid Item
The children of the grid container. Here the item elements are grid items, but sub-item isn't.
 
### Grid Line
The dividing lines that make up the structure of the grid. They can be vertical ("column grid lines") or horizontal ("row grid lines") and reside on other side of a row or column. Here the blue line is an example of a column grid line.

### Grid Track
The space between two boundary grid lines. You can think of them like the columns or rows of the grid. Here's the grid track between the second and third column grid lines.

### Grid Cell
The space between two boundary row and two boundary column grid lines. It's a single "unit" of the grid. Here's the grid cell between the lines of the second and third rows and lines of columns three and four.

### Grid Area
The total space surrounded by four grid lines. A grid area may be comprised of any number of grid cells. Here's the grid area between row grid lines one and three, and column grid lines one and two.

The theory is interesting but without practice it is a dead! Let's take an ***example***. I am a civil engineer, so let's try using Grid to solve the problem of a simple interior designer. Let pretend that our room is a Grid Container where we will add the Grid Lines. The fr module allows to create flexible grids. It is a part of the available space in the grid container (it works like some Flexbox values). Here is the result.

Let's install a door and a window in our room- Grid Container first.
What else is needed? A desk for a highly qualified Frontend-developer, a cupboarde and a chest of drawers work in order to store all the necessary things for comfortable program development, and a sofa, where you can discuss Frontend-development innovations with programmer friends. And a soft carpet in the center of the room.

Using justify-items and align-items and colors we create beautiful titles for elements of our interior.
Everything looks good, right? But engineers not just only build, they also ***break***. What can break the layout on Grids?

Frontend- developers are always worried by the sudden appearance of a horizontal scrollbar on the site. And what if the scroll due to the order? It turns out that any element with overflow-x breaks the grid. Usually **overflow-x: auto** handles solving this problem. But not at this time. Another idea - all sorts of tricks with **overflow: hidden**, but also not. The fact is that the default for grid elements is min-width: auto and their size is automatically set to the content in them. It sets their min-width to the width of the overflow block. Therefore to fix it you can go up the DOM tree to the grid element and null it to **min-width**.
Due to this the dimensions of the grid element with the overflow of content will be set correctly.

The information heard and seen will not be enough to own the Grid at a professional level of course. Because I propose several of simulators that will raise your skill further.

***CSS Grid Playground*** - simple text-based tool;

***CSS Grid Cheat Sheet*** - bright and dynamic;

***CSS Grid Template Builder*** - 'hybrid' of visual and textual interfaces;

And of course funny ***Grid Garden***.

They are all cool and helpful and the choice is yours! 

This is not the end, just the last slide.
Have a nice day and thank you for your attention.
