app = angular.module('StarterApp', ['ngMaterial']);

	app.controller('AppCtrl', ['$scope', '$mdSidenav', function($scope, $mdSidenav){
	  $scope.toggleSidenav = function(menuId) {
	    $mdSidenav(menuId).toggle();
	  };
	 
	}]);

	app.controller('RightCtrl', ['$scope', '$mdSidenav', function($scope, $mdSidenav){
	  $scope.toggleSidenav = function(menuId) {
	    $mdSidenav(menuId).toggle();
	  };
	}]);

	app.controller('artCtrl',  ['$scope', '$http', function($scope, $http){
	    $http.get("http://blog-intigrent.cloudapp.net/api/v1")
	    .success(function(response) {
	    	$scope.articles = response;
	    });

	    $scope.isSelected = function(url) {
	    	$scope.details = url;
	    };
	}]);