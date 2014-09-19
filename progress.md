## to do
* implement colloquy style messages (rather than the bare protocol messages for user input)
* figure out how to allow multiple server connections
* use `ack` instead of `grep` for searching through source code
* 'how do you detect a cycle in a linked list in constant space'
* look into pandocs

# Sep 19
* job prep on hash tables 
* got basic functions of the irc client working with asyncio (responds to pings, sends user messages)

# Sep 15
* more pycon proposals
* learned about smtp and smtplib in python
* learned about byte literal vs string literal python3

# Sep 14
* working on pycon proposal

# Sep 13
* recursion practice 

# Sep 10-12
* finished ac blog posts
* refactored snake
* attended job fair 

# Sep 9
* wrote draft of resume, need to register for startup job fair
* more work on AC blog post
# Sep 8
* looked at ipython __future__ imports with the -i (interactive) flag with Tom
* Hacker school learning styles interview with Mel
* finished writing tests for Sudoku with Maia, just have to finish the main outer loop and rewrite the printer and then we will be done.
* working on AC blog post

# Sep 6-7
* finished snake
* wrote blog post about snake

# Sep 5
* phonebook jobs prep challenge. so much sql. maybe should have checked out argparse and maybe should have used separate database for each phonebook

# Sep 4
* wrote test for bpython
* submitted some other bugs to bpython (ANSI escape sequences and terminal resizing issue)
* bpython traceback pull request accepted!
* working on writing body segment class for snake

# Sep 3
* I can move a rectangle around my screen with they keyboard using pygame!
* learning firebase

# Aug 29-30
* successfully installed and used air conditioner remote control
* figured out how to use git rebase -i to squash commits and make a nice looking commit history
* made bpython pull request


# Aug 28
* successfully installed pygame
* completed some more hacker school ctf levels.
  * learned that getElementsByClassName returns an array
  * learned that adding an extra / allowed me to bypass the security filtering 
# Aug 27
* major refactoring of sudoku solver with Maia. Lessons on writing testable code!
* Hacker school capture the flag!! wow learning to use Burp, wireshark, do sql injection and cross site scripting attacks.

# Aug 26

### AC project (pretty much) complete!!!
* All components of AC project working! The project is pretty much complete, still could use some improvements to the styling and needs a bit of security. Also need to set it up in my room.
### bpython
* merged bpython helpful-traceback commits from Tom
* some hiccups figuring out merging properly in git, but I've got it now
* getting errors in unittests
* also, not sure whether I should merge my dev branch into master or whether I should rebase
* waiting for comment from Tom

# Aug 25
* refactored UI for AC project
* played around with bootstrap and jQuery
* worked on sudoku solver with Maia: now have a solver that works for unambiguous 9x9 boards
* figured out how to send POST JSON to my server using jQuery .ajax, and figured out that that's what I needed to be doing to make it work :)

# Aug 23-24
* finished jQuery course, working on javaScript course
* one-on-one with Tom
* met with Carter, worked on making a bouncing ball with gloss in Haskell
* learned about Haskell's pandocs

#Aug 22
* went over dfs and bfs and coded up various solutions (though I need to solidify how to do this with graphs not just trees)

# Aug 21
* discussed recursion with Alan
* went over why a recursive implementation of max(list) blows up in python, talked about tail call optimization and how it would work in Haskell/scheme, and also how the version with a loop in python is basically the same/what tail call optimization turns a tail recursive definition into in a language with tail call optimization

# Aug 20
* started Quick Reminders, a chrome extension to schedule reminders
* worked through a good chunk of jQuery course on code academy
* huge refactor of AC project code, server and UI, still need to refactor the pi code

# Aug 19
* Soldered temperature sensor circuit for AC project, all hardware works
* Need to refactor code for the server and pi program
* wrote blog post about bpython pull request

## Aug 18
Subclassed bpython formatter and code.InteractiveInterpreter, got traceback coloring to work with pygments, just need to incorporate into bpython itself

## Aug 16 - 17
Went to pygotham

## Aug 15
* successfully deployed app to heroku
* practiced for job interviews
* updated github readmes and hacker school bio 

## Aug 14
#### bpython bug
* got a good first draft of the traceback, posted some screenshots on the github issue, people seemed into it
*now need to make some changes to the way I'm doing the regex so that it doesn't fail so much, and also make sure that if it fails, bpython will just do the usual non-colorized traceback rather than blowing up
#### blog
* changed the favicon
* downloaded the .html for twitter cards

## Aug 13
#### bpython bugs
* filed my first bug! <-- not just first for bpython, first for any open source project!
* submitted a pull request for a fix to this bug
* tom merged my pull request
* this was not the original bug I was working on, but a bug I ran into while working on the other one having to do with autocomplete failing on syntax errors when you're just trying to revise a line of code before hitting enter 
* still working on the helpful traceback colors

#### ac project
* paired with dana to get the temperature sensor working
* it works, but now I need to implement how the home/away modes should work, namely that I should always be able to manually override the desired temperature setting, but the "desired state" variable should not always interfere with home mode
* also need to buy some wires and a new temperature sensor to give back to dana 
*also learned a bit of css

## Aug 12
####bpython bugs

* got set up with dev environment
* paired with Tom to learn about the bpython directory structure, important files, getting started, etc
* chose a "bitesize bug" to work on: making the Traceback output friendlier and easier to read (right now it's just all red)
* subclassing code.InteractiveInterpreter 
* thus far, I have a subclass that can change colors of various lines of the output
####ac project
* paired with brent to make my raspi program handle http errors more gracefully, within the try statement of my main error handler i have another try except that catches IOErrors, which should catch the request errors. Using timedelt from datetime, the program tries the request again for five minutes, at which point it turns the AC off, but keeps throwing requests at the server in the hopes that it will come back

####algorithms course group
####textbooks

* read through some of the later chapters of learning python the hard way

## Before this log started
In broad strokes
### Projects
#### remotely controlled air conditioner web app:

* working flask server returning functional but ugly UI
* got a raspberry pi set up and installed raspbian, set up usb wifi
* pi runs a python program using the requests library to post to my flask server (currently hosted locally), and updates the air conditioner state according to information in the response to the post request
* have some javascript with jquery for improving the UI side
* using threads (flask's threaded=true option) so that requests from the client on the UI side do not interfere with the pi requests (this should be ok since, I am the only intended client)
* thus far, the app successfully can turn my ac (right now a lightbulb) on and off

### Courses

* completed first chapter of udacity *Design of Computer Programs* with Peter Norvig
* watched first 5 chapters of lectures for Stanford machine learning on coursera

### Textbooks

* read 5 chapters of intro to network programming in python
* working through this [python algorithms and data structures book](http://interactivepython.org/runestone/static/pythonds/index.html) as well as this [* Introduction to Algorithms* ](http://mitpress.mit.edu/books/introduction* algorithms)

###other

* lots of getting set up/comfortable with sublime/comfortable using virtualenvs etc
