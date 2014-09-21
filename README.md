# component.collection_list-view-scroll [![Build Status](https://travis-ci.org/typesettin/component.collection_list-view-scroll.svg?branch=master)](https://travis-ci.org/typesettin/component.collection_list-view-scroll) [![NPM version](https://badge.fury.io/js/component.collection_list-view-scroll.svg)](http://badge.fury.io/js/component.collection_list-view-scroll)


# component.collection_list-view-scroll

An on scroll effect template that animates the sides of sections once they are in the viewport


## Example

Check out `example/index.html`, the example javascript for the example page is `resources/js/example_src.js` and in the head section of the example. Full non-js graceful fallback.

[Live Demo - http://typesettin.github.io/component.collection_list-view-scroll](http://typesettin.github.io/component.collection_list-view-scroll)

## Installation

```
$ npm install linotypejs
```

The full page scroll component is a browserify javascript module.


## Usage

*JavaScript*
```javascript
var LinotypeObject = require('linotypejs'),
	myLinotype;
//initialize linotype component after the dom has loaded
window.addEventListener('load',function(){
	myLinotype = new LinotypeObject({
		idSelector: 'linotype'
	});
	//expose your nav component to the window global namespace
	window.myLinotype = myLinotype;
});
```

*HTML*
```html
<html>
	<head>
  	<title>Your Page</title>
  	<link rel="stylesheet" type="text/css" href="[path/to]/component.collection-linotype.css">
  	<script src='[path/to/browserify/bundle].js'></script>
	</head>
	<body>
    <div id="linotype" class="linotype">
    	<div class="section active">
		    <h1>Page One </h1>
		    <p>the basic structure, require a linotype class (for css) and sections for each fullpage section</p>
		  </div>
		  <div class="section">
		    <h1>Page Two </h1>
		    <p>Any html content can go here</p>
		  </div>
		  <div class="section">
		    <h1>Page Three </h1>
		    <p>Keyboard, MouseWheel and Touch Support</p>
		  </div>
		  <div class="section">
		    <h1>Page Four </h1>
		  </div>
	</body>
</html>
```

##API

```javascript
myLinotype.section(1); //jump to section 1
```

###[*FULL API DOCUMENTATION*](https://github.com/typesettin/component.collection-linotype/blob/master/doc/api.md)

##Development
*Make sure you have grunt installed*
```
$ npm install -g grunt-cli
```

Then run grunt watch
```
$ grunt watch
```

##Notes
* The Navigation Module uses Node's event Emitter for event handling.
* The less file is located in `resources/stylesheets`