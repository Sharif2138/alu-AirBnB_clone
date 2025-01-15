AirBnB Clone - The Console

Description

Welcome to the AirBnB Clone project! This is the first step towards building a full-stack web application that mimics the functionality of AirBnB. In this initial phase, we will create a command-line interpreter (CLI) that will manage and manipulate the backend objects of our application, such as users, places, cities, and more.

This command interpreter, referred to as "The Console," will allow us to:

Create and manage new objects.

Save objects to a file in JSON format.

Retrieve objects from storage.

Update object attributes.

Delete objects.

The console will act as the foundation for future phases, including database storage, API development, and front-end integration.

Features of the Command Interpreter

The Console supports the following operations:

Create: Create a new object (e.g., User, Place).

Read: Retrieve an object or list of objects.

Update: Modify attributes of an existing object.

Delete: Remove an object permanently.

Other Operations: Count objects, compute statistics, etc.

How to Start the Console

Requirements

Python version: Python 3.8.5

OS: Ubuntu 20.04 LTS

Pycodestyle Compliance: Code adheres to PEP 8 (version 2.7.*).

Setup

Clone the repository:

git clone https://github.com/<your-group-name>/alu-AirBnB_clone.git
cd alu-AirBnB_clone

Run the console:

./console.py

Usage

Interactive Mode

You can start the console in interactive mode, where you can type commands directly:

$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) quit

Non-Interactive Mode

You can also pass commands in non-interactive mode by piping input to the console:

$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit

Example Commands

Starting the Console

$ ./console.py
(hbnb)

Creating an Object

(hbnb) create User
<new_user_id>

Listing All Objects

(hbnb) all
[<User>, <Place>, <City>...]

Updating an Object

(hbnb) update User <user_id> name "John Doe"

Deleting an Object

(hbnb) destroy User <user_id>

Exiting the Console

(hbnb) quit

Authors

This project is developed by the contributors listed in the AUTHORS file. Each team member has played an integral role in its creation. To view the full list of contributors, check the AUTHORS file: