# superbowlsquares
This is designed as a static html page which uses javascript's localstorage feature to provide a automated solution on generating super bowl squares in your next event!  


"PRINT" aligned in top right of the page's nav.  When clicked, we will open the print dialog with default  selection for "Save AS PDF".

"Create Board" button issues modal warning that memory will be lost if board is currently in session. Confirm "Continue" with a red danger.  Or include "cancel" secondary theme to return back to page.

Board grid is saved as stringified json in javascript localstorage.  { a:{ 1,2,3,4,5,6,7,8,9,10,11}, b:{ 1,2,3,4,5,6,7,8,9,10,11}, c:{ 1,2,3,4,5,6,7,8,9,10,11}, d:{ 1,2,3,4,5,6,7,8,9,10,11}, e:{ 1,2,3,4,5,6,7,8,9,10,11}, f:{ 1,2,3,4,5,6,7,8,9,10,11}, g:{ 1,2,3,4,5,6,7,8,9,10,11}, h:{ 1,2,3,4,5,6,7,8,9,10,11}, i:{ 1,2,3,4,5,6,7,8,9,10,11}, j:{ 1,2,3,4,5,6,7,8,9,10,11},k:{ 1,2,3,4,5,6,7,8,9,10,11}}

Where letters are columns and number keys are rows.  The 0-9 value assignments are assigned to row 1 of column b through rows column k for the away team.   The 0-9 value assignments are assigned to all 10 column a rows for the home team. 


When "Purchase Squares" is clicked, i want modal to enter quantity and enter initials.  On submit, these initials are assigned to our grid for column b to column k and for row 2 to row 11.  Only set columns row value if its not already assigned a non empty string.

when i purchase squares and assign initials to squares where initials are not already assigned, I do not want to change the value of any rows in column "a" of my grid. I also never want to change the value of row 1 on any columns of my grid. i.e.. a.1, b.1, c.1, ...., k.1.

When the square is purchased, i want to randomly choose any of the other squares in this grid where initials arent already assigned.
 
