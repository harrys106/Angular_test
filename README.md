# Angular project's README

Step 2:

Two way binding in angular app

we can add field into an angular app through html and js

this is called as two way binding since we can change either in html and js, the last change will effect at both sides

in this example , we just created an angular app by this piece of code

	var app = angular.module('myApp', []); 

After having an app called 'myApp' , we should create a controller for the app which will control the app
this can be implemented by writing following lines of codes 

	app.controller('myCtrl', function($scope) {
    $scope.firstName= "John";  // here on the time of loading we binded variable 'firstname' to 'John'
    $scope.lastName= "Doe";
	}); 

in the above syntax, contorller name is user dependent .. here it is 'myCtrl'
argument inside the function() , i.e $scope
->Scope is an object that refers to the application model


Task :
add this to controller


$scope.sayHello = function() {
    $scope.greeting = 'Hello ' + $scope.username + '!';
  };

 and put a button in html and  link with this greeting
 and display the result below the Fullname

:)