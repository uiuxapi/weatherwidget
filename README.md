# Weatherwidget

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.9.

## Generating Lib
Run `ng generate library weather` The Angular-CLI will create a directory called projects and within projects create a libary called weather.

## Public APi
Inside the projects directory at a couple directories in `projects/weather/src/public-api.ts`, you will find a public-api.ts which marks the location for the public api, where you can add your re-usable angular code.

## Build Lib
Run `npm run build-lib` The terminal / command prompt will display Building Angular Package. The following script tag from package.json is used.

` "build-lib": "ng-packagr -p projects/weather/package.json",`

## Build and Watch for Changes
Run `npm run build-lib-watch`  The terminal / command prompt will build the library and watch for changes. The following script tag from package.json is used.

` "rebuild-lib": "ng-packagr -p projects/weather/package.json --watch",`

## Publish Lib to Github Package Repository
Run `build-lib-publish` This will execute the following script to build and publish to the github package repository.

 `"build-lib-publish": "ng build weather && cd dist/weather && npm publish",`

## Install Packaged Lib
Run `npm install weather/dist`

## Library Usage
In the app.module.ts or core.module.ts import the library  `import { WeatherModule } from '@uiuxapi/weather';` and also add the library to the imports array `imports:[ WeatherModule ]`.  The items exported in the public api are now ready for use in the application.

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
