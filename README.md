# angular-dropdowns

Forked from https://github.com/jseppi/angular-dropdowns
Data types have been changed for a simpler implementation. Options are an array of strings and the seleceted value is a string.

## Usage

Include `ngDropdowns` in your module dependencies:

```js
var app = angular.module('app', ['ngDropdowns']);
```

In your controller, setup the select options and object to hold the selected value:

```js
app.controller('AppCtrl', function($scope) {

    $scope.selectOptions = ['Option1', 'Option2', 'Option3'];

});
```

And in your html, specify the `dropdown-select` and `dropdown-model` attributes on an element.

You can optionally set `dropdown-item-label` to specify a different label field from the default (which is 'text'):

```html

    <div dropdown-select="selectOptions" dropdown-model="yourModel.fieldName"></div>

```

