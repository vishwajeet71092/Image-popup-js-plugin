# Image Popup (Javascript Plugin)
This Plugin will help you to create pop up image whenever you click on any image on your webpage.

## About Plugin
###### Plugin Name: Image Popup Js Plugin
###### Plugin version: 1.0.0
###### Plugin Author: vishwajeet kumar
###### Description: This Plugin will help you to create pop up image whenever you click on any image on your webpage. This can work in three ways 1. popup all the images of a webpage 2. popup only image inside a div with a paticular id 3. popup all images which has a similar class.

## How to Use
1. Download **image-popup.js** and **image-popup.css**. 
2. Put it in your project directory and link it on the page.

    ````html
    <!-- link image-popup.css (required) -->
    <link rel="stylesheet" href="image-popup.css">
    <!-- link image-popup.js (required) -->
    <script src="image-popup.js"></script>
    ````
### Case 1 (All Image) 

Paste this script before closing body tag and after all js

	
	<script> 
		// for all image
		imagePopupInit({
			type: 'allImage'
		}); 
	</script>
	


### Example Markup for All Image



```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Image Popup Javascript</title>
	
	<!-- styling this page -->
	<style>
		body{
			text-align: center;
			font-family: Arial, Helvetica, sans-serif;
			padding: 10px 50px;
		}
		img{
			max-width: 150px;
			margin: 20px;
		}
		#image-pop{
			border: 1px solid red;
			margin:20px 0px;
		}
		.popimg{
			border: 4px solid #ff9800;
		}
	</style>

	<!-- link image-popup.min.css (required) -->
	<link rel="stylesheet" href="image-popup.css">
</head>
<body>
	<h2>All Image Popup Example</h2><hr>

	<div>

		<!-- images ouside div -->

		<h4>Images ouside div</h4>

		<img src="https://image.freepik.com/free-photo/3d-male-medical-figure-showing-shoulder-scaption_1048-8833.jpg" alt="">
		<img class="popimg" src="https://image.freepik.com/free-photo/3d-halloween-background-with-tree-silhouetted-against-the-moon_1048-8794.jpg" alt="">
		<img src="https://image.freepik.com/free-vector/mountain-landscape-at-night_1048-8048.jpg" alt="">
		<img class="popimg" src="https://image.freepik.com/free-photo/3d-mountain-landscape-against-sunset-sky_1048-7754.jpg" alt="">
		<img src="https://image.freepik.com/free-vector/hand-painted-background-of-a-mountain-landscape_1048-8362.jpg" alt="">

		<!-- images inside a div having class image-pop -->

		<div id="image-pop">

			<h4>Images inside  div</h4>

			<img src="https://image.freepik.com/free-photo/3d-earth-and-fantasy-planet-with-bright-star_1048-8845.jpg" alt="">
			<img class="popimg" src="https://image.freepik.com/free-photo/wooden-table-looking-out-to-a-defocussed-christmas-tree_1048-7235.jpg" alt="">
			<img class="popimg" src="https://image.freepik.com/free-photo/green-world-with-a-tree-background_1048-1484.jpg" alt="">
			<img src="https://image.freepik.com/free-photo/3d-render-of-a-wooden-table-looking-out-to-a-tropical-landscape_1048-6505.jpg" alt="">
			<img class="popimg" src="https://image.freepik.com/free-photo/nature-design-with-bokeh-effect_1048-1882.jpg" alt="">
		</div>
	</div>

	<div>
		<!-- pic credit -->
		<a href="https://www.freepik.com/free-photos-vectors/background">Background image created by Kjpargeter - Freepik.com</a>
	</div>
	
	<!-- link image-popup.min.js (required) -->
	<script src="image-popup.js"></script>
	<!-- initiate the plugin -->
	<script> 
		// for all image
		imagePopupInit({
			type: 'allImage'
		}); 
	</script>
	
</body>
</html>
```

### Case 2 (Images inside a div) 

Paste this script before closing body tag and after all js and target value will be the id of div

	
	<script>
		 
		// for image inside a div
		imagePopupInit({
			type: 'insideDiv',
			target: 'image-pop'
		}); 
 
	</script>
	

### Example Markup for Images inside a div



