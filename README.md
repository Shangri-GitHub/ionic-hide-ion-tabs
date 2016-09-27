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
1)ion-tabs导航
  打开页面添加 ng-class="{'tabs-item-hide': hideTabs};
<ion-tabs class="tabs-icon-top tabs-color-active-positive" ng-class="{'tabs-item-hide': hideTabs}">
</ion-tabs>
2)注意添加这个模块hideTabs的directive js 注意app=angular.module(‘directive’, [])
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
 3)内页需要隐藏导航 hide-tabs=”true”
 <ion-view hide-tabs="true" view-title="{{investname}}">
 </ion-view>
```

# Issues



