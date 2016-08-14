# textDecapitator
Single or multi-line truncation with ellipsis.

## How to use

When your document is ready, simply use :

```
$('.your-selector').textDecapitator();
```

You can also use multiple selectors : 


```
$('.your-first-selector, .your-second-selector').textDecapitator();
```

The default text will be assigned to the data-default-text attribute of the HTML element you are decapitating, in case you need it.

## Options

You can pass an object with these options :

- cutRate : the number of characters that are removed on each iteration. 1 will be more precise but slower, 5 will be 5 times faster but
less precise. 

- nbOfLines : the number of lines that you want in the elements of your selector(s).

- callback : callback function executed when all the elements are decapitated.

Example using default values : 

```
$('.your-selector').textDecapitator({
	cutRate : 1,
	nbOfLines : 1,
	callback : function() {

	}
});
```