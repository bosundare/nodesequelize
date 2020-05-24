# nodesequelize
Using Node JS with MySQL - A Job Search tool
### Installation
```sh
$ git clone https://github.com/bosundare/nodesequelize.git
```
Install the dependencies

```sh
$ cd nodesequelize
```
```sh
$ npm install
```
Make a database.js file in the /config directory to store your variables. 

```sh
$ touch config/database.js
```
```
// Paste the following mysql configs into config/database.js file and save.
const Sequelize = require('sequelize');

module.exports =  new Sequelize('#_Database_name#', '#_Database_user#', '#Database_password#', {
  host: 'localhost',
  dialect: 'mysql',
  
  pool: {
    max: 5,
    min: 0,
    acquire: 30000,
    idle: 10000
  },
});
 ```

Run app

```sh
$ npm start
```

```sh
Visit localhost:5000 to view the app.
```
