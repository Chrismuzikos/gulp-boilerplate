# gulp-boilerplate

## Description

This my personal front-end gulp boilerplate.

### Step 1

Copy the following files :

- app <!-- work directory  -->
   - index.html
   - css
   - img
   - js
   - scss
- .gitignore <!-- to ignore bower_components and node_modules folders -->
- .jshintrc <!-- for gulp-jshint errors -->
- gulp-config.json
- gulpfile.js
- package.json
- README.md


### Step 2

In a terminal, go into your folder project and run the following commands :

```
npm install

gulp
```

### Step 3

If you need to use Bower, run the following commands :

```
npm install bower //if bower isn't already install
bower init
bower install package -save-dev //bootstrap, fontawesome for example
```

and fill the path of the css and js files in the file gulp-config.json like this :

```
{
	"paths": {
    "source": "app",
    "distribution": "dist",
		"vendorcss": [
			"bower_components/bootstrap/dist/css/bootstrap.css",
			"bower_components/font-awesome/css/font-awesome.css",
			"bower_components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css"
		],
		"vendorjs": [
			"bower_components/jquery/dist/jquery.js",
			"bower_components/bootstrap/dist/js/bootstrap.js",
			"bower_components/bootstrap-datepicker/dist/js/bootstrap-datepicker.js"
		]
	}
}
```










```
gulp-boilerplate/
|—— app/
|   |—— css/
|   |   |—— vendor.min.css
|   |—— js/
|   |   |—— script.js
|   |—— scss/
|   |   |—— style.scss
|   |   |—— vendor.scss
|   |   |—— components/
|   |   |   |—— _variables_bootstrap.scss
|   |   |   |—— # more components
|   |—— img/
|   |   |—— # static files and folders
|—— dist/
|   |—— index.html
|   |—— css/
|   |   |—— style.css
|   |   |—— style.min.css
|   |   |—— vendor.css
|   |   |—— vendor.min.css
|   |—— img/
|   |   |—— # image files
|   |—— js/
|   |   |—— classList.js
|   |   |—— classList.min.js
|   |   |—— myplugin.js
|   |   |—— myplugin.min.js
|   |—— fonts/
|   |   |—— # fonts files
|—— .jshintrc
|—— bower.json
|—— gulp-config.json
|—— gulfile.js
|—— package.json
|—— README.md
```
