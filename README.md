Created by
==========

Andreas Politz

Script type
===========

utility

Description
===========

*ShowMarks*

Give a visual aid to navigate marks, by displaying them as signs
(obviously needs the +signs feature).

Commands
--------

    :DoShowMarks
       show marks for current buffer
    :DoShowMarks!
       show marks for all buffers
    :NoShowMarks
       disable it for current buffer
    :NoShowMarks!
       disable it for all buffers

    :[count]ShowMarksOnce
       Display marks for [count] Cursorhold
       events. Mostly for mapping it like :
       nnoremap ` :ShowMarksOnce<cr>`

    :[count]PreviewMarks
       Display marks of current buffer in pvw.
       Like ':marks', but at the top of the window ;-).
       [count] is the same as above.

Variables
---------

let g:showmarks_marks = "abcdef...."
   the marks you want to have displayed.
hlShowMarks
   the highlight color

I suggest you lower the value of 'updatetime'.
