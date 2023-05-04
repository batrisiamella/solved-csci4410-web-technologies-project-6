Download Link: https://assignmentchef.com/product/solved-csci4410-web-technologies-project-6
<br>
Use the 3d webgl canvas and websockets to develop a 3D, 2-player networked “game”. You will need to write a node server named:serverP6.js ## (note the camel case) And, as usual you will need to provide a client in an html file named:p6.html

The server should help the clients to coordinate their views. The game can be re-started by re-starting the server and reloading client web pages.

One cube should be provided to represent each player based on the order in which they visit the game server. One cube should be some interesting color and the other one should have a texture, e.g. crate. Each client should display current view of both cubes as the game progresses. Each player should be able to move and rotate its cube (at some reasonable speed) by using the following key-board commands:

X Y Z – rotate around specified axisW A S D – move along X and YE C – move along Z

Be sure to include a version of three.min.js for your project; I will NOT copy one to your directory from elsewhere.

Likewise, your node server should have a node_modules sub-directory available with the project that supplies all modules it requires, e.g. some websockets library such as ws.

Use turnin to submit a tar file containing all files for the project.

The project will be graded on www.cs.mtsu.edu in this manner:

node serverP6.js &amp; ## &lt;– your server should use one of the two## ports that you were assigned in class## note your server MUST be named serverP6.js

python3 -m http.server –cgi 5994 &amp;## where 5994 is a port that may change; I will choose the port## number AT THE TIME OF TESTING

in chrome on another computer, visit:http://www.cs.mtsu.edu:5994 ## 5994 chgd to same port as above

When I visit that URL, there should be a file there named p6.htmlwhich I will select to load into the browser.Note that I will load p6.html in two different instances of chrometo test as 2 simultaneous players.