# ionic-hide-ion-tabs-
ionic hide ion-tabs and resolve scroll problem
#Instructions
##About
Have you ever noticed a group of friends Playing mobile phone. When you click on the button on the mobile phone or ipad, button rock will bring you a new experience, could not help but like click with your fingers.
#Installation
 - Clone this repo (or fork then clone, if you prefer)
  - Run `bower install https://github.com/Shangri-GitHub/waggle-and-verification.git --save-dev`

#Example
```javascript
angular.module('starter.directive', [])
//隐藏导航栏
  .directive('hideTabs', function($rootScope) {
    return {
      restrict: 'A',
      link: function($scope) {
        $rootScope.hideTabs = true;
        $scope.$on('$destroy', function() {
          $rootScope.hideTabs = false;
        });
      }
    };
  });
```
 
# Issues

`gulp-sass` is a very light-weight wrapper around [`node-sass`](https://github.com/sass/node-sass), which in turn is a Node binding for [`libsass`](https://github.com/sass/libsass), which in turn is a port of [`Sass`](https://github.com/sass/sass). Because of this, the issue you're having likely isn't a `gulp-sass` issue, but an issue with one of those three projects.

If you have a feature request/question how Sass works/concerns on how your Sass gets compiled/errors in your compiling, it's likely a `libsass` or `Sass` issue and you should file your issue with one of those projects.

If you're having problems with the options you're passing in, it's likely a `node-sass` or `libsass` issue and you should file your issue with one of those projects.

We may, in the course of resolving issues, direct you to one of these other projects. If we do so, please follow up by searching that project's issue queue (both open and closed) for your problem and, if it doesn't exist, filing an issue with them.

