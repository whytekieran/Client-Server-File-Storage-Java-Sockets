						CLIENT / SERVER SOCKET PROJECT
						==============================

MODULE: Operating Systems
LECTURER: Martin Hynes
STUDENT: Ciaran Whyte
STUDENT ID: G00254624

						     PROJECT INTRODUCTION
						     ====================

This project contains four classes and their class files:

ClientSideApplicationMain.java - This consists of the main application on the client side. The main method runs here for the client,
it consists of a Client object which has methods for handling the clients main tasks. As well as a do-while loop which contains
a switch statement. The switch statement is used for the users commands and corresponds to a do-while and switch on the server side.

Client.java - A class which contains methods that are used by the Client object inside our main method for the client.

ServerSideApplicationMain.java - The main method for the server, doesnt do much except listen for a client connection and when it
gets one it spawns off an individual thread for that particular client.

ClientRequestThread.java - The thread that is spawned off by the servers main method, this does the work on the server. Each client
would have a corresponding thread like this one servicing it.

It also contains a folder called "User Information" that holds two text files for user names and passwords.
It accepts 

						  BRIEF PROJECT DESCRIPTION
						  =========================

Briefly, the program works as follows. First when we run the client side main where you will be asked for authentication. 
This is inside a do while and will keep asking until authentication is successful.
The user name and password entered is then sent to the server which sends back either 0 = no success or 1 = success. Then after a
successful login the user will be sent all the information regrading his/her root directory. This is then followed by a do-while
loop that contains the main menu and a switch statement for each task the user might choose, this corresponds with a do-while and 
switch statement on the server side. All the code has been heavily commented to help in understanding what is happening quickly.

						 	HOW TO RUN IT
							=============
Acceptable Usernames: user1, user2, user3
Acceptable Passwords: pass1, pass2, pass3
The usernames and passwords are case sensitive and must be entered like user1 pass1, user2 pass2 etc

The class files contained in this project can be placed anywhere on the server and ran from the command line. You should run
ServerSideApplicationMain from the command line on the server side. Then on the client side you can run the ClientSideApplicationMain
which will ask for username, password and the IP address of the server. You may use your own server for this but if you want to 
use mine the IP address is 40.76.26.86 and wont change as im leaving it running. Its only one core it is not hogging much credit.
On my server ive left an empty folder called "ServerSideProjectOS" which you can place the information needed inside. (You dont 
have to do this i just left it there if you want, its your choice)

IMPORTANT: Wherever you decide to put the information needed to run the server side program is your choice, but you will need the 
following three items in that location to run the server side:

					ServerSideApplicationMain - Its class file (Run this from command line)
					ClientRequestThread	  - Its class file
					User Information	  - Folder with text files containing authentication details
					
--Finally if there are any issues whatsoever please do not hesitate to email me ASAP. The program has been tested and meets requirements
in your specification.
						Merry Christmas Martin :)
						



 




