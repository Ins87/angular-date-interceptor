# angular-date-interceptor
==============

An AngularJS interceptor to parse dates from server response.

[![Build Status](https://codeship.com/projects/58bfa520-2ed5-0132-0af5-6a016ae0b812/status?branch=master]

The problem
-----------
By default, if you want to bind a model (which comes from the server) to a date input, you will get `Error: [ngModel:datefmt] Expected `2015-07-25T11:40:35.395Z` to be a date`. 
The problem is that the date is in ISO 8061 string format and it is not a date object. This interceptor convert dates into date objects.

Installation
------------
You can choose your preferred method of installation:
* Through bower: `bower install angular-date-interceptor --save`
* Through npm: `npm install angular-date-interceptor --save`
* Download from github: [unminified version](https://raw.github.com/Ins87/angular-date-interceptor/master/dist/angular-date-interceptor.js) or [minified version](https://raw.github.com/Ins87/angular-date-interceptor/master/dist/angular-date-interceptor.min.js)

Usage
-----
Include angular-date-interceptor.js in your application.

```html
<script src="components/angular-date-interceptor/dist/angular-date-interceptor.js"></script>
```

Add the module `angularDateInterceptor` as a dependency to your module:

```js
angular.module('myApp', ['angularDateInterceptor']);
```

License
-------
Released under the terms of the [MIT License](LICENSE).
