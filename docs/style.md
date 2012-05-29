#Style

The style object allows you to assign custom classes to the main qTip element, as well as [Themeroller](http://jqueryui.com/themeroller/) and
tip options when using the [tips plugin](./plugins/tips.md)

## style.classes: *""*

### Values
"String", false

### Overview
A *space separated* string containing all class names which should be added to the main qTip element.
There are several base styles included in the CSS file provided, including:

```css
/* CSS2 styles */
ui-tooltip{ } /* This one is applied by default (formally the "cream" style) */
ui-tooltip-plain{ }
ui-tooltip-light{ }
ui-tooltip-dark{ }
ui-tooltip-red{ }
ui-tooltip-green{ }
ui-tooltip-blue{ }

/* CSS3+ styles */
ui-tooltip-shadow{ } /* Adds a shadows to your tooltips */
ui-tooltip-rounded{ } /* Adds a rounded corner to your tooltips */
ui-tooltip-bootstrap{ } /* Bootstrap style */
ui-tooltip-tipsy{ } /* Tipsy style */
ui-tooltip-youtube{ } /* Youtube style */
ui-tooltip-jtools{ } /* jTools tooltip style */
ui-tooltip-cluetip{ } /* ClueTip style */
ui-tooltip-tipped{ } /* Tipped style */
```

### Examples
Create a tooltip with the included blue theme and a shadow:

```js
$('.selector').qtip({
	content: {
		text: 'I\'m blue... deal with it!'
	},
	style: {
		classes: 'ui-tooltip-blue ui-tooltip-shadow'
	}
});
```


## style.def: *true*

### Values
true, false

### Overview
This propery allows you to prevent the .ui-tooltip-default class from being applied to the main tooltip element.

### Notes
* Setting this to false will cause the tooltip to have no visual styling if you haven't applied any [custom classes](#style.classes)</li>


## style.widget: *false*

### Values
true, false

### Overview
Determines whether or not the ui-widget classes of the [Themeroller](http://jqueryui.com/themeroller/) UI styles are applied to your tooltip

### Notes
* For more information on Themeroller classes checkout their [documentation](http://docs.jquery.com/UI/)

### See also
* [Classes](#classes)


## style.width: *false*

### Values
"String", Integer, false

### Overview
This property allows you to override all applied CSS width styles for the tooltip. Can be any valid width CSS value. Please note that this
**does not override max/min width styles!** Change those in the CSS file provided.

### Notes
* Again, this **does not override max/min width styles!**


## style.height: *false*

### Values
"String", Integer, false

### Overview
This propery allows you to override all applied CSS height styles for the tooltip. Can be any valid width CSS value. Please note that this
**does not override max/min height styles!** Change those in the CSS file provided.

### Notes
* Again, this **does not override max/min height styles!**


## style.tip: *false*

### Overview
Defines the tooltip's [tip](./plugins/tips.md) properties. See the [plugin documentation](./plugins/tips.md) for more information.