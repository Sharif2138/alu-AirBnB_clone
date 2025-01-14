# AirBnB Clone - The Console

## Description
Welcome to the **AirBnB Clone** project! This is the first step towards building a full-stack web application that mimics the functionality of AirBnB. In this initial phase, we will create a **command-line interpreter** (CLI) that will manage and manipulate the backend objects of our application, such as users, places, cities, and more.

This command interpreter, referred to as "The Console," will allow us to:
- Create and manage new objects.
- Save objects to a file in JSON format.
- Retrieve objects from storage.
- Update object attributes.
- Delete objects.

The console will act as the foundation for future phases, including database storage, API development, and front-end integration.


Features of the Command Interpreter
The Console supports the following operations:
1. **Create**: Create a new object (e.g., User, Place).
2. **Read**: Retrieve an object or list of objects.
3. **Update**: Modify attributes of an existing object.
4. **Delete**: Remove an object permanently.
5. **Other Operations**: Count objects, compute statistics, etc.

---

How to Start the Console

 Requirements
- **Python version**: Python 3.8.5
- **OS**: Ubuntu 20.04 LTS
- **Pycodestyle Compliance**: Code adheres to PEP 8 (version 2.7.*).

 Setup
1. Clone the repository:
   bash
   git clone https://github.com/<your-group-name>/alu-AirBnB_clone.git
   cd alu-AirBnB_clone
   
2. Run the console:
   bash
   ./console.py


Usage
Interactive Mode
You can start the console in **interactive mode**, where you can type commands directly:
bash
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) quit

Non-Interactive Mode
You can also pass commands in **non-interactive mode** by piping input to the console:
bash
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit


Example Commands

Starting the Console
bash
$ ./console.py
(hbnb)


Creating an Object
bash
(hbnb) create User
<new_user_id>


Listing All Objects
bash
(hbnb) all
[<User>, <Place>, <City>...]
```

Updating an Object
bash
(hbnb) update User <user_id> name "John Doe"


Deleting an Object
bash
(hbnb) destroy User <user_id>


Exiting the Console
bash
(hbnb) quit


File Structure
├── AUTHORS             
├── README.md           
├── console.py          
├── models              
│   ├── base_model.py   
│   ├── user.py         
│   ├── place.py        
│   ├── ...
├── tests               
│   ├── test_models
│   │   ├── test_base_model.py
│   │   ├── test_user.py
│   │   ├── ...

Authors
This project is developed by the contributors listed in the `AUTHORS` file. Each team member has played an integral role in its creation. To view the full list of contributors, check the `AUTHORS` file:

bash
cat AUTHORS


License
This project is licensed under the MIT License. See the LICENSE file for details.

Notes
1. Ensure all your Python files end with a new line and are executable.
2. Use `python3 -m unittest discover tests` to run all unit tests.
3. Follow the directory structure for easy navigation and testing.
4. For help, type `help` in the console.


