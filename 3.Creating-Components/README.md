# Module 3: Creating Components

We learnt in the last module what are the components of components *`hihi`* but now we are going to create one of our own!!

Let's say that we want a component that has an input link for an image and it automatically loads it to our page

## Step 1: To our app folder, add a `TypeScript` file.

Go to app -> new file -> name it imageupload.component.ts

## Step 2: Import the Component Object

![ImportComponent](https://github.com/microsoft-dx/angular2-fundamentals/blob/master/Images/module-3-1.PNG)

Angular 2 make use of the [ES2015 module syntax](http://exploringjs.com/es6/ch_modules.html) (also known as ES6). For those unfamiliar with the syntax, it makes use of `import` statements to access different pieces of code. In addition the these `import` statements, this syntax also relies upon `export` statements to make code accessible to the rest of our application.

#### Below, we can check out some of the other [APIs](https://angular.io/api) that are central to developing web applications in Angular 2.0.

- [@angular/http](https://angular.io/api/http/Http) - For making HTTP requests
- [@angular/common](https://angular.io/api/common) - Common core things including form validation
- [@angular/router](https://angular.io/api/router) - Routing for our entire app

### [@angular/http](https://angular.io/api/http/Http)

As you may have guessed, this library gives us access to all of Angular 2's functionality regarding http requests. The following script is required when using the http library.

```html
<script src="node_modules/@angular/bundles/http.dev.js"></script>
```
### [@angular/forms](https://angular.io/api/forms)

The [@angular/forms](https://angular.io/api/forms) is frequently used to deal with [form building](https://angular.io/guide/forms). This library holds lies `FORM_DIRECTIVES` constant which gives developers access to important directives like [NgForm](https://docs.angularjs.org/api/ng/directive/ngForm) and [NgModel](https://angular.io/api/forms/NgModel).

### [@angular/router](https://angular.io/api/router)

The `@angular/router` libraries hold all of the code necessary to implement client-side routing. The following script is required:

```html
<script src="node_modules/@angular/bundles/router.dev.js"></script>
```

## Step 3: Add Meta-data to our Component using TypeScript Decorators

Once the `Component` object is imported, we can then begin describing our component using TypeScript's `@` symbol.

![Component](https://github.com/microsoft-dx/angular2-fundamentals/blob/master/Images/module-3-2.PNG)

*Hint*: You have this `.ts` file inside of this repository, no need to type everything by hand

### Angular Metadata

The whole point of the meta-data is that we can specify the compiler how we want it to *interpret* our component. There are many configuration options but we are going to go only through the ones that we actually use:

* **selector** - defines the name of the HTML tag where this component will live. In this case, our component will by shown through the <my-app></my-app> tags.

* **directives** - We use the directive option when we want to access another component directive. Because this is the top-level component, we often see components being passed into this option, and we will see how this works shortly.

* **styles** - The styles option is used to style a specific component. One of the advantages of using components is their ability to encapsulate their styles. We could have just as easily linked to an external stylesheet by using the *styleUrls* property. We should note that an array of stylesheets can be passed into this option.

* **template** - This is the portion of our component that holds our template. It is an integral part of the component as it allows us to tie logic from our component directly to a view. When defining a template, we can either write it inline, or we can opt to use *templateUrl* to link to an external template.

Now that we've defined all the parts of our component, the last step is to export it so it can be used in other parts of our application.

## Step 4: Export the Component

The exported class is where we can define any variables or functions that our component's template will be using:

![ExportedComponent](https://github.com/microsoft-dx/angular2-fundamentals/blob/master/Images/module-3-3.PNG)

By using the `export` statement, this component can be imported into different files in a project so it is a pivotal part of *Angular 2*.
