# EmergencyDashboard - Real-Time Dashboard

## Purpose
This adesktop pplication is created to allow the user/ volunteers to view data in real time.

## Technologies involved
This real-time dashboard is generated with Angular 9 [https://github.com/angular/angular-cli] and Electron [https://www.electronjs.org/]
It also interacts through REST with the backend created with Cubejs Framework. 
The database used is MongoDB with the corrisponding BI Connector.

## How to setup the dev enviroment
### Setting up MongoDB and BI Connector
1. Go to the following link and install MongoDB on your computer. [https://www.mongodb.com/download-center/community]
2. Go to the following link and install the BI Connector on your computer. [https://www.mongodb.com/download-center/bi-connector]
3. After the installation has been successfully completed, please start the MongoDB and the BI Connector from the respectibe **/bin** directory  with the following command from your terminal 
```
mongod
```
```
mongosqld
```
4. If everything works correctly you should see a success log message in your shell for the **mongosqld** process:
```
... [initandlisten] waiting for connections at 127.0.0.1:3307
```
### Setting uo the Cube.js Application (Backend)
1. We're going to use the **Cube.js CLI** in order to create the backend application. If you don't have _Node.js_ already installed on your computer, please follow the steps of this guide [ https://nodejs.org/en/download/package-manager/ link]
To install the CLI run this commans on yout terminal
```
npm install -g cubejs-cli
```
2. Now we're going to open the application with an IDE and change the **.env** file with the credential of your new created dtaabase.
Attention : If you created the MongoDB as described above the right credential are still in the document.
3. To start the backend that then listen to **http://localhost:4000** pleade run from the application folder this command
```
npm run dev
```
### Start the frontend dashboard
1. In order to **build** this applicaiton you need to have installed _Node.js_ and _Electron_ on your machine.
In order to install bglobally _Electron_ run the following command on your terminal
```
npm install electron -g
```
otherwise only in your app run from within the application
```
npm install electron --save-dev
```
2. To start the application in _Electron_ run from the root of the app
```
npm run start:electron
```
## Important:
##  Important: to find the project, due to GitHub size limit, see
### https://ibm.ent.box.com/folder/111683426682

## Author:
* Giulia Gallico - [codeAllien](https://github.com/codeAllien)
