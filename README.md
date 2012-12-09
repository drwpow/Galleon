Galleon
=======

JavaScript maps loader with Google Maps JavaScript API v3, for use on GalleonProperties.com

Description
-----------
This is the JavaScript code that generates the map on GalleonProperties.com. While there’s not much documentation or explanation for this, I thought I’d share for anyone’s benefit that’s developing a mapping application.

Dependencies
------------
* jQuery
* jQuery UI
* Google Maps API Key

Usage
-----
I have this included as the last line on the page with my map:

	...
	<div id="map-canvas" style="width:100%;height:75%"></div>
	<script type="text/javascript" src="https://maps.googleapis.com/maps/api/js?key=YOURAPIKEY&amp;sensor=true&amp;region=US&amp;libraries=drawing"></script>
	<script type="text/javascript" src="loadmap.js"></script>
	</body>
	...

This is pretty much all it needs to work.  

Notes
-----
The file is divided into 5 sections:

# Global Variables / Initialization: invokes the Google Maps API, sets the center, sets some variables I use globally throughout the script
# Events: event listeners for when a search is made, or when the map is moved or zoomed
# Google Map Functions: functions that place markers on the map and clear drawings
# Common JS functions: functions that parse the results from a PHP script and format them for the map
# UI Setup & UI Events: mostly jQuery UI code for the search box. There's some jQuery code for the search (section 4), but most of the jQuery code is here.


Download
--------
https://github.com/dangodev/Galleon/zipball/master