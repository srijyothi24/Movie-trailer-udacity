# Movie-trailer-udacity
MOVIE-TRAILER: 
The Movie Trailer Website project consists of server-side code to store a list of movies titles, along with its respective box art imagery and movie trailer website. The data is served as a web page allowing visitors to watch the trailers

GETTING-STARTED: 
These instructions will help you to run the project on your local computer. See deployment for notes on how to deploy the project on a live system.

INSTALLATION AND EXECUTION: 
Install python on your computer from https://www.python.org/downloads/ To confirm that your installation was successful, open IDLE (python GUI), a program installed by Python that makes it easy to edit and run Python code. After the successful installation of python on your system, check with the basic commands like,

Python itself comes with an editor that you can access from the IDLE File > New File menu option. Write the code in that file, save it as [filename].py and then (in that same file editor window) press F5 to execute the code you created in the IDLE Shell window.

USING COMMAND PROMPT:
command line python in windows, save your file with .py extension. Now open command prompt and and change the current directory to python existing directory using the command

cd C:\Python27 try this

C:\Python27>python if you get the python version and message then your python is succesfully installed and python path is added to your system

C:\Python27>python Python 2.7.9 (default, Dec 10 2014, 12:28:03) [MSC v.1500 64 bit (AMD64)] on win32 Type "help", "copyright", "credits" or "license" for more information.
>>>

If you get this message, then python isn't on your path 'python' is not recognized as an internal or external command, operable program or batch file. Putting Python In Your Path

My Computer > Properties > Advanced System Settings > Environment Variables > system variables -> Path This needs to include: C:\Python26; (or equivalent). If you put it at the front, it will be the first place looked. You can also add it at the end.Then restart your prompt, and try typing 'python'. If it all worked, you should get a ">>>" prompt.

PROCEDURE:
open a new file and save with .py extension such that it represents a python file. And follow the instructions as given below: Create a class named Movie remember class name should start with a capital letter

class Movie (): # to store the movie name title story and trailer Create an instance for Movie class that includes name story trailer and poster, which allocates memory for the Movie class. The init function is called a constructor, or initializer, and is automatically called when you create a new instance of a class. Within that function, the newly created object is assigned to the parameter self.

def init (self, arg1, arg2, ..): In init method self refers to the newly created object, in other class methods, it refers to the instance whose method was called.

import webbrowser 
class Movie(): 
def init(self, title, storyline, poster_image_url, trailer_youtube_url):
self.title = title 
self.storyline = storyline 
self.poster_image_url = poster_image_url
self.trailer_youtube_url = trailer_youtube_url
def show_trailer(self): webbrowser.open(self.trailer_url) 
Notice that we had to pass self in again; this is true of all instance methods. We modifed our other file a bit to see things working:

toy_story = media.Movie("Toy Story", "A story of a boy and his toys that come to his life",
                        "images/Toy_Story.jpg", 
                        "https://www.youtube.com/watch?v=vwyZH85NQC4")

The web browser should open with the trailer playing!

open movies list and takes in the list of movies
fresh_tomatoes.open_movies_page(movies) I have created the class Movie and created instances for that in the same file, in order to make it clear, create a list of these movie objects and save it another file entertainment_center.py and by calling the constructor media.Movie() we can instantiate movie objects, and this list of movies is given as input to open_movies_page() function to build the HTML file and display our website

RUN THE PROGRAM: 
once we finish writing the code save the file and run the module as go to run and click run module-F5 (IDLE) and finally it displays our movie trailer website or we can run in command prompt as mentioned in the installation process like

D:\UDACITY PROJECT1
D:\UDACITY PROJECT1\entertainment_center.py(2.7.9)*

This opens our project output window(Movie trailer website).This tells about the sucessful execution of our project
