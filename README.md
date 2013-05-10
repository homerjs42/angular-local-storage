angular-local-storage
=====================

These are my modifications to the module developed by Greg Pike.  The original is located at
https://github.com/grevory/angular-local-storage.

This is an Angular module that gives you access to the browsers local storage

Remember to set your app name (settings.appPrefix) in the settings at the beginning of localStorageModule.js.

Example use:

```javascript
angular.module('yourModule', ['LocalStorageModule'])
.controller('yourCtrl', [
  '$scope',
  'localStorageService',
  function($scope, localStorageService) {
    // Start fresh
    localStorageService.clearAll();
    localStorageService.add('Favorite Sport','Ultimate Frisbee');
}]);
```
