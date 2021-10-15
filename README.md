
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
```

## What is NgRx about?

According to [NgRx docs](https://ngrx.io/docs#what-is-ngrx)

> NgRx is a framework for building reactive applications in Angular. NgRx provides libraries for:
> 
> -   Managing global and local state.
> -   Isolation of side effects to promote a cleaner component architecture.
> -   Entity collection management.
> -   Integration with the Angular Router.
> -   Developer tooling that enhances developer experience when building many different types of applications.

 
Check this [diagram](https://ngrx.io/docs#what-is-ngrx)
[<img src="https://ngrx.io/generated/images/guide/store/state-management-lifecycle.png">](https://ngrx.io/generated/images/guide/store/state-management-lifecycle.png)


