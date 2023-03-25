---
title: "Lightning Fast React Apps with Vite: A Comprehensive Guide"
datePublished: Sat Mar 25 2023 08:04:15 GMT+0000 (Coordinated Universal Time)
cuid: clfnoqmep000009jt5veeeo1q
slug: lightning-fast-react-apps-with-vite-a-comprehensive-guide
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1679731069359/22825063-f0af-4bcd-8a35-2a1965b7c3d9.png
tags: web-development, reactjs, vite

---

If you're a web developer, you might have heard of Vite. It's a relatively new tool that has taken the world by storm. Vite is a build tool that's designed to be fast, lightweight, and easy to use. In this blog post, we'll be discussing Vite and how to create React apps using it.

# What is Vite?

Vite is a build tool that's designed to be fast and lightweight. It's built on top of ESbuild, a fast and efficient bundler. Vite allows you to develop your web apps with lightning-fast HMR (Hot Module Replacement) and build them with a single command. Vite is also optimized for tree-shaking, which means that it only includes the code that's actually used in your app, resulting in a smaller bundle size.

### Vite's features include:

* Fast development server with HMR
    
* Lightning-fast build times
    
* Support for TypeScript, CSS preprocessors, and JSX out of the box
    
* Optimized for tree-shaking
    
* Easy to configure and use
    

### How to create a React app using Vite:

Creating a React app with Vite is straightforward. To get started, you'll need to have Node.js and npm installed on your computer.

### Step 1: Create a new React app.

To create a new React app with Vite, you can use the following command:

```powershell
npx create-vite-app your-app-name --template react
```

This will create a new React app with Vite, and install all the necessary dependencies.

### Step 2: Start the development server.

To start the development server, navigate to your project directory and run the following command:

```powershell
npm run dev
```

This will start the development server, and you should see a message in your terminal that says "Server running at [**http://localhost:3000**](http://localhost:3000)".

### Step 3: Create your React components.

You can create your React components in the `src` directory. By default, Vite comes with a `App.jsx` component, which is the root component of your app. You can modify this component or create new ones to build your app.

### Step 4: Build your app.

When you're ready to build your app, you can run the following command:

```powershell
npm run build
```

This will create a production-ready build of your app in the `dist` directory.

### Step 5: Deploy your app.

You can deploy your app to any hosting service that supports static sites. One popular option is Netlify, which offers a free plan for static sites.

### Step 6: Fix paths.

If all the links in your React app built on Vite start with a forward slash (/) instead of a dot (./), it is likely because your Vite configuration is set up to use absolute paths instead of relative paths.

To fix this, you can modify your Vite configuration to use relative paths instead of absolute paths. Here's how:

* Open your Vite configuration file. This is typically named `vite.config.js` and should be located in the root directory of your project.
    
* Add the following code to your `vite.config.js` file:
    
    ```powershell
    export default {
      base: './',
    };
    ```
    
    This sets the `base` option to `'./'`, which tells Vite to use relative paths instead of absolute paths.
    
* Save the `vite.config.js` file.
    
* Restart your development server.
    

After completing these steps, all of the links in your React app should use relative paths starting with `./` instead of absolute paths starting with `/`.