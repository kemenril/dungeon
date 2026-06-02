# Dungeon
A port to new-ish GFortran of the old Dungeon game, originally created at the MIT Laboratory. This was the basis for Infocom's Zork. 

### Provenance
This is a port to GFortran of the old MIT Dungeon game, which I did around the end of 2010, uploaded to a web server on the internet around January 2011, and left for a while.  It was based on a distribution of Dungeon 3.2 which I found in an archive somewhere.  The original readme files, which will be included (along with the old binaries, for reasons of completeness), say that it was Robert Supnik's V3.2B ported to MS-DOS by David Kinder, around 2003, based on some earlier work by Volker Blasius.  Robert targeted G77 under MS-DOS.

I took that code, and ported it to GFortran under RHEL 5.  A number of minor changes were required to make it go, at the time.  More have been added recently, in order to bring things in line with the Fortran 2018 standard.  The newest code now builds without changes on EL9, and probably anything else with an appropriate GFortran.

### Installation
There really isn't any.  The executable expects two files in the current directory: *dindx* and *dtext*, which contain game data.  The executable will print an amusing error message if it doesn't find these files.  You can use a wrapper script, such as the one included in *scripts/dungeon*, in your PATH, in order to run it without so much of a mess.


### Summary, from the in-game text

#### Welcome to Dungeon!

   Dungeon is a game of adventure, danger, and low cunning.  In it you will explore some of the most amazing territory ever seen by mortal man.  Hardened adventurers have run screaming from the terrors contained within.

   In Dungeon, the intrepid explorer delves into the forgotten secrets of a lost labyrinth deep in the bowels of the earth, searching for vast treasures long hidden from prying eyes, treasures guarded by fearsome monsters and diabolical traps!

   No system should be without one!

   Dungeon was created at the MIT Laboratory for Computer Science by Tim Anderson, Marc Blank, Bruce Daniels, and Dave Lebling.  It was inspired by the Adventure game of Crowther and Woods, and the long tradition of fantasy and science fiction games.  The original version was written in MDL (alias MUDDLE).  The current version was translated from MDL into FORTRAN by a somewhat paranoid DEC engineer who prefers to remain anonymous.

### See also

It seems like I'm not the only one who's been working on such a project.  Look at Edward Geist's project over here:
[GOAFI/dungeon](https://github.com/GOFAI/dungeon) ... which seems to be based on the same DOS port.

