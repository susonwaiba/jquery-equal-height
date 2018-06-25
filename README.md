# jQuery Equal Height

A small jQuery plugin to match equal height of elements in row

- [online demo](https://susonwaiba.github.io/jquery-equal-height/index.html)

## Setup

### Installation from npm
```
npm install jquery-equal-height --save
```

### Installation from github

[Download Zip](https://github.com/susonwaiba/jquery-equal-height/archive/master.zip) and copy **js/jquery-equal-height.min.js** file to your working js dir.

Add "**jquery-equal-height.min.js**" to your footer after jQuery
```
<!-- Loading jQuery -->
<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
<!-- Loading jQuery Equal Height for Newer version of Jquery -->
<script type="text/javascript" src="js/jquery-equal-height.min.js"></script>
```

### For Older Version of jQuery

```
<!-- Loading jQuery Equal Height for Newer version of Jquery -->
<script type="text/javascript" src="js/jquery-equal-height-old.js"></script>
```

### Initialize

Use load if images are mixed up for proper height calculation after images are loaded

HTML
```
<div class="row">
	<div class="col-md-6 jQueryEqualHeight">
		<div class="card">
			...
		</div>
	</div>
	...
</div>
```

JavaScript
```
$(window).on('load', function(event) {
    $('.jQueryEqualHeight').jQueryEqualHeight();
});
```

### Define Inner Class
**.card** class is default but you can define your own

```
$(window).on('load', function(event) {
    $('.jQueryEqualHeight').jQueryEqualHeight('.new-card-class');
});
```

### Resize

```
$(window).resize(function(event) {
    $('.jQueryEqualHeight').jQueryEqualHeight();
});
```

### Equal height different parts of card

```
$(window).on('load', function(event) {
    $('.jQueryEqualHeight').jQueryEqualHeight('.card .card-body .card-title');
    $('.jQueryEqualHeight').jQueryEqualHeight('.card .card-body .card-text');
    $('.jQueryEqualHeight').jQueryEqualHeight('.card');
});
```

## Links
[Website](http://susonwaiba.com) | [Github](https://github.com/susonwaiba)
