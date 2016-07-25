# Address Auto Complete

Improve the user-experience of your forms by adding auto-complete functionality to your address fields, powered by Google Maps. [Solodev](https://www.solodev.com/) has provided a turn-key form for you to use on your website or in your project.

## Note

This example will not work unless you have a registered and active Google API key. To register a new key, visit [Google's 
Get a Key/Authentication](https://developers.google.com/maps/documentation/javascript/get-api-key) page.

## Tutorial

For detailed instructions, view Solodev's [Adding an Auto-Complete Address Form to your Website](https://www.solodev.com/blog/web-design/code-examples/adding-an-auto-complete-address-form-to-your-website.stml) article.

## Demo

Check out a working example on [JSFiddle](https://jsfiddle.net/solodev/ykajnmkk/).

## HTML

The form includes basic HTML markup:
```
<div class="container">
	<div class="panel panel-primary">
		<div class="panel-heading">
			<h3 class="panel-title">Address</h3>
		</div>
		<div class="panel-body">
			<input id="autocomplete" placeholder="Enter your address" onFocus="geolocate()" type="text" class="form-control">
			<br>
			<div id="address">
				<div class="row">
					<div class="col-md-6">
						<label class="control-label">Street address</label>
						<input class="form-control" id="street_number" disabled="true">
					</div>
					<div class="col-md-6">
						<label class="control-label">Route</label>
						<input class="form-control" id="route" disabled="true">
					</div>
				</div>
				<div class="row">
					<div class="col-md-6">
						<label class="control-label">City</label>
						<input class="form-control field" id="locality" disabled="true">
					</div>
					<div class="col-md-6"> 
						<label class="control-label">State</label>
						<input class="form-control" id="administrative_area_level_1" disabled="true">
					</div>
				</div>
				<div class="row">
					 <div class="col-md-6">
						<label class="control-label">Zip code</label>
						<input class="form-control" id="postal_code" disabled="true">
					 </div>
					 <div class="col-md-6">
						<label class="control-label">Country</label>
						<input class="form-control" id="country" disabled="true">
					 </div>
				</div>
		   </div>
		</div>
	</div>
</div>
```

## CSS

CSS for this repository is primarily based on default Bootstrap classes.

## JavaScript

Some basic validation is included in auto-complete.js. Further, the form requires a registered API key from Google Developers. Once your key is registered, copy it and replace in the following script:
```
<script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&libraries=places&callback=initAutocomplete" async defer></script>
```

To register a new key, visit [Google's 
Get a Key/Authentication](https://developers.google.com/maps/documentation/javascript/get-api-key) page.

## External Includes

The form includes the following third-party resources:
```
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css" rel="stylesheet" type="text/css"/>
	
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js" type="text/javascript"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js" type="text/javascript"></script>
```
