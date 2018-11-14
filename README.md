![cf](http://i.imgur.com/7v5ASc8.png) Access Control (ACL)
==========================================================

## Submission Instructions
  * Follow the instructions in the "Lab Instructions" documentation in the reference folder of the class repository

### Overview
Implement Role Based Authentication

#### Feature Tasks -- Server
* Protect your API Routes with the proper permissions based on user capability
  * `app.get('/schema')` should require the `superuser` capability
  * `app.get(...)` should require the `read` capability
  * `app.post(...)` should require the `create` capability
  * `app.put(...)` should require the `update` capability
  * `app.patch(...)` should require the `update` capability
  * `app.delete(...)` should require the `delete` capability

* You will need to create, allocate, and identify user permissions in the model
* You will need to restrict based on the given permission via middleware

#### Feature Tasks -- RESTy
* Add support for basic and bearer authentication
* You will need to add fields for those on the form
* You will need to pass those through, when present, in the superagent calls.

#### Test
* Add tests to the api routes, asserting restricted access to the routes as shown.

#### Documentation

##### Getting Started
In order to use this program, a user would need to fork this repo and clone it down from their machine. They can use [this](https://github.com/ashley-breunich/lab-15) link to access the repository. They would need to install the dependencies (npm install) before beginning. 

##### .env Variables
```
PORT=3000
STORAGE=mongo
MONGODB_URI=mongodb://localhost:27017/store
```