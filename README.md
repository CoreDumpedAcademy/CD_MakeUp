# CD_MakeUp
Open styles library, proudly made by Core Dumped Hackaton Team

# Hey, listen to me
This, guys, is a node project. Once you are inside of it you need to install the dependencies, so:

``
$ cd <<PROJECT-PATH>>
$ npm install
``

Just in case, you can also install node-sass globaly (it has some issues finding its path it seems). **This step might not be needed for you**. Install it globaly with `` npm install -g node-sass``

# Last step, I promise
To run the project and execute everything do:
``
$ npm run start
``
This will do the following:
1. Compile the sass to the css folder
2. Start listening to the changes you do to the sass and compile it automagically
3. Start a server that serves the html

Therefore, once it is running, you just edit the sass and html, and refresh the page as you normally do, the server will handle the rest for you.
Besis.
