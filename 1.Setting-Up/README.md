# Module 1: Configuration & Routing

In this module we will install Angular 2 and get it set up to a basic configuration, based on their own [quickstart](https://angular.io/guide/quickstart).

The [Angular CLI](https://cli.angular.io/) is a *command line interface*(`CLI`) tool that can create a project, add files, and perform a variety of ongoing development tasks such as testing, bundling, and deployment.

The goal in this module is to build and run a simple [`Angular`](https://angular.io/) application in [`TypeScript`](https://www.typescriptlang.org/), using the Angular CLI while adhering to the Style Guide recommendations that benefit every Angular project.

If you are new to [TypeScript], I suggest you check out our [repo](https://github.com/microsoft-dx/typescript-fundamentals) before pursuing this course. 

### Step 1: Set up the Development Environment

Before doing anything, we have to set up our Development Environment.

Prerequisites:

- [Node.js](https://nodejs.org/en/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Git Bash](https://git-scm.com/downloads)

Then install [Angular CLI](https://cli.angular.io/) globally. Open up a `cmd`/`PowerShell` and type in:

>npm install -g @angular/cli

### Step 2: Create a new project

Open a `terminal window` in a folder that you created for your project and create a new project typing in:

>ng new my-first-app

### Step 3: Get your new application running

Go to the project's directory and launch the server

>cd my-first-app
>ng serve --open

The awesome thing about `ng serve` is that not only it launches your server, but also watches your files and rebuilds the application as those files are changed. What does this mean? You don't have to compile and recompile endlessly as you develop your aplication, you can just watch it change as you write your code.

### Step 4: Check out your application in your browser

Our `serve` command looked like this:
>ng serve --open 

The fact that we added the additional oprion `--open`, or we could have used `-o` as well, opened up a new tab in our browser that looks something like this:

![module-1-1]()

*Congratulations!* 
You have just built your first Angular app!
