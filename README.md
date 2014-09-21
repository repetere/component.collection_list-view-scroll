# component.collection_list-view-scroll [![Build Status](https://travis-ci.org/typesettin/component.collection_list-view-scroll.svg?branch=master)](https://travis-ci.org/typesettin/component.collection_list-view-scroll) [![NPM version](https://badge.fury.io/js/component.collection_list-view-scroll.svg)](http://badge.fury.io/js/component.collection_list-view-scroll)


# component.collection_list-view-scroll

An on scroll effect template that animates the sides of sections once they are in the viewport


## Example

Check out `example/index.html`, the example javascript for the example page is `resources/js/example_src.js` and in the head section of the example. Full non-js graceful fallback.

[Live Demo - http://typesettin.github.io/component.collection_list-view-scroll](http://typesettin.github.io/component.collection_list-view-scroll)

## Installation

```
$ npm install periodicjs.component.collection_list-view-scroll
```

The scroll component is a browserify/commonjs javascript module.


## Usage

*JavaScript*
```javascript
var ListViewScrollObject = require('periodicjs.component.collection_list-view-scroll'),
	listViewScroller1;
//initialize linotype component after the dom has loaded
window.addEventListener('load',function(){
	listViewScroller1 = new ListViewScrollObject({
		idSelector: 'list-view-scroll'
	});
	//expose your nav component to the window global namespace
	window.listViewScroller1 = listViewScroller1;
});
```

*HTML*
```html
<html>
	<head>
  	<title>Your Page</title>
  	<link rel="stylesheet" type="text/css" href="[path/to]/component.collection_list-view-scroll.css">
  	<script src='[path/to/browserify/bundle].js'></script>
	</head>
	<body>
    <div id="list-view-scroll" class="list-view-scroll">
    	<section class="list-view-scroll-section">
      	<article class="list-view-scroll-side-item list-view-scroll-side-left">
      	<h1>Page One </h1>
		    <p>the basic structure, require a linotype class (for css) and sections for each fullpage section</p>
				</article>
        <figure class="list-view-scroll-side-item list-view-scroll-side-right">
          <img src="http://dummyimage.com/600x400/000/fff">
        </figure>
		  </section>
		  <section class="list-view-scroll-section">
        <figure class="list-view-scroll-side-item list-view-scroll-side-left">
          <img src="http://dummyimage.com/600x400/000/fff">
        </figure>
      	<article class="list-view-scroll-side-item list-view-scroll-side-right">
		    <h1>Page Two </h1>
		    <p>Any html content can go here</p>
				</article>
		  </section>
    	<section class="list-view-scroll-section">
      	<article class="list-view-scroll-side-item list-view-scroll-side-left">
      	<h1>Page One </h1>
		    <p>the basic structure, require a linotype class (for css) and sections for each fullpage section</p>
				</article>
        <figure class="list-view-scroll-side-item list-view-scroll-side-right">
          <img src="http://dummyimage.com/600x400/000/fff">
        </figure>
		  </section>
		  <section class="list-view-scroll-section">
        <figure class="list-view-scroll-side-item list-view-scroll-side-left">
          <img src="http://dummyimage.com/600x400/000/fff">
        </figure>
      	<article class="list-view-scroll-side-item list-view-scroll-side-right">
		    <h1>Page Two </h1>
		    <p>Any html content can go here</p>
				</article>
		  </section>
	</body>
</html>
```

##API

###[*FULL API DOCUMENTATION*](https://github.com/typesettin/component.collection_list-view-scroll/blob/master/doc/api.md)

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