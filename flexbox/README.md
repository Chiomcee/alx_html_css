# Flexbox

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

What is Flexbox?
How to convert float positioning to a flex display
How to horizontally and vertically align elements using Flexbox
The difference between the main and cross axes
Properties that work on flex elements vs flex container
Shorthands for flex
How to create a new page with flex in mind
Files
Required images for your HTML files
Download the images linked in the CSS Advanced and place them into an images directory at the root of the project.

HTML starter file
CSS starter file

## Tasks
0. Add display flex
mandatory
Use the starter HTML and CSS files from this task to task 7. Copy the contents of the starter files into the files that you need to produce and make the necessary changes according to the task description.

When using display: flex; on a container, all direct children become flex-items (and no more inline or block elements).

With display flex, margins are not collapsing as they would with block items. Also remember that flexbox is 1-dimensional system (vs CSS Grid which is a 2 dimensional system)

In the /* Grid section within your CSS

Add a selector for the row class
Property: display, Value: flex
=> Now, all children from the row class are flex items

Entirely remove the row::after declaration
Remove the float: left inside [class*='col-']
=> All elements should appear same than before using the float

Repo:

GitHub repository: alx_html_css
Directory: flexbox
File: 0-index.html, 0-styles.css
  
0/4 pts
1. Add new classes on sections
mandatory
Using the files from the previous task as the base for this task:

In the outermost section tag for services

Add the class section-services
In the outermost section tag for works

Add the class section-works
In the outermost section tag for about

Add the class section-about-us
In the outermost section tag for latest_news

Add the class section-latest-news
In the outermost section tag for testimonial

Add the class section-testimonial
In the outermost section tag for contact

Add the class section-contact
Repo:

GitHub repository: alx_html_css
Directory: flexbox
File: 1-index.html, 1-styles.css
  
0/6 pts
2. Reverse order Latest news cards
mandatory
Using the files from the previous task for this task:

The flex-direction property says how flex items are placed on the main axis and their direction (normal or reversed).

flex-direction is sometimes used when doing responsive design. Some elements may appear better when they are in column mode on mobile and row when on desktop.

row-reverse and column-reverse should be used in specific situation. The visual order of elements should be the same visually and in the HTML code. Refer to flex-direction - CSS: Cascading Style Sheets | MDN for more information

In your CSS file:

Before /*** 4. CARD ***/, add a new comment: /* Section Latest news ============================= */

Under that comment section, target the row class inside section-latest-news class

Property: flex-direction, Value: row-reverse
The Latest news should appear in a reverse order.

Repo:

GitHub repository: alx_html_css
Directory: flexbox
File: 2-index.html, 2-styles.css
  
0/3 pts
3. Simplify services list
mandatory
Using the files from the previous task for this task:

flex-wrap is a property that can force the flex items to be in one or multiple lines. Learn more about it here.

In the Services section of 3-index.html, remove the second ul and put the 3 lielements under the first ul

Now, in your CSS file, before /*** 4. CARD ***/, add a new comment: /* Section SERVICES ============================= */

Under that comment section, add a new selector targeting the row class inside the section-services class

Property: flex-wrap, Value: wrap
Repo:

GitHub repository: alx_html_css
Directory: flexbox
File: 3-index.html, 3-styles.css
  
0/3 pts
4. Playing around with the spacing between flex service items
mandatory
Using the files from the previous task for this task:

In 4-styles.css file, within the Grid section

In .col-1-3 selector

Replace the current width with calc((100% / 3) - 2rem)
In .col-1-2 selector

Replace the current width with calc((100% / 2) - 2rem)
In [class*='col-']

Remove the padding declaration
Set Property: margin to 1rem
In ul.row declaration

Replace the current margin with -1rem
Repo:

GitHub repository: alx_html_css
Directory: flexbox
File: 4-index.html, 4-styles.css
  
0/5 pts
5. Flexify the header
mandatory
Using the files from the previous task for this task:

In your 5-index.html file, inside the Header section

Wrap the div with class header-logo and the div with class navbar-menu with a div that has header-container as a class
In your 5-styles.css file,

Inside the /* Header section
Add a selector for the header-container class
Property: display, Value: flex
Property: justify-content, Value: space-between
Remove header-logo and header-logo a rules
Remove the navbar-menu rule

In the variables section

Remove
header-logo-position
header-logo-link-display
header-logo-link-position
header-logo-link-top
header-logo-link-left
Repo:

GitHub repository: alx_html_css
Directory: flexbox
File: 5-index.html, 5-styles.css
  
0/11 pts
6. Flexify the navbar
mandatory
Using the files from the previous task for this task:

in 6-styles.css, inside the /* Navbarsection

In the nav class selector
Property: display, Value: flex
Inside the .nav .nav-item selector, remove the display declaration
Target .nav-item + .nav-item inside nav class
Move the margin declaration from .nav .nav-item inside the new selector.
In the variables section
Change the value of the variable nav-item-margin to be 0 0 0 2rem
Repo:

GitHub repository: alx_html_css
Directory: flexbox
File: 6-index.html, 6-styles.css
  
0/6 pts
7. Align center logo and navbar
mandatory
Using the files from the previous task for this task:

In 7-styles.css, inside the /* Header section, in the header-container class selector, set the property align-items to center

Repo:

GitHub repository: alx_html_css
Directory: flexbox
File: 7-index.html, 7-styles.css