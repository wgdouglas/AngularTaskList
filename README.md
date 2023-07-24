# AngularCrash

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