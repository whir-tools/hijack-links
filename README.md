hijack-links
============

Hijack your static and dynamic anchors without needing jquery

# usage

```javascript

var hijack = require('whir-hijack-links');

var handler = function(pathname){
	console.log(pathname);
	// but expecting something like:
	// eg. with director
	// router.setRoute(pathname);
}

// as we're not setup yet, give hijack a handler
// if it's the first time you call it, will throw if you dont give it a callback
var controls = hijack(handler);

// controls are as follows
controls.isHijacking(); // true in this case
controls.disable(); // stop hijacking
controls.enable(); // start again


```


