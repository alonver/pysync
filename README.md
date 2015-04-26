#pysync

###What?
The point of this project is to enable easy synchronization between any 2 directories, as automatically as possible.

###Why?
Over time i realized i'm relying to much on ITunes to synchronize my music, because the concept is convenient. But 
then I thought "what happens when i replace my IPod with some other player?"
This is why i'm writing this, to allow the same level of fun synchronization, for non-apple products.

###TODO
* Write simple code that compares between directories:
  * comparing files with same name by data/hash (whichever is faster).
  * adding missing files to dest directory.
  * src directory may be hierarchical and the sync process flattens it.
  * printing files in dest but not in src and allowing basic actions (delete/ignore).
  * printing changed files and allowing basic actions (prefer this/other).
* support mp3 format for smarter comparison and diff display
* design a nice looking web page to manage the sync more interactively and more easily.
  * restful api, obviously
  * flask with Google's "material"
  * popping diffs and stuff like that.
* manage a db for faster, more efficient work. (TinyDB maybe?)
* make it run as a process and identify insertion of new media and then popping a question if a sync is required. 
* support more music formats (wav etc.)
* support non-music formats for more general usages.