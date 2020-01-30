# [sequelize-burger](https://burgersequelizedsanjib.herokuapp.com/burgers)
## Overview
In this assignment, you're going to Sequelize the `Burger` app you made last week. We've split this exercise into three different tiers, all with different tasks and expectations. Finish whichever tier will provide you with the most reasonable challenge.
## Dependencies
* body-parser
* express
* express-handlebars
* method-override
* mysql2
* sequelize
## Installation
### Install Locally
```
git clone https://github.com/skbiswas1975/Burger_Sequelized.git
cd Burger_Sequelized
npm install
```
### config.json File
1. Navigate to the `config.json` file in the `config` directory and locate the `development` object:
```
  "development": {
    "username": "[root]",
    "password": "[newpassword]",
    "database": "burgers_db",
    "host": "[localhost]",
    "dialect": "mysql",
    "operatorsAliases": false
  }
```
2. Edit any of the values in the brackets above to coordinate with your MySQL Database.
### Command
`node server.js`
## Requirements
### Tier 1: Sequelized
- [x] Remove all references to your vanilla MySQL queries and replace them with Sequelize queries.
  - [x] Replace your MySQL `Burger` model with a Sequelized equivalent.
    - [x] Edit the model and initial migration file to make the burger's devoured field carry a default value of false.
    - [x] Sync the models.
- [x] Edit your new `config.json` file to include your database configurations.
  - [x] Place your Local Database details in the `development` property of your json file.
  - [x] Place your JawsDB details in the `production` property of your json file.
- [x] Remove your old ORM file, as well as any references to it in `burgers_controller.js`. 
  - [x] Replace those references with Sequelize's ORM methods.
### Tier 2: Customer Associations
- [x] Add in a Customer association to the project. 
  - [x] Create at least one new `Customer` model and connect it with your `Burger` model.
- [x] Edit the handlebars files and CSS stylesheets to implement some sort of additional feature to the site. 
## Bonus
- [x] Add validations to your models where:
  - [x] A burger's name cannot be null
  - [x] A burger's devoured status is false by default
  - [x] A Customer's name cannot be null
- [x] Order the Burgers you send back to the user in alphabetical order using the Sequelize "order" option.
