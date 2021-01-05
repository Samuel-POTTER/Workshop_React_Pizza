
---
title: My first React application
 

author: Samuel POTTER, Donovan FONTAINE

version: 1.29

---

  

## Introduction

React is a javascript framework designed to improve and simplify the web development. 
  During this workshop, you are going to learn the **basics** of React.
  * Create your first webpage
  * Learn **fundamentals** (states, hooks, useEffect, useState, arrow function)
  * Get data from a json file and display it on the page
  
### prerequisites:
* Basic knowledge of HTML    

## Step 0 - Setup

  * Check if you have **node.js** installed.
	`node --version`
	
	If it's not installed:
	**node**: https://nodejs.org/en/download/package-manager/

* **Create your project**:
```js
npx create-react-app workshopreact
``` 
It may take a few minutes for the creation of the project. Use this time to check some basics of **HTML**. 
https://jaetheme.com/balises-html5/

* When it's done `cd` inside the folder and execute: 
````bash
npm start
````

Welcome to your **localhost3000/**.
 
 If all the previous step worked fine, you should see a react animated logo on your browser.
 
## Step 1 - Hello World

It's time to get rid of the code inside of the `App.js`. It should look like this/
```js
 function  App() {
	return (
		<p>
			Hello World !
		</p>
	);
}

export  default  App;
```

  **Seems pretty easy isn't it ?** 

  Now we will see how to display content from another file and what is an arrow function.
  Create a **Hello.js** file. 

This is the basic way to create a function: 
```js
function Hello() {
	return (
		<h1>
			Hello World !
		</h1>
	);
}
export default Hello;
```  
This is how the same function looks in an arrow function: 
```js
const Hello = () => {
	return (
		<h1>
			Hello World !
		</h1>
	);
}
export default Hello;
```

Now how are you going to use this function inside your **App.js** ?
*tips: man google import in react*

## Step 2 - Navbar

  To beautify our website, we are going to use **Materialize**.
  ```bash
npm install --save materialize-css@next
```
https://materializecss.com/getting-started.html

Create a folder named `img` inside your `src` folder. Past the images provided inside or use yours. 
**Materialize** provide a simple way of creating a navbar. It's magic.
https://materializecss.com/navbar.html
Copy and past the navbar of your choice in your `App.js`. You will only need **3 redirections**. 
* Home
* Menu
* Contact

Change the code to have the required expectation.

![alt text](https://image.noelshack.com/fichiers/2021/01/1/1609746180-navbar.png)



## Step 3 - Create your pages

Now that we have our navbar, we would like to have content in each pages. For this, create **3 js file** in `src`
* Contact.js
* Home.js
* Menu.js

Each pages will display a unique message of the file.

Now how are you going to swap between each page ? Try to figure out how to use **Router**
https://reactrouter.com/web/api/Link

## Step 4 - Time to order

In order to display data in your menu page, you need to get it from the **json** previously provided.
Remember **step 1**, on how to import things in your file.
When it's done, try to display the first pizza info in your HTML (name, price, ingredients). 

![alt text](https://image.noelshack.com/fichiers/2021/01/2/1609842813-regina.png)

Good job mate, you've displayed your first pizza. Now how can we display all of them at once ?
*tips: https://fr.reactjs.org/docs/lists-and-keys.html*


![alt text](https://image.noelshack.com/fichiers/2021/01/2/1609843429-menui.png)


Now you can use **materialize** to beautify the content or you can use **packages** to have better content.
https://www.npmjs.com/package/react-ui-cards 

 ![alt text](https://image.noelshack.com/fichiers/2021/01/2/1609847849-final.png)
 
 
 ## GO FURTHER

**Congratulation**, you succeed your first react application. 
To improve your knowledges you can read the documentation.

The code you write in react will only implement the so-called business logic. In other words, your main job will be to write glue between selected software components to complete the requested project. Instead of building everything from scratch, don't hesitate to google things to find packages, template etc...
https://www.npmjs.com/ can be very useful.
