# MailBag
A third party IMAP web email system for Gmail implemented with Node.js, React, Webpack and TypeScript.
## Table of contents
* [Overview](#Overview)
* [Techniques](#techniques)
* [Setup](#setup)
## Overview
This project is a third-party IMAP e-mail system for Gmail, which is aimed at helping users customize and design their mailboxes based on their needs. The system currently supports receiving, editing e-mails, and configuring contacts. 

The project has a server-side and a client-side. The server is developed with Node.js, TypeScript, NoSQL, and Express. The client part is created using Webpack, React, and TypeScript. The project utilizes RESTful APIs to simplify the development and testing process.

More functions like data analysis, email recommendations based on machine learning will be added in the future versions. 
	
## Techniques
Project is created with:
* Node version: 12.16.2
* TypeScript
* React
* Express
* Webpack
* Babel
	
## Setup
To run this project, clone or download the project into local repository:

First, configure server-side:

```
$ cd ../server
$ npm install
$ npx tsc
$ npm run dev
```

Now the server will run on port 80. 

To configure your own email, you can add your name and password into serverInfo.json under server folder and open IMAP support on your Gmail.

Then , start up the client-side.

```
$ cd ../client
$ npm install
$ npx webpack
```

Then open the index.html in generated dist-folder under client. Now the program is running. 

To make the server run on a different port. Please configure it in main.ts file in server/src folder. Also configure the port for client by changing config.ts in client/src/code. 

