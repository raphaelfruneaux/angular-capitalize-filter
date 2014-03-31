# angular-capitalize-filter

AngularJS filter to capitalize sentences and specially team names.

## Installation

You can install the filter using [Bower](http://bower.io/):

```bash
$ bower install angular-capitalize-filter
```

Then you have to include it in your HTML:

```html
<script src="bower_components/angular-capitalize-filter/capitalize.js"></script>
```

And inject the module `customFilters` in your application:

```js
angular.module('webApp', ['customFilters']);
```

## Usage

You can use it like any other AngularJS filter:

```html
<p>{{ input | capitalize }}</p>
```

Available formats:

* [all](#all)
* [team](#team)

### All

It capitalizes all the words of a given sentence. As it's the default format you can omit the parameter.

```html
<p>{{ sentence | capitalize:'all' }}</p>
```

### Team

Specially adapted for team names, with uppercase abbreviation.

```html
<p>{{ teamName | capitalize:'team' }}</p>
```

It formats the team name as CD Logroñés, FC Barcelona or Valencia CF.