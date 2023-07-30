# AngularCrash-TaskList

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 16.1.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

### This project has simlpe CRUD

## Header & button setup

Start by using `ng g c <pathName/comnponentName>` to create the coponents for both header & button components.

- We'll be first passing our header component root path into our main html component

- Using string interpolation place the title variable inside of our header component then also use our root path of our button component inside to pass our button into the header

## Adding the Task's

- We'll have a task coponent & item for each item 
- This will come from JSON Server (which is a fake Rest API that we can create & run locally)
- This will just export our task's and set them into an array of objects with custom values
- We also want to create an interface for the tasks like what specific fields should the model contain

## Creating a Delete Icon and it's functionality
- You can use an angular package called `Font-Awesome` (https://github.com/FortAwesome/angular-fontawesome)
- For this since we have the latest angluar we can just use the add command of `ng add @fortawesome/angular-fontawesome`
- Our current goal is to create a click function inside of our task-item component & set the method `deleteTask()` to be passed in which we will pass in that index of task inside of our `ts` file to view it on each click inside of our console in the browser
- Next we need to use an observable and eeventEmmitter to be able to collect the information on each click of the delete button
- from here we will now pass in another new method inside of our task-component in which we'll be passing in our previous method from our task-item component and assigning our property of `task` to it.
- Now inside of our task.ts file we'll set our method of deleteTask & pass in our index of task since we're only aiming to delete just the one instance of that index from our array

## Creating a Add button and it's functionality
- This section is going to be started bt first adding our `add-task` component, then we will add our styling's by using `form-control` & passing in a label & input
- with this we'll add stylings in each with an id, name, placeholder and class
-Now when working with forms we want to put a property in for each of our filed's of 'day, text, & reminder' which we'll add these properties inside of our `add-task`.ts file but make sure that reminder is passed as a boolean since it only hold's a boolean value
- for setting up our properties to have two-way data binding with our inputs we'll utalize the `ngMoldel` directive from our forms module which we first have to add to our `app.module.ts`
- Now for two-way data binding we use brackets for input & we use parenthesis for event binding but for this we will be using both in order to properly use  `ngModel` directive & set it to the name property of each input & make sure that the attributes have the same name value per input

