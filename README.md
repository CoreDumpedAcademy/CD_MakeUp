# CD_MakeUp
Open styles library, proudly made by Core Dumped Hackaton Team

# Hey, listen to me
This, guys, is a node project. Once you are inside of it you need to install the dependencies, so:

`
$ cd <<PROJECT-PATH>>
$ npm install
`

Just in case, you can also install node-sass globaly (it has some issues finding its path it seems). **This step might not be needed for you**. Install it globaly with `` npm install -g node-sass``

# Last step, I promise
To run the project and execute everything do:
`$ npm run start`
This will do the following:
1. Compile the sass to the css folder
2. Start listening to the changes you do to the sass and compile it automagically
3. Start a server that serves the html

Therefore, once it is running, you just edit the sass and html, and refresh the page as you normally do, the server will handle the rest for you.
Besis.

# Progress bar

To implement the progress bar, just copy this into the html:

```html
<div class="progress">
  <div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100" style="width: 75%"></div>
</div>
```

Write `progress-bar-stripped` if you want stripes on the progress bar, and ``progress-bar-animated`` if you want an animation on it. The width determines how the progress bar is going, the 75% above is just an example, later it will be linked to something and will not use the width.

# Switch 

To implement the switch, just copy this into the html:

```html
<div class="my-switch">
   <label class="switch">
     <input type="checkbox">
     <span class="my-slider round"></span>
   </label>
</div>
```
# Button

CD_Makeup library modifies buttons giving them a special hover effect:

```html
<button class="btn btn-primary btn-hover-close">>Button_</button>
```

# Cards

CD_Makeup cards are also very simple to implement, they basicly include the button and some styling to links:

```html
<div class="card" style="width: 18rem;">
  <img class="card-img-top" src="img">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary btn-hover-close">Go somewhere</a>
  </div>
</div>
```

# Modals

## Large Modal

This HTML element will create a modal spanning the whole width of the screen

```html
<div class="modal fade" id="myModalLarge" role="dialog">
	<div class="modal-dialog modal-lg">
		<div class="modal-content">
			<div class="modal-header background-primary">
				<h4 class="modal-title">Modal Header</h4>
				<button type="button" class="close" data-dismiss="modal">&times;</button>
			</div>
			<div class="modal-body">
				<p>Some quick example text to build on the modal body and make up the bulk of the modal's content</p>
			</div>
			<div class="modal-footer">
				<button type="button" class="btn btn-primary" data-dismiss="modal">Close</button>
			</div>
		</div>
	</div>
</div>
```

## Short modal

This HTML element will create a shorter modal that will not take the whole screen

```html
<div class="modal fade" id="myModalLarge" role="dialog">
	<div class="modal-dialog modal-lg">
		<div class="modal-content">
			<div class="modal-header background-primary">
				<h4 class="modal-title">Modal Header</h4>
				<button type="button" class="close" data-dismiss="modal">&times;</button>
			</div>
			<div class="modal-body">
				<p>Some quick example text to build on the modal body and make up the bulk of the modal's content</p>
			</div>
			<div class="modal-footer">
				<button type="button" class="btn btn-primary" data-dismiss="modal">Close</button>
			</div>
		</div>
	</div>
</div>
```

# Password Field

This CD_MakeUp element will show the typed characters as points to hide them from view

```html
<div class="form-group">
	<label for="exampleInputPassword1">Password</label>
	<input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
</div>
```