# [https://nodejs.org/en](Node.js) Tutorial

In this tutorial, you will learn the basics of Node.js and how to start building web applications using this server-side JavaScript runtime environment.

![NodeJs in 5](https://www.youtube.com/watch?v=_h-pj7YqHQw&t=206s&ab_channel=Jayanam)

## Installing Node.js

To get started, you'll need to install Node.js on your machine. You can download the latest stable version from the official Node.js website: [nodejs.org](https://nodejs.org).

## Creating a Node.js project

Once you have installed Node.js, you can create a new Node.js project using the following command in your terminal:

## Creating a package.json file

The `package.json` file is a fundamental file in any Node.js project. This file contains metadata about your application, such as the name, version, description, authors, dependencies, and more.

To create a `package.json` file, you can use the `npm init` command. This command will guide you through a series of questions to help you set up your `package.json` file.

```bash
npm init
```

What is the package-lock.json file?
The `package-lock.json` file is automatically generated when you install packages via npm. This file contains detailed information about your project's dependency tree, including the exact versions of each package that has been installed.

This file is important because it ensures that everyone working on the project is using the same package versions, helping to prevent errors and discrepancies.

Installing packages
To install a package in your Node.js project, you can use the `npm install` command. For example, if you wanted to install the express package, you could do so with the following command:

```bash
npm install express
```

This will install the `express` package in your project and add an entry in the `package.json` file under the dependencies section. It will also generate or update the `package-lock.json` file with the exact version of the installed package.

## What is the package-lock.json file?

The `package-lock.json` file is automatically generated when you install packages via npm, the Node.js package manager. This file contains detailed information about your project's dependency tree, including the exact versions of each package that has been installed.

Its main purpose is to ensure that the structure of the `node_modules` folder is identical across all installations, regardless of intermediate package updates. This is achieved by specifying an exact version, location, and integrity hash for each package and subpackage in your project.

### Why is the package-lock.json file important?

1. **Consistency**: It ensures that everyone working on the project is using the same package versions, helping to prevent errors and discrepancies caused by differences in package versions.

2. **Efficiency**: By having a detailed record of the exact structure of the `node_modules` folder, npm can avoid unnecessary network requests when installing packages, which can speed up the installation process.

3. **Security**: The `package-lock.json` file includes integrity hashes for each package, allowing npm to verify that the packages have not been altered since they were installed.

### Should the package-lock.json file be included in version control?

Yes, it is recommended to include the `package-lock.json` file in your version control system. This ensures that everyone working on the project uses exactly the same package versions, helping to maintain consistency and prevent errors.

## [https://vitejs.dev/](Vite)

### What is Vite and how does it work?

Vite is a development environment for modern web applications that focuses on speed. It works by changing the way web applications are developed and served during the development process.

Instead of compiling all the code before serving it to the browser, as other frameworks like Webpack do, Vite uses ESM (ECMAScript Modules) to serve modules directly to the browser during development. This means that the code is compiled and served incrementally and on-demand, resulting in fast build times and an agile development experience.

![Vite in 5 minutes](https://www.youtube.com/watch?v=KCrXgy8qtjM)

### Managing environment variables in Vite

Vite allows managing environment variables through .env files. Here's an example of how to do it:

```env

VITE_API_URL=https://api.example.com
VITE_DEBUG=true

```

By prefixing each variable with `VITE_`, there is no need to use a package like `dotenv` to handle environment variables.

## [https://es.react.dev/](React)

![React in 5 minutes](https://www.youtube.com/watch?v=s2skans2dP4&ab_channel=DennisIvy)

## Installing React

To install React, you'll need to have Node.js and npm installed on your machine. Once you have them, you can install `create-react-app`, which is a command-line tool that allows you to create new React projects.

```bash
npx create-react-app my-app
```

This command will create a new directory named `my-app` with an initialized React project.

## Creating a React project

To create a new React project, you can use the `create-react-app` command followed by your project name. For example, if you wanted to create a project named `my-react-app`, you could do so with the following command:

```bash
npx create-react-app my-react-app
```

This will create a new directory named `my-react-app` with an initialized React project. Inside this directory, you'll find various files and directories that form the basic structure of a React project.

To start your application, navigate to your project directory and run the `npm start` command:

```bash
cd my-react-app
npm start
```

This will start the development server and open your application in a web browser.

Although this is the way to create a normal project, in our case it is not necessary to use them, but it is important to know it for our future project creation.

## npx vs npm

`npm` and `npx` are two tools that come with Node.js, but they are used for different purposes.

**npm** (Node Package Manager) is the default package manager for Node.js. It is used to install and manage Node.js packages. When you install a package using `npm install`, that package is downloaded and stored in your `node_modules` directory, and you can require it in any file in your project.

On the other hand, **npx** (Node Package Execute) is a tool used to execute Node.js packages. `npx` comes with npm 5.2+ and above. The main difference between `npm` and `npx` is that `npx` runs packages without the need to install them beforehand.

For example, if you wanted to use the `create-react-app` tool to create a new React application, you could do so with `npx` without needing to install `create-react-app` globally on your machine:

```bash
npx create-react-app my-app
```

In summary, `npm` is for installing and managing your dependencies. `npx` is for executing your packages.

## How to run the project from this repository

Once the repository is cloned and after running `npm install` to install dependencies, to activate the application we run `npm run dev`.

The declaration of these scripts can be seen in the `package.json`.

```json
  "scripts": {
    "dev": "vite",
    "build": "tsc && vite build",
    "lint": "eslint . --ext ts,tsx --report-unused-disable-directives --max-warnings 0",
    "preview

": "vite preview"
  },
```

If we want to view the project the same way it would look on a real server, we use `npm run build` which will create the files of our application in its live version.
