# Project Title
JavaScript MEAN stack project template based on Angular (+7)


## Description 
Template for JavaScript MEAN stack project contains all needed setup to download and start implementing your project quickly based on Angular (+7) and using Grunt as Task runner. 

### Contents

```
Project
│   README.md       --> Contains project description you are reading now.
│   Gruntfile .js   --> Contains Grunt "Tasks Runner"  configurations with some plugins as examples "develop, watch and jshint".
│   package.json    --> Contains all npm packages needed for this project.
|   bower.json      --> Contains all bower packages needed for this project. 
|   
└─── server --> Folder contains all Back-End codes.
│   │   
│   └─── express --> Folder contains "Express" configurations and "routes" files for app APIs.
|        |
|        |_____ configs.js  --> File contains all needed "Express" configurations like its middlewares and so on.
|        |
|        |_____ routes      --> Folder contains all routes for this app APIs.
|           
│       
│   │   
│   └─── models  -->  Folder contains all Mongoose models and its plugins.
│          
│       
│   │   
│   └─── controllers --> Folder contains all modules which handle different APIs.
│          
│       
│   │   
│   └─── utilis   --> General utilis which needed by different app's modules.
│          
│       
│   │   
│   └─── app.js   --> App startup script to set the needed configurations, load Mongoose models, start listening and so on. 
|
│          
│       
│   
└─── client  --> Folder contains all "Front-End" codes. This folder generated automatically using 
     ```
    ng new client
    ```
           
```


### Prerequisites
* Know about JavaScript MEAN stack.
* Have npm & bower installed on your machine.
* Assure you have MongoDB server running on your machine with default settings.

### Building Steps:

* Download project source code.

* Build the needed NPM modules as following
    ```
    npm install
    ```

* Build the needed bower modules as following
    ```
    bower install
    ```

* Create '.env' file in the project root directory to contains your app's environment variable
```
    DATABASESERVER_URL='mongodb://localhost:27017/mean_template'
    PORT=8080
```

* Run this app as following.
    #### Terminal 1:

    ```
    npm run angular
    ```
    This command will build Angular codes and output to 'server/public' folder, and watch for changes and rebuild automatically.


    #### Terminal 2:
    ```
    grunt
    ```
    runs default Grunt tasks for you (running Node.js app, watch for any server changes). 
    
    #### Side note:
    And also there is a separate task can use to lint your JavaScript codes "jshint" as following.
    ```
    grunt jshint
    ```

* From browser just type 
    ```
    http://localhost:8080/
    ```






 