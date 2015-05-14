MarkScripts
===========
Personal Bash functions for marking and returning to directories on unix system.

Description
-----------
These are a set of Bash functions that I like to carry around which 
give the ability to mark/delete/set/print a directory according to a
user-defined alias 

Additionally, I have some code that is non sequitur to the purpose of this repository.
I'm including them regardless.  One is a tea timer and the other a note taker.

Usage
-----
These scripts require that the directory '~/var' be created.  They are simply aliases and Bash functions
that need to either be sourced or included in the users .profile or .bashrc to function.

The scripts mark, return, and manage named directory marks.  The following is a brief
list of usage examples:

~> cd somedirectory
~/somedirectory> m some  # I'm calling this directory 'some'
~/somedirectory> cd ~/someother/place
~/someother/place> m other  # yet another mark
~/someother/place> g some   # go back to 'some'
~/somedirectory> k          # print all marks
~/var/mdirother   ~/someother/place
~/var/mdirsome    ~/somedirectory
~/somedirectory> d other    # deletes 'other'
~/somedirectory> k
~/var/mdirsome    ~/somedirectory

Additionally
------------
There are also two other things packaged here.  The alias 'notes' opens a file '~/notes.txt' with vi and the
function 'timer' is a small tea timer that I frequently use. :)
