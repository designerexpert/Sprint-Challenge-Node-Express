# Prepare Boilerplate
* Create a file for the server: `touch server.js`
* `npm init -Y` | `yarn init -y`
* `npm install --save express, cors, knex, sqlite3` | `yarn add express, cors, knex, sqlite3`
* `npm install --save-dev nodemon` | `yarn add --dev nodemon`
* Edit the package.json file to include a script to start the server: `"nodemon server.js"`

# Projects Endpoints
|Type|Address|Example Request Body|
|:-:|:-|:-|
|GET|/api/projects||
|GET|/api/projects/:id||
|POST|/api/projects|{ name: 'str', description: 'str', completed: false }|
|DELETE|/api/projects/:id||
|UPDATE|/api/projects/:id|{ name: 'str', description: 'str', completed: false }|

# Actions Endpoints
|Type|Address|Example Request Body|
|:-:|:-|:-|
|GET|/api/actions||
|GET|/api/actions/:id||
|POST|/api/actions|{ project_id: 1, description: 'str', notes: 'str', completed: false }|
|DELETE|/api/actions/:id||
|UPDATE|/api/actions/:id|{ project_id: 1, description: 'str', notes: 'str', completed: false }|