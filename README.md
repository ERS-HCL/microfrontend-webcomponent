# MicrofrontendWebcomponent

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.2.1.

Microfrontend is an architectural approach for frontend where features has broken down into small independent deployable units. for detail information read here [Micro frontend Curry](https://levelup.gitconnected.com/micro-frontend-curry-506b98a4cfc0)

## Demo

You can find working demo on Netlyfy, check this here [Microfronend](https://microfrontend.netlify.com/) and to check the single, independent running feature, click here  [microfrontend-team-movies](https://microfrontend-team-movies.netlify.com)

## Features
1. **WebComponents** using Angular Elements
2. **Individual features Development** - created Sub applications using [Angular CLI](https://angular.io/guide/file-structure)  
3. **Independent Deployment for scalability** - Can deploy feature independently 
4. **Cross feature communication** - Custom event bus using pub-sub design pattern
5. **Ease in setup** - Client side dynamic integration of Apps 

## High Level Design
![Logical structure](https://1.bp.blogspot.com/-U6yrliNYzxs/Xfyla62jgmI/AAAAAAAAMf4/C2z-Q0RKc_wmjP89J0HD75LQJPGXq9QzQCK4BGAYYCw/s640/hld.png)

## Inter App Communication Design
![Cross communication](https://miro.medium.com/max/876/1*QusqsahREktw7OdFg5nVsg.png)

## Application Bundling approach - stitching feature app's together
![Bundling](https://4.bp.blogspot.com/-DjBLjUGz23c/Xfylk6tW5QI/AAAAAAAAMgA/04o0M653f5QwE2wRLqwohJPHAfbwfqroQCK4BGAYYCw/s640/app-bundling.png)


## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## License

MIT
