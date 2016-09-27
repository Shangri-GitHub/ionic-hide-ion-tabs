# ionic-hide-ion-tabs-
ionic hide ion-tabs and resolve scroll problem
'''
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
'''
