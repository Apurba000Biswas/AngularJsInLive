# AngularJsInLive

AngularJs started as a project inside Google. Its now open source project. 


## MVC Software Design Patterns:
MVC stands for Model View Controller.

Model :  It is responsible for managing application data. It responds to the requests from view and to the instructions from controller to update itself.

View : It is responsible for displaying all data or only a portion of data to the users. It also specifies the data in a particular format triggered by the controller's decision to present the data

Controller : 
It is responsible to control the relation between models and views. It responds to user input and performs interactions on the data model objects. The controller receives input, validates it, and then performs business operations that modify the state of the data model. 


[AngularJs Home](https://angularjs.org/)

[Plunker](https://plnkr.co/) is a complete web development environment hosted in your browser.

There are two Requirements to add angularjs in a web page.

1. Add a <script> tag pointing to angular.js
    <script src="angular.js"></script>
2. Add an ng-app attribute somewhere in your HTML.
 ```
 <div ng-app>
 	This area controlled by Angular!
 </div>
```

 ```
 <DOCTYPE.!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>My First Page</title>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.2.5/angular.min.js"></script>  
</head>
<body ng-app="myapp">

    <div ng-controller="HelloController" >  
    <h2>Hello {{hello.title}} !</h2>  
    </div>


    <script>  angular.module("myapp", [])  
    .controller("HelloController", function($scope) {  
        $scope.hello = {};  
        $scope.hello.title = "World, AngularJS";  
    } );
    </script>

</body>
</html>
```

### View Part : 
    <div ng-controller="HelloController" >  
    <h2>Hello {{hello.title}} !</h2>  
    </div>

### Controller Part : 

    <script>  angular.module("myapp", [])  
        .controller("HelloController", function($scope) {  
            $scope.hello = {};  
            $scope.hello.title = "World, AngularJS";  
        } );
    </script>

