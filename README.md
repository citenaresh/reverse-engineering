# Reverse Engineering Code

[![License: MIT](https://img.shields.io/badge/license-MIT-yellowgreen)](https://opensource.org/licenses/MIT)

## Description

This is a reverse engineering task of the files in devlop folder and how the app can be acheived or run, this is to dissect the code for any member of the team related to understand what is going on and how everything works.

## Deployed Google Doc Tutorial: 

https://drive.google.com/file/d/1WEqHfVj3D-o06aFAYTmE9PHt2wXVXQam/view?usp=sharing


## Table of Contents

-   [Installation](#installation)
-   [License](#license)
-   [Files_Explained](#File_Explained)
-   [Authors](#Authors)
-   [Acknowledgments](#Acknowledgments)
-   [Questions](#questions)

## Installation

to begin using this app, please clone this repository into your local storage. Once this is complete, please follow these steps;

1)create a mysql db called "passport_demo" 
2)go into the config file, open config.js and insert your personal data: username, password etc 
3)open terminal in current repo and run "npm install" to install all the node packages 
4)Run "node server.js" in the terminal and you will successfully be connected to the server 
5)open browser and locate to "http://localhost:8080" 
6)enjoy using the app!


## License

    								MIT License

    		Team Profile Generator   Copyright (C) 2021 Naresh Raj Poudel

    		Permission is hereby granted, free of charge, to any person obtaining a copy
    		of this software and associated documentation files (the "Software"), to deal
    		in the Software without restriction, including without limitation the rights
    		to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    		copies of the Software, and to permit persons to whom the Software is
    		furnished to do so, subject to the following conditions:

    		The above copyright notice and this permission notice shall be included in all
    		copies or substantial portions of the Software.

    		THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    		IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    		FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    		AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    		LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    		OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    		SOFTWARE.


## Files Explained

--PASSWORD AUTHENTICATION--

This app allows users to create an account, log into and out from the account securely. All the data (users) is stored in  mysql database.

--TECH USED --

-bbcrypts, express, express-session, mysql, passport, sequelize

--FILES EXPLAINED--

CONFIG

MIDDLEWARE

isAuthenticated.js 
it restricts the routes that user is not permitted to visit if not logged in. But if the user is logged in, it continues with request.

config.json: connection configuration to connect to the server.

passport.js: contains javascript logic which tells passport about the login requirements (user name and password).

MODELS

index.js: connects to the database and imports the users data( log in).

user.js: requires "bcrypt" for password hashing. This makes our database secure even if compromised. Here we have JS that defines what is stored on our database.

ROUTES

api-routes.js: contains routes for log in and out and getting specific data to be displayed on the browser.

html-routes.js:routesfor checking whether user is logged in, has already an account etc and locate them to the respected page };

package.json: contains all package info, the used dependencies or modules, version info etc etc.

server.js: Starting point for this app , requires packages, sets up PORT, creates middleware and express, creates routes and syncs database with the input data, logs message in terminal on status of the connection to the server.


## Authors

* **Naresh Raj Poudel** - [Git Hub Profile](https://github.com/citenaresh): https://github.com/citenaresh

## Acknowledgments

* Great gratitude to Luca ([https://github.com/duvet86](https://github.com/duvet86)), Sam ([https://github.com/sam-ngu](https://github.com/sam-ngu)) and Renata from the UWA Bootcamp for their enormous help.

## Questions

-   For any questions related to this applicaiton, please feel free to contact me at: citenareshn@gmail.com.

-   Please use this link to access my Github Profile: [Git Hub Profile](https://github.com/citenaresh): https://github.com/citenaresh
