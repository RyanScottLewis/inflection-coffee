# InflectionCoffee

This is an almost direct port of [InflectionJS](http://github.com/rxgx/inflection-js) written in [CoffeeScript](http://coffeescript.org).

# Usage

#### String.pluralize(plural)

Renders a singular English language noun into it's plural form.  
Normal results can be overridden by passing in an alternative.

#### String.singularize(singular)

Eenders a plural English language noun into it's singular form.  
Normal results can be overridden by passing in an alternative.

#### String.camelize(lowFirstLetter)

Renders a lower case underscored word into camel case.  
The first letter of the result will be upper case unless you pass true.  
This also translates "/" into "::" (`underscore` does the opposite.)

#### String.underscore()

renders a camel cased word into words separated by underscores.
This also translates "::" into "/" (`camelize` does the opposite.)

#### String.humanize(lowFirstLetter)

Renders a lower case and/or underscored word into human readable form.
The first letter of the result will be upper case unless you pass true.

#### String.capitalize()

Renders all characters to lower case and then makes the first upper.

#### String.dasherize()

Renders all underscores and spaces as dashes.

#### String.titleize()

Renders words into title casing (as for book titles.)

#### String.demodulize()

Renders class names that are prepended by modules into just the class.

#### String.tableize()

Renders camel cased singular words into their underscored plural form.

#### String.classify()

Renders an underscored plural word into its camel cased singular form.

#### String.foreign_key(dropIdUnderscore)

Renders a class name (camel cased singular noun) into a foreign key.
Defaults to separating the class from the id with an underscore unless you pass true.

#### String.ordinalize()

Renders all numbers found in the string into their sequence like "22nd".