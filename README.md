# Microfrontend using Webcomponent

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.2.1.

Microfrontend is an architectural approach for frontend where features has broken down into small independent deployable units. for detail information read here [Micro frontend Curry](https://levelup.gitconnected.com/micro-frontend-curry-506b98a4cfc0)

## Demo

You can find working demo on Netlyfy, check this here [Microfronend](https://microfrontend.netlify.com/) and to check the single, independent running feature, click here  [microfrontend-team-movies](https://microfrontend-team-movies.netlify.com)


## Why Web Component approach
There are many variants avaliable to implement Microfrontend, like, Web component based,  JS run-time integration, Server side integration using ESI, SSI using Fragments and some streaming server like Tailor.js, etc.

We have choosen Web component based approach becuase we think its fit into the Frontend boundries. Also, its evident with current industry trends that companies are now moving towards technology agnostic solutions, and using web component you can meet this requirement quickly. 

## How this approach works

We have choosen Angular as a framework of choice becuase in its v8 you have direct access to Angular Elements, which later complies into webcomponent. Please see below section for more detailed information 

## High Level Design
There are four major challenges one need to solve to implement Microfrontend as a design solution. Lets quickly see what those are and how we solved it in our design

1. **Independent development of feature/modules :** With the use of sub-application CLI command Angular supports independent feature development . Using [Angular CLI](https://angular.io/guide/file-structure) we can create multi sub applications in a single project. This very much looks like a mono-repo structure. 
 
 ![Logical structure](https://1.bp.blogspot.com/-U6yrliNYzxs/Xfyla62jgmI/AAAAAAAAMf4/C2z-Q0RKc_wmjP89J0HD75LQJPGXq9QzQCK4BGAYYCw/s1600/hld.png)

2. **Integration of feature/modules in a common shell :** There are multiple ways you can integrating feature apps into a common app. In our approach we are integrating feature/modules at run time. Application Bundling approach - stitching feature app's together

![Bundling](https://4.bp.blogspot.com/-DjBLjUGz23c/Xfylk6tW5QI/AAAAAAAAMgA/04o0M653f5QwE2wRLqwohJPHAfbwfqroQCK4BGAYYCw/s1600/app-bundling.png)

3. **Inter-communication between feature/modules :** There are many patterns avaliable to do communication between different parts of application like HTML5 PostMessage API, Pub-sub based EventBUS, local storage, etc. In our design we have selected Pub-sub approach as its more robust and reactive way of doing communication.

4. **Independent deployment of feature :** There are CLI commands avaliable to run and deploy independent feature apps.

## Features
1. **WebComponents** using Angular Elements
2. **Individual features Development** - created Sub applications using [Angular CLI](https://angular.io/guide/file-structure)  
3. **Independent Deployment for scalability** - Can deploy feature independently 
4. **Cross feature communication** - Custom event bus using pub-sub design pattern
5. **Ease in setup** - Client side dynamic integration of Apps 


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

## Thank you
Special thanks to Tarun Kumar Sukhu for valuable feedback given throuhout the design excercise.

## License

MIT
