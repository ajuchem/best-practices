# JAVASCRIPT BEST PRACTICES - PART 1
### Resource: [Thinkful](http://www.thinkful.com/learn/javascript-best-practices-1/#Allow-for-Configuration-and-Translation)

***

## Make it understandable
Choose easy to understand and short names for variables and functions.

## Avoid globals
You run the danger of your code being overwritten by any other JavaScript added
to the page after yours.

Use closures and the module pattern.

## Stick to a strict coding style
Browsers are very forgiving JavaScript parses. However, lax coding style will
hurt you when you shift to another environment or hand over to another developer.

Valid code is secure code.

Validate your code: [JSLint](http://www.jslint.com)

## Comment as much as needed but not more
##### "Good code explains itself" is an arrogant myth.

Avoid using the line comment ``//``.

``/* */`` is much safer to use because it doesn't cause errors when the line break is removed.

## Avoid mixing with other technologies
JavaScript is good for calculation, conversion, access to outside sources (Ajax)
and to define the behavior of an interface (event handling). Anything else should
be kept to the technology we have to do that job.

## Use shortcut notations
Shortcut notations keep your code snappy and easier to read once you get used to it.

## Modularize
Keep your code modularized and specialized.

Make sure to write smaller, generic helper functions that fulfill one specific
task rather than catch-all methods.

Good code should be easy to build upon without rewriting the core.

## Enhance Progressivery
Avoid creating a lot of JavaScript dependent code.

DOM generation is slow and expensive. Elements that are dependent on JavaScript
but are available when JavaScript is turned off are a broken promise to our users.

## Allow for configuration and translation
Everything that is likely to change in your code should not be scattered throughout
your code. This includes labels, CSS classes, IDs and presets.

By putting these into a configuration object and making this one public we make
maintenance easy and allow for customization.
