
  

# NgrxSandbox

  

## First steps

  

Generate a project like this by running

  
  

ng new your-project-name

yarn

ng serve --open

git init

git status

git add .

git config --get user.name

git config --get user.email

If the username and email don't match the ones you want to use in your Github repository, run the commands below.

git config user.name "Your name"

git config user.email "your@email.com"

Make sure to create a repo over Github.

git remote add origin https://github.com/[your-name]/[your-project-name].git

git branch -M main

git push -u origin main

  

It is now time to add the ngrx specific stuff

  

```

yarn add @ngrx/store
ng add @ngrx/store-devtools            

```
Make sure to add StoreDevtoolsModule.instrument() to the app.module.ts imports, as it is necessary for running the dev tools.

## What is NgRx about?

  

According to [NgRx docs](https://ngrx.io/docs#what-is-ngrx)

  

> NgRx is a framework for building reactive applications in Angular. NgRx provides libraries for:


>  - Managing global and local state.

>  - Isolation of side effects to promote a cleaner component architecture.

>  - Entity collection management.

>  - Integration with the Angular Router.

>  - Developer tooling that enhances developer experience when building many different types of applications.

  

Check this [diagram](https://ngrx.io/docs#what-is-ngrx)

[<img src="https://ngrx.io/generated/images/guide/store/state-management-lifecycle.png">](https://ngrx.io/generated/images/guide/store/state-management-lifecycle.png)

  

## Tutorial

  

This tutorial (over the state-management branch) has been based on the

https://ngrx.io/guide/store/walkthrough.

Create your own branch from main and do the steps from the NgRx website tutorial. Check if everything works.

Make sure to install the ([Chrome](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=pt-BR)) or ([Firefox](https://addons.mozilla.org/en-US/firefox/addon/reduxdevtools/)) dev tools for NgRx.

  

## Watch out

  

Add StoreDevtoolsModule.instrument() to the app.module.ts imports.

Make sure to fix the books.actions and the books.reducer.


## Homework
Try to find out what could be improved over the app.component.ts ngOnInit() method. Is there anything we could do there to make the code more NgRx-like?
