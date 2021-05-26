# GOD-VIEW
Experimental Remote Access Tool written in Python for the Server / Client with an Sqlite3 database. React.js with TypeScript using Redux for global state management & styled components for custom design for the Desktop / Web UI.
The project tackles a multitude of topics related to sophisticated networking related applications. With support for different operating systems, application types with strong compatibility for Terminal usage, web browsers, mobile usage, scalable data-structures. Supporting smart code-design & modern Python versions.
* Windows, Mac & Linux OS support
* Provides a Terminal, Desktop & Web UI
* Extensive Terminal UX support & Desktop / Web Responsive Design (320x320+)
  * Mobile specific interactions & strong browser support
* Uses TCP sockets, utilizing a custom protocol supporting
  * Serialization
  * Encoding
  * Compression
  * Asymmetrical AES Encryption
* Providing 41 sophisticated commands over 9 categories of actions
 * Initial client connection with 30 data fields gathered
 * Can run any command with one-to-many clients without performance issues
* Support for extensive features with a relatively small executable
  * ~8MB client & an larger ~58MB server
* Streaming sockets for modules
 * Desktop, Webcam & Audio streams
 * Keylogger & Clipper

### The Terminal & GUI User Interfaces
<img src="/build/github/ui.png" />
<img src="/build/github/terminal.png" />

## How to run GOD-VIEW
* Simply run the host.exe & then bot.exe
  * These are executable files for Windows
---
To run it with Python you simply install the necessary packages.
This will also allow for hosting not limited to your localhost
- pip install -r build/requirements.txt
- install the necessary .wheel files from build/wheel_requirements.txt
  - PyAudio
  - VideoCapture when using Windows
---
Then run the python scripts
- python host.py
- python bot.py
---
To support external hosting, simply specify the "-IP" CLI argument to your real IP and modify the Static.IP class variable in client/state.py before using the build command on the server.

## How to use GOD-VIEW
<img src="/build/github/help.png" />

GOD-VIEW follows a very simple, straight forward way of constructing commands. Use the "help" command in the terminal for all the available options for each command, were parenthesis means the flag is optional. --FLAG is a boolean, while --FLAG [INPUT] means it requires a string input.

<img src="/build/github/gui help.png" />
This is even simpler using the desktop / web UI, you simply click a command, enter the necessary data into the inputs / checkboxes and execute the commands. To enter sessions from the desktop / web UI you would click, CTRL+click or SHIFT+click on any of the connected clients before right-clicking on them to get up a menu with the option to add the selected clients to a session.

## GOD-VIEW Network Architecture
<img src="/build/github/network architecture.png" />
The architecture has the terminal window as the main server, the GUI as an interface for the terminal and then the connecting clients.

<object data="/build/github/GOD-VIEW.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="/build/github/GOD-VIEW.pdf">
     <p>This browser does not support PDFs</p>
    </embed>
</object>
