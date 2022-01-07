## Notes from U4D4
# touch .gitignore
- creates a .gitignore file, these files won't be pushed to github
# Keep the venv folder from pushing to github
- /venv (in .gitignore file)

# echo "/venv" > .gitignore
- creates a .gitignore file and places /venv into it

# python -m venv venv
-creates venv

# Activates Venv
- source ./venv/bin/activate

# Deactivates Venv
- deactivate

# Install dependencies
- pip install (dependency name)  
- Ex. pip install flask

# List dependencies 
- pip list

# Import dependencies
- from (dependency) import (dependency name), request
- Ex. from flask import Flask, request

## Create our application object
app = Flask(__name__)

# create routes
@app.get("/")
def home():
    return {"response": "Hello World"}

# a route with a param
@app.get("/param/<my_param>")
def param(my_param):

# access a URL query
    query = request.args.get("query", None)
    return {"my param was": my_param, "my query was": query}

# app.run(host="localhost", port=3000)
- Turn on server like app.listen in express

# python (file name)
- Runs the local host server
