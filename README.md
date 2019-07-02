# NgMdStarter

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.3.4.

## Installation

Clone the project by using ssh `git clone git@github.com:mrpharderwijk/ng-md-starter.git` or https `git clone https://github.com/mrpharderwijk/ng-md-starter.git`. Then run `npm install` to install all dependencies. To run the application locally see below at the Development server section.

## Development server

Run `npm run serve:local` for a dev server. Navigate to `http://localhost:4203/`. The app will automatically reload if you change any of the source files. Use `npm run serve:prod` for a check for prod build/server.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `npm run build` to build the project. The build artifacts will be stored in the `dist/` directory. Use `npm run postinstall` for a production build.

## Running unit tests

Run `npm run test` to execute the unit tests via [Karma](https://karma-runner.github.io). Run `npm run coverage` after that to start the coverage server and check the reports by navigating to `http://localhost:9875`.

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Custom starter stuff

Changes made in:

- added `./.prettierignore`
- added `./.prettierrc`
- `./angular.json`
  - added `stylePreprocessorOptions` rules for custom general scss files
  - added `local`-build and `local`-serve rules
- `./tslint.json` refers to a `./custom-tslint.json` file with all the rules in it
- `./src/styles.scss` added a reference to the custom general scss file (`_main.scss`)
- `./package.json`
  - added/adjusted in scripts
    - `build` with aot build
    - `coverage` run the test coverage server
    - `postinstall` aot production build
    - `pretty` prettify all ts source files
    - `serve:local` aot local serve, running on port 4203
    - `serve:prod` aot production serve, running on port 4203
    - `start` runs the application with express.js from the `dist`-folder
    - `test` runs the tests with coverage and watch mode on
  - `pre-commit` hooks added
  - `dependencies` and `devDependencies` updated
