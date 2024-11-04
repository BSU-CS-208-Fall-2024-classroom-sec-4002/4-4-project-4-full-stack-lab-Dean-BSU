# Retrospective

- name: Dean Cunningham
- email: deancunningham@u.boisestate.edu

## Experience

I went into this project a bit confused and disoriented, however all turned out to be ok in the end. Setting up the layout of the page in pug was not an issue, but I was confused how to communicate data between the pug file and server.js. I started working through the TO-DOS, firstly making it so my page could render, and then figuring out a setup to allow for tasks to be stored in javascript and sent back to the pug. Once things stopped crashing (debugging solved via notes and asking for help) I was able to implement adding tasks next, tasks were added starting at index 0 and counting upward. I thought this was implemented properly, so I moved on to delete. Upon moving onto delete, I realized that adding was not in fact implemented correctly (on the client-side). Previously, my local tasks variable in the js file stored just the task, as I assumed auto-increment would take care of the id for me. However, this caused it to become offsync from the index of the page's ul. To fix this, I made my tasks variable store both an array of tasks and an array of ids, which should always correspond to each other. Because of this, removing tasks now properly updates the id and index identically and there are no longer issues while adding and removing elements. For the CSS, I remembered the teachings of a wise man from Australia I know, "when you want to make a website really ugly, use a fireworks png with a hard to read font color".

## Known issues or Bugs

None

## Sources used

https://www.tutorialspoint.com/sqlite/sqlite_delete_query.htm - Used to double check my usage of the DELETE function during troubleshooting.
https://glassbeach.band/archive/lp1/bear1 - Facebook page
