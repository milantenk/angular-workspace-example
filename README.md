# Angular workspace demo

This workspace was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.2.3.

The goal of this repo is to demonstrate an Angular workspace with a library and a consumer. It is used as demo for this [stackoverflow question](https://stackoverflow.com/questions/58997143/why-cant-i-build-an-angular-app-that-references-an-internal-angular-library).

## Build and Serve
After calling `npm install` run `npm run build:lib` and after that `npm run start`.

## Creating such a workspace
Do following steps to create a workspace structure like this.
- Create the workspace with following command:
```bash
ng new my-workspace --create-application=false
```
- Navigate into the newly created workspace:
```bash
cd my-workspace
```
- Generate the library:
```bash
ng generate library my-lib
```
- Generate the application:
```bash
ng generate application my-app
```
- Add `MyLibModule` to the `app.module.ts` of the application.
- Update package.json with `build:lib` and `build:app` commands.
