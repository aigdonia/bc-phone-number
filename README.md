# bc-phone-number [![Build Status](https://travis-ci.org/Ahimta/bc-phone-number.svg?branch=master)](https://travis-ci.org/Ahimta/bc-phone-number)

## Installation

### Bower
```bash
bower install --save bc-phone-number
```
```js
angular.module('myApp', ['bcPhoneNumber'])
```

### NPM
```bash
npm install --save bc-phone-number
```
```js
angular.module('myApp', [require('bc-phone-number')])
```

### Other (not recommended)
Just download the [dist](https://github.com/Ahimta/bc-phone-number/tree/master/dist) folder.

## Usage
```html
<bc-phone-number ng-model='theNumber' default-country='us' preferred-countries='us gb ca' is-valid='isValid'></bc-phone-number>
```

```js
angular.module('myModule', ['bcPhoneNumber', function(bcPhoneNumber) {

  scope.formattedNumber = bcPhoneNumber.format('966501234567');
  scope.isValid = bcPhoneNumber.isValid(scope.formattedNumber);
}]);
```

Note that`ng-model` and `is-valid` are scope variables.
