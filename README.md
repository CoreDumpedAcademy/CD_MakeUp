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

# Map View

To implement the map view, just copy this into the html:

```html
<head>
	<link rel="stylesheet" href="css/styles.css">
	<link rel="stylesheet" href="https://unpkg.com/leaflet@1.3.4/dist/leaflet.css" integrity="sha512-puBpdR0798OZvTTbP4A8Ix/l+A4dHDD0DGqYW6RQ+9jxkRFclaxxQb/SJAWZfWAkuyeQUytO7+7N4QKrDh+drA=="
	 crossorigin="" />
</head>

<body>
	<div class="container-fluid">
		<div class="row">
			<div class="col-md-3-sm-12 offset-md-1">
				<div id="map-view" class="card">
					<div id="mapid" class="leaflet-container card-img-top" tabindex="0">
					</div>
					<div class="card-body">
						<h5 class="card-title">Av. de la Justisia</h5>
						<p class="card-text">Ven a visitarnos ... o no, a mí me da igual</p>
					</div>
				</div>
			</div>
		</div>
	</div>
	<script src="https://unpkg.com/leaflet@1.3.4/dist/leaflet.js" integrity="sha512-nMMmRyTVoLYqjP9hrbed9S+FzjZHW5gY1TWCHA5ckwXZBadntCNs8kEqAWdrb9O7rxbCaA4lKTIWjDXZxflOcA==" crossorigin=""></script>
	<script src="js/map.js"></script>
</body>