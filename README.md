# GOD-VIEW
explain what it does (like the desc)
- and browser support

**The User Interface**
<img src="/build/github/UI.png" />

## How to Install GOD-VIEW
> Simply run the host.exe & then bot.exe
  > These are executable files for Windows
---
To run it with Python you simply install the necessary packages.
This will also allow for hosting not limited to your localhost.
---
- pip install -r build/requirements.txt
- install the necessary .wheel files from build/wheel_requirements.txt
  - PyAudio
  - VideoCapture when using Windows
---
Then run the python scripts
- python host.py
- python bot.py
---
To support external hosting, simply specify the -IP CLI argument to your real IP and modify the Static.IP class variable in client/state.py before using the build command on the server.

## How to use GOD-VIEW
![image text](image url "image Title")

GOD-VIEW follows a very simple, straight forward way of constructing commands. Use the "help" command in the terminal for all the available options for each command, were parenthesis means the flag is optional. --FLAG is a boolean, while --FLAG [INPUT] means it requires a string input.

To enter a session with a client, this would be an example of how to do it:
- list
- session --id [Unique ID]

Then you would be able to run session specific commands, for example to take a screenshot of all monitors and showing the screenshot you would simply type:
- screenshot --monitor -1 --show

To enter multiple clients into a session at the same time you would run:
session --id [Unique ID],[Unique ID],[Unique ID]

To remove these clients from the session, you would run:
[Unique ID],[Unique ID],[Unique ID] --remove

![image text](image url "image Title")
This is even simpler using the desktop / web UI, you simply click a command, enter the necessary data into the inputs / checkboxes and execute the commands. To enter sessions from the desktop / web UI you would click, CTRL+click or SHIFT+click on any of the connected clients before right-clicking on them to get up a menu with the option to add the selected clients to a session.

## GOD-VIEW Network Architecture
![image text](image url "image Title")
The architecture has the terminal window as the main server, the GUI as an interface for the terminal and then the connecting clients.
