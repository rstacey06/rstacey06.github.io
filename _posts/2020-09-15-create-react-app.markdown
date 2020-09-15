---
layout: post
title:      "create-react-app "
date:       2020-09-15 13:36:20 +0000
permalink:  create-react-app
---


   If you've tried to set up a React App from square one, You know it can be quite pain staking, there are multipule tools you must know how to use and configure before we even begin to program our actual Apps code. Fourtunally for us, we have this cool create-react-app tool that was created by facebook devlopers to help simplify the process! 
	
 Create-react-app is a tool that gives us a head start when building our React apps. It saves on that time consuming configuration and setup by running just one command that will set up all the tools you need to start your React  App. Lets take a look! 
	 
 First thing we need to do is install the create-react-app npm package globally in our computer. We can do this by running the following command in our terminal: 
	 
```
 npm install -g create-react-app  
```
	 
 Easy enough right?! Now that we have installed our create-react-app tool, we can create our React App: 
	 
```
 npx create-react-app my-app 
```
	 
 We use the npx create-react-app command PLUS what we want to name our app(in this instant my-app). This will install all of our packages and output a list of difrent commands we can now run, this will also get out React app running at our http://localhost:3000/. 
	 
 Along with installing our packages and setting up our local, the create-react-app has four default commands bundled into it: start, test, build, and eject. 
	 
 start - enables you to start the server 
 
 test - enables you to launch the test runner in  interactive watch mode
 
 build - ensures that the finished project is bundled, minified and optimized with the best practices
 
 eject - will remove the single build dependency from your project
	 
Also with this, create-react-app uses Yarn by default insted of NPM. Here's a break down: 

```
   npm run build OR yarn build
```
Essentially, it's taking all of our JavaScript code that can't be interpreted without help and turned into a smaller version or 'minified' version that the browser and read. It reduces the file down as much as it can to speed up the download time and creates a build directory. This directory will have the bundled .js and index.html files. Since the index.html is supposed to be served with a static file server, we cant open the index.html in the browser, most React Apps use client-side routing so we cant do that with file://URL. 
  
```
npm test OR yarn test 
```
This will start the test runner
  
```
npm run eject 
```
Per the React docs: “If you aren’t satisfied with the build tool and configuration choices, you can eject at any time. This command will remove the single build dependency from your project. Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except eject will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.”
Essentially this pulls our app out of the context of the create-react-app framework and into a standered webpack build. 

We can also change our development server port from 3000 if we need to. To do so, make a file called .env in the root of your project, then set the port number you'd like:` PORT = 3001 `

The create-react-app cli is a very powerful tool we can use to help ease the difficulties of getting started on a React app. Use the create-react-app command to start your applications to provide a solid base! 


