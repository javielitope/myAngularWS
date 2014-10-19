// Expressions
AngularJS expressions are much like JavaScript expressions: They can contain literals, operators, and variables.
Example {{ 5 + 5 }} or {{ firstName + " " + lastName }}

// Objetcs
AngularJS objects are like JavaScript objects: person={firstName:'John',lastName:'Doe'}

// Arrays
AngularJS arrays are like JavaScript arrays: points=[1,15,19,2,40]

// Directivas
- The ng-app directive defines the root element of an AngularJS application. The ng-app directive will auto-bootstrap (automatically initialize) the application when a web page is loaded. Later you will learn how ng-app can have a value (like ng-app="myModule"), to connect code modules.

- The ng-model directive binds the value of HTML controls (input, select, textarea) to application data. The ng-model directive can also:
   Provide type validation for application data (number, email, required).
   Provide status for application data (invalid, dirty, touched, error).
   Provide CSS classes for HTML elements.
   Bind HTML elements to HTML forms.

- The ng-init directive initialize application data.

- The ng-bind directive binds application data to the HTML view. Equivalente a {{ expressiong }}

- The ng-controller directive defines the controller. The controller code will execute when the page loads. A controller is a JavaScript Object, created by a standard JavaScript object constructor.
The $scope of the controller is the application (the HTML element) it is referred from.
Controllers can have properties and methods.

- The ng-repeat directive repeats an HTML element.

- The ng-disabled directive binds AngularJS application data to the disabled attribute of HTML elements.

- The ng-show directive shows or hides an HTML element.
- The ng-hide directive hides or shows an HTML element.

- The ng-click directive defines an AngularJS click event.

// Filtros
- currency: Format a number to a currency format.
- filter: Select a subset of items from an array.
- lowercase: Format a string to lower case.
- orderBy: Orders an array by an expression.
- uppercase: Format a string to upper case.

// Services
- AngularJS $http is a service for reading data from web servers. $http.get(url) is the function to use for reading server data.

// Miscelaneo / Trucos
- You can use data-ng-, instead of ng-, if you want to make your page HTML5 valid.
- Using ng-init is not very common. You will learn a better way to initialize data in the chapter about controllers.
- A web page can contain many AngularJS applications, running in different elements.
- A common advise for HTML applications, is to place all scripts at the very bottom of the <body> element. But, in many AngularJS examples, you will see the library being loaded in the <head> element. This is often done because calls to angular.module can only be compiled after the library has been loaded. Another solution is to load the AngularJS library in the <body> element, but before your own AngularJS scripts