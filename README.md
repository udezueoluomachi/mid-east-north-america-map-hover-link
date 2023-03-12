# How To Use With Wordpress

Here's an example of you can display the edited SVG in WordPress:

* Save the SVG file to your computer.

* Log in to your WordPress admin panel and navigate to the page or post where you want to add the map.

* Click on the "Add Media" button to upload the SVG file.

* Drag and drop the SVG file into the media uploader, or click the "Select Files" button to choose the file from your computer.

* Once the file is uploaded, click on it to open the "Attachment Details" panel.

* In the "Attachment Details" panel, copy the "File URL" or "Image URL" for the SVG file.

```html
<object data="path/to/usa-labels-full.svg" type="image/svg+xml" id="map">
	Your browser does not support SVG
</object>
```

* Replace "path/to/your/usa-labels-full.svg" with the correct file path or URL of the edited SVG file which you uploaded (usa-labels-full.svg).

* To add the SVG to WordPress, follow these steps:

* Open the WordPress post or page where you want to add the SVG map.

* Switch to the "Text" or "HTML" view of the editor.

* Paste the html code above into the editor where you want the SVG map to appear.

## Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <!--you should style the object map container-->
    <style>
		#map {
			max-width: 100%;
			height: auto;
			border: 1px solid grey;
            object-fit: contain;
		}
    </style>
</head>
<body>
    <!--This is where you want to add the map-->
    <object id="map" alt="MAP" data="./usa-labels-full.svg" type="image/svg+xml">
        Your browser does not support SVG
    </object>
</body>
</html>
```

* Save or publish the post or page.

## Note

* The section of the map clicked opens the link in a new tab

This code will display the edited SVG map in the post or page, with the CSS styles applied. The "object" tag is used to embed the SVG file in the HTML code, and the "type" attribute specifies the MIME type of the file. The "id" attribute can be used to apply additional styles or scripts to the SVG object if needed.

Note that some WordPress themes or plugins may have restrictions on adding SVG files, so make sure to check the documentation or contact the support team if you encounter any issues.