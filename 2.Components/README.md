# Module 2: Components

In this module we will learn about Angular Components. 

### What is a component?

In Angular 2, *everything is a component*. Components are the main way we build and specify elements and logic on the page, through both custom elements and attributes that add functionality to our existing components.

### Let's look at what we have so far

We have created our first application but we never actually opened the project to check out what *Angular* created for us so let's do that for now

#### Step 1: Open up Visual Studio Code

On the `top left` corner click the *Explorer* icon -> ![ExplorerIcon](https://github.com/microsoft-dx/angular2-fundamentals/blob/master/Images/module-2-1.PNG) and *Open* the folder that we created in the last module.

#### Step 2: Explore the Solution

Go to `src->app` and let's see what we have here. You can see that each file starts with `app.component`. This is a default component that Angular built for us so let's look at it closer. 

Let's look at `app.component.ts`

![First Component](https://github.com/microsoft-dx/angular2-fundamentals/blob/master/Images/module-2-2.PNG)

In our component, we can see that we have a bunch of atributes.

* `selector`
  If we want to call this component to a view, we do that by adding the `<app-root>``</app-root>` tags.
  
* `templateUrl`
  This is the path to our HTML file so that Angular knows what to add to the DOM.
  
* `styleUrls`
  An array of urls for the various css files that we need.
  
Looking further down, we must remember that this is still a `TypeScript` file. We define a model for our view as our `AppComponent` class. For now, we can see that it only has a *title* property and we'll leave it at that for now.

![Model](https://github.com/microsoft-dx/angular2-fundamentals/blob/master/Images/module-2-3.PNG)

Another important aspect is our `View`. We can see that Angular created a view for us (`app.component.html`). 

![View](https://github.com/microsoft-dx/angular2-fundamentals/blob/master/Images/module-2-4.PNG)

Let's look at the first `div` tag. We can see that we have the following text:

`Welcome to {{title}}!`

Any clues what {{title}} is? It is the actual property from the class that we defined earlier.

In *Visual Studio Code*, open up `app.component.ts` and inside our `AppComponent` class change the title property's value to anything that you wish. 

Click [here](http://localhost:4200/) and see what happens. 

*Bonus!* As I said earlier, the server that we started with `ng serve` watches our files and compiles the ones that we modified in real time so let's check that out. Minimize the text editor, make a change and then watch what happens when you actually save the file.

![HelloWorld2](https://github.com/microsoft-dx/angular2-fundamentals/blob/master/Images/module-2-5.PNG)

Great! Now that we know more about modules, let's create some of our own in the next module!

[Module 3: Creating your own Components](https://github.com/microsoft-dx/angular2-fundamentals/blob/master/3.Creating-Components/README.md)