```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Image Popup Javascript</title>
	
	<!-- styling this page -->
	<style>
		body{
			text-align: center;
			font-family: Arial, Helvetica, sans-serif;
			padding: 10px 50px;
		}
		img{
			max-width: 150px;
			margin: 20px;
		}
		#image-pop{
			border: 1px solid red;
			margin:20px 0px;
		}
		.popimg{
			border: 4px solid #ff9800;
		}
	</style>

	<!-- link image-popup.min.css (required) -->
	<link rel="stylesheet" href="image-popup.css">
</head>
<body>
	<h2>Image Inside Div Example</h2><hr>

	<div>

		<!-- images ouside div -->

		<h4>Images ouside div</h4>

		<img src="https://image.freepik.com/free-photo/3d-male-medical-figure-showing-shoulder-scaption_1048-8833.jpg" alt="">
		<img class="popimg" src="https://image.freepik.com/free-photo/3d-halloween-background-with-tree-silhouetted-against-the-moon_1048-8794.jpg" alt="">
		<img src="https://image.freepik.com/free-vector/mountain-landscape-at-night_1048-8048.jpg" alt="">
		<img class="popimg" src="https://image.freepik.com/free-photo/3d-mountain-landscape-against-sunset-sky_1048-7754.jpg" alt="">
		<img src="https://image.freepik.com/free-vector/hand-painted-background-of-a-mountain-landscape_1048-8362.jpg" alt="">

		<!-- images inside a div having class image-pop -->

		<div id="image-pop">

			<h4>Images inside  div</h4>

			<img src="https://image.freepik.com/free-photo/3d-earth-and-fantasy-planet-with-bright-star_1048-8845.jpg" alt="">
			<img class="popimg" src="https://image.freepik.com/free-photo/wooden-table-looking-out-to-a-defocussed-christmas-tree_1048-7235.jpg" alt="">
			<img class="popimg" src="https://image.freepik.com/free-photo/green-world-with-a-tree-background_1048-1484.jpg" alt="">
			<img src="https://image.freepik.com/free-photo/3d-render-of-a-wooden-table-looking-out-to-a-tropical-landscape_1048-6505.jpg" alt="">
			<img class="popimg" src="https://image.freepik.com/free-photo/nature-design-with-bokeh-effect_1048-1882.jpg" alt="">
		</div>
	</div>

	<div>
		<!-- pic credit -->
		<a href="https://www.freepik.com/free-photos-vectors/background">Background image created by Kjpargeter - Freepik.com</a>
	</div>
	
	<!-- link image-popup.min.js (required) -->
	<script src="image-popup.js"></script>
	<!-- initiate the plugin -->
	<script>
		 
		// for image inside a div
		imagePopupInit({
			type: 'insideDiv',
			target: 'image-pop'
		}); 
 
	</script>
	
</body>
</html>
```


### Case 3 (Images with a class) 

Paste this script before closing body tag and after all js and target value will be the class of images

	
	<script> 
		//for image having class
		imagePopupInit({
			type: 'imageClass',
			target: 'popimg'
		}); 
		 
	</script>
	

### Example Markup for Images with a class



```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Image Popup Javascript</title>
	
	<!-- styling this page -->
	<style>
		body{
			text-align: center;
			font-family: Arial, Helvetica, sans-serif;
			padding: 10px 50px;
		}
		img{
			max-width: 150px;
			margin: 20px;
		}
		#image-pop{
			border: 1px solid red;
			margin:20px 0px;
		}
		.popimg{
			border: 4px solid #ff9800;
		}
	</style>

	<!-- link image-popup.min.css (required) -->
	<link rel="stylesheet" href="image-popup.css">
</head>
<body>
	<h2>Image with class Example</h2><hr>

	<div>

		<!-- images ouside div -->

		<h4>Images ouside div</h4>

		<img src="https://image.freepik.com/free-photo/3d-male-medical-figure-showing-shoulder-scaption_1048-8833.jpg" alt="">
		<img class="popimg" src="https://image.freepik.com/free-photo/3d-halloween-background-with-tree-silhouetted-against-the-moon_1048-8794.jpg" alt="">
		<img src="https://image.freepik.com/free-vector/mountain-landscape-at-night_1048-8048.jpg" alt="">
		<img class="popimg" src="https://image.freepik.com/free-photo/3d-mountain-landscape-against-sunset-sky_1048-7754.jpg" alt="">
		<img src="https://image.freepik.com/free-vector/hand-painted-background-of-a-mountain-landscape_1048-8362.jpg" alt="">

		<!-- images inside a div having class image-pop -->

		<div id="image-pop">

			<h4>Images inside  div</h4>

			<img src="https://image.freepik.com/free-photo/3d-earth-and-fantasy-planet-with-bright-star_1048-8845.jpg" alt="">
			<img class="popimg" src="https://image.freepik.com/free-photo/wooden-table-looking-out-to-a-defocussed-christmas-tree_1048-7235.jpg" alt="">
			<img class="popimg" src="https://image.freepik.com/free-photo/green-world-with-a-tree-background_1048-1484.jpg" alt="">
			<img src="https://image.freepik.com/free-photo/3d-render-of-a-wooden-table-looking-out-to-a-tropical-landscape_1048-6505.jpg" alt="">
			<img class="popimg" src="https://image.freepik.com/free-photo/nature-design-with-bokeh-effect_1048-1882.jpg" alt="">
		</div>
	</div>

	<div>
		<!-- pic credit -->
		<a href="https://www.freepik.com/free-photos-vectors/background">Background image created by Kjpargeter - Freepik.com</a>
	</div>
	
	<!-- link image-popup.min.js (required) -->
	<script src="image-popup.js"></script>
	<!-- initiate the plugin -->
	<script> 
		//for image having class
		imagePopupInit({
			type: 'imageClass',
			target: 'popimg'
		}); 
		 
	</script>
	
</body>
</html>
```
