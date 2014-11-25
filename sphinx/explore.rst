Explore and Friends
====================

I frequently see new Vim users (and sometimes experienced Vim users) use the following
clunky workflow: open a file from the shell
with 'vim <some file>', make edits, save and quit,
then open another file with 'vim <some other file>', make edits, and so on. 

This is a bit kooky. Imagine doing this with any other text editor, for example
TextMate. Would you 'mate <some file>', make edits, save and exit, then 'mate
<some other file>'? No. That'd be goofy, right?

Fortunately, there are much more efficient ways to work with multiple files.
Some of those ways include: Vim buffers, Vim tabs, and the NERDTree plugin.
While those techniques are covered elsewhere in Black Belt Vim, 
this chapter teaches you to work with multiple files by using Explore and friends.

Explore (and related commands) enables you to navigate through the filesystem
on your computer and open a file or multiple files *without exiting
Vim*.

Let's try it.

Create a directory for experimenting. (In real life, you'll use your
project's actual directory, but for the sake of practice, we'll make
a practice directory)::

  $ mkdir exploretest
  $ cd exploretest

We'll need some files to play with and maybe a subdirectory too,
so let's make some::

  $ touch a b c
  $ mkdir d
  $ touch d/e

Time to fire up Vim!::

  $ vim

To begin exploring the filesystem, run :Explore::

  :Explore

You should now see::
  
  " ============================================================================
  " Netrw Directory Listing                                        (netrw v138)
  "   /home/btanaka/tmp/exploreandfriends
  "   Sorted by      name
  "   Sort sequence: [\/]$,\<core\%(\.\d\+\)\=\>,\.h$,\.c$,\.cpp$,*,\.o$,\.obj$,\.info$,\.swp$,\.bak$,\~$
  "   Quick Help: <F1>:help  -:go up dir  D:delete  R:rename  s:sort-by  x:exec
  " ============================================================================
  ../                                                                                                                                               
  d/
  a
  b
  c

Hey! There are our files and our subdirectory! 

[ TODO: keep going with example, then work in Sexplore Texplore ] 
