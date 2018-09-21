#1. Introduction

Full Stack Shopping Cart With MEVN Stack 

VueJS 2.0 Nodejs Tutorial is today’s main topic. NodeJS is a viral platform nowadays because of its features and Express is a web framework build on top of Node.js. This is the perfect example of How to use VueJS with NodeJS.

One possible reason I am writing this is showcase how Node.js, Express Framework,MongoDB and modern client-side Javascript frameworks (Vue.js with Webpack) can all play nicely together. Express is still the dominant Node.js web framework.

#Step 1: Make a directory for this Project.

First we need to create a directory which will contain both folders Client and Server

Install Express Generator


Now we’re going to install Express, which is a framework that takes Node from a barebones application and turns it into something that behaves more like the web servers we’re all used to working with. We need to start with Express-Generator, which is actually different than Express itself … it’s a scaffolding app that creates a skeleton for express-driven sites. In your command prompt, type the following:

npm install -g express-generator


This command will install express-generator globally, So let’s use our generator to create the scaffolding for a website.

express server


Now we have some basic structure in there, but we’re not quite done. You’ll note that the express-generator created a file called package.json in your server directory which is a basic JSON file describing our app and its dependencies

Right now we need to install our dependencies by running this command

npm install 


It’s going to print out a ton of stuff. That’s because it’s reading the JSON file we just installing all the stuff listed in the dependencies object

You now have a fully-functioning app ready and waiting to run, so let’s test out our web server! Type the following:

npm start


Everything working? Awesome! Open a browser and head for http://localhost:3000 where you will see a welcome to Express page.

#Step 2: Create Products and Categoies Models.


Now, we need to create one folder in a root called models which will contain two file js for products schema and categories schema both.

#Connect to MongoDB


Mongoose requires a connection to a MongoDB database. You can require() and connect to a locally hosted database with mongoose.connect(), as shown below.

#FAKERIZATION

Using Faker.js


Now we need to add much data to our products and categories models, for that we want to use faker.js to get some random data

Let’s start by creating a folder in routes directory called seeder which will contain products.js file, where were going to store some random data to products and categories.


