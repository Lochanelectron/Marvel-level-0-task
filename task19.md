# Express Web App – Life Problem Resource Library

## Introduction

For this task I created a small web application using **Node.js** and **Express.js**. 
The idea was to make a simple resource library website. Instead of normal articles or books, I made a funny "life problem library". Users choose a problem and get redirected to a YouTube video that gives a solution.

Example problems include:
- How to get a girlfriend
- How to fart quietly
- How to study the night before exam
- How to eat air
- How to touch grass

Each problem redirects to a related YouTube video.

## Tools Used

- Node.js
- Express.js
- HTML
- Visual Studio Code
- Linux (Fedora)

## Project Structure

The project folder structure is:
life-problem-library
│
├── server.js
├── package.json
└── public
└── index1.html


`server.js` contains the Express server code and routing logic.  
`index.html` contains the webpage that lists the problems.

## How It Works

The Express server runs on localhost and serves the HTML page.  
When a user clicks on a problem, the request goes to a route like:

/problem/1


The server then redirects the user to the corresponding YouTube video.

## Running the App

To start the application I ran:
node server.js

The website can be opened in a browser at:
http://localhost:3000/index1.html


## Conclusion

In this task I created a simple Express web app that works as a humorous resource library.  
This helped me understand how to set up a Node.js project, create routes in Express, serve HTML files, and redirect users to external links.


