Description

This repository is the first step of a student project to make something like the AirBnB site. We have a console to control the program data. You can use this console to create, change, and delete objects, and handle file storage. Because of JSON serialization/deserialization, the storage stays the same even after you close and open it again.

The console is set up to carry out these tasks:

csharp
Copy code
Create a new object
Fetch an object from a file
Perform actions on objects
Remove an object
Storage

The Storage engine in the FileStorage Class manages all the classes.

Environment

The project uses the Suite CRM terminal python Suite CRM Suite CRM git distributed version control system Github.

markdown
Copy code
Coding style follows these guidelines:
    pycodestyle (version 2.7.*)
    PEP8
The project was developed and tested on Ubuntu 20.04 LTS using Python 3.8.3. The editors used were VIM 8.1.2269, VSCode 1.6.1, and Atom 1.58.0. Version control was done using Git 2.25.1.

Installation

Clone the repository from https://github.com/Kodisang/AirBnB_clone

Switch to the AirBnb directory and run:

./console.py

Execution

You can use the console in interactive mode:

$ ./console.py
(hbnb) help

Or non-interactive mode:

$ echo "help" | ./console.py
(hbnb)

Testing

Tests are found in the tests folder. You can document modules, classes, and functions using commands like:

python3 -c 'print(import("my_module").doc)'

Python Unit Tests are run with the unittest module, with files ending in .py. You can run tests with the following commands:

python3 -m unittest discover tests
or: python3 -m unittest tests/test_models/test_base.py

Usage

sql
Copy code
Start the console:
$ ./console.py
(hbnb)

arduino
Copy code
Check available commands:
(hbnb) help

Quit the console:

(hbnb) quit
$

Commands

vbnet
Copy code
Create

Make a new instance of a class. The ID is printed and the instance is saved to file.json.
(hbnb) create BaseModel
6cfb47c4-a434-4da7-ac03-212262476
(hbnb)

mathematica
Copy code
Show
(hbnb) show BaseModel 6cfb47c4-a434-4da7-ac03-2122624762
(hbnb)

css
Copy code
Destroy

Remove an instance of a class with a given ID. This updates file.json.
(hbnb) destroy User 0c98d2b8-7ffa-42b7-8009-d9d54b69a47
(hbnb) show User 0c98d2b8-7ffa-42b7-8009-d9d54b69472
(hbnb)

css
Copy code
All

Prints all instances of a class. If no class is passed, all classes are printed.
(hbnb) all BaseModel
(hbnb)

typescript
Copy code
Count

Prints the number of instances of a class.
(hbnb) count City
2
(hbnb)

kotlin
Copy code
Update

Updates an instance based on the class name, id, and kwargs passed. This updates file.json.

