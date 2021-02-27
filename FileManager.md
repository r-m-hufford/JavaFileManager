# FileManager

An amazingly useless tool!

##Console Class

The *Console* class manages inputs and outputs. The role of the *console* class is to create the
objects necessary to interact with a user in the terminal. After prompting the user for some input,
it then trims extra white space off any input and makes them uniformly lower case.


##File Operator Class
The *File Operator* class provides the methods necessary to analyze the user input and determine if certain 
file and directory requests are legal. Additionally, it contains functions to return various 
information about files that already exist. *File Operator* holds function which can be used to:
- Check for contents
- Receive info (Name, Path, Size, Created, Last Modified)
- Create directories
- Check file names for illegal characters
- Rename files 
- Copy and delete both files and directories

##File Manager
Using the *Console* class and the methods produced in the *File Operator* class the *File Manager* class
executes the functions that the use requests. An intro is sent which displays the available commands.
The initial while loop buffers against empty inputs. Next a switch statement is used to select 
between the possible methods in *File Operator*. Rename and copy/move are instatiated outside the switch
statement and include the ability to search for an existing file and a try/catch statement to handle
errors form the copy/move method.
