# gulp-boilerplate

## Description

This my personal front-end gulp boilerplate.

### Step 1

Download .zip. The folder content the following files :

```
.
├── ...
├── app                     # work directory
│   ├── index.html
│   ├── css
│   │   ├── ...
│   ├── fonts               # copy/paste your fonts here
│   │   ├── ...
│   ├── img
│   │   ├── ...
│   ├── js
│   │   ├── ...
│   ├── scss
│   │   ├── base
│   │   │   ├── ...
│   │   ├── layout
│   │   │   ├── ...
│   │   ├── module
│   │   │   ├── ...
│   │   ├── utilities
│   │   │   ├── _fonts.scss
│   │   │   ├── ...
│   │   ├── ...
│   ├── ...  
├── .gitignore              # to ignore bower_components and node_modules folders
├── .jshintrc               # for gulp-jshint errors
├── gulp-config.json
├── gulpfile.js
├── package.json
├── README.md
└── ...
```

### Step 2

Unzip the folder and rename it :

```
mv gulp-boilerplate/ newProjectName/
```

Change the README.md file :

```
echo "# newProjectName" > README.md
```

### Step 3

In a terminal, go into your folder project and run the following commands :

```
npm install

(step 4)

gulp
```

### Step 4

If you need to use Bower, run the following commands :

```
npm install bower //if bower isn't already install

bower init

bower install package --save-dev //bootstrap, fontawesome for example
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
		],
		"vendorfonts": [
			"bower_components/bootstrap-sass-official/assets/fonts/**/*",
			"bower_components/font-awesome/fonts/**/*"
		]
	}
}
```
