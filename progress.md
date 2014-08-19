## to do
* blog about bpython pull request
* implement home/away mode
* finish bpython traceback colors
* install bootstrap
* play around with css and javascript stuff

# Aug 19
Soldered temperature sensor circuit for AC project, all hardware works
Need to refactor code for the server and pi program

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
