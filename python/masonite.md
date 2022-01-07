## U4D4

***note*** masonite should be installed in its own folder
# pip install masonite
- installs masonite 
**note** needed its own folder was clashing with .gitignore

# craft (command)
- craft is the CLI for masonite

# craft help
- shows list of command lines for masonite

# craft serve
- runs server

# pip install -r requirements.txt

# craft controller (name)
- generates a controller
- Ex. craft controller First

# craft controller (name) -r
- -r labels it as a resource and adds all the restful routes

# contains routes
-folder routes/web.py
# """Web Routes."""

# from masonite.routes import Get, Post
-imports routes others can be added (delete, update)
# ROUTES = [
#    Get("/", "WelcomeController@show").name("welcome"),
#    Get("/first", "FirstController@first").name("first"),
#    Get("/second/@param", "FirstController@second").name("second"),
#    Post("/third", "FirstController@third").name("third")
]