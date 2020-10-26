# tourbar
Our first MERN Stack project 

- Here in our Full stack application we have: **Frontend** and **Backend**
  Frontend holds react app with some components
  and Backend holds the core js file.

### Basic development setup
  
  __// navigate to frontend/proj_name__
  > npm install 

  __// navigate to backend/proj_name (in our case tourbar)__
  > npm intall 

  __// to start the server__
  > npm start


- Let's understand first the basic idea How this app will work


- **Sketching the frontend (wireframe)** 
 

#### M - mongoDB (database solution)
#### E - express (a nodejs framework)
#### R - react (browser-side javascript library)
#### N - nodejs (server-side javascript runtime)

### So, here in this project we will be building a fullstack MERN application where our frontend will be in react and backend will be in Node.

 :octocat: **What is React ?**

 > A client-side (browser) library which allows you to build highly reactive user interfaces.
 > Responsible for controlling what users see on screen and how the things change there.

  ![This is what React does](https://github.com/madhav06/projectImages/blob/master/react.png)

### A brief note on Node now...

 :octocat: **What is Node ?**

 > It's a javascript runtime often used to create server-side applications.
 > Node JS is used to execute javascript code outside the browser.

  ![This is what Node does](https://github.com/madhav06/projectImages/blob/master/node.png)


### A brief note on Express...
 :octocat: **What is Express ?**

 > A Node framework which simplifies writing server-side code and logic.
 > Express is for Node what Laravel for PHP.

  ![This is what Express does](https://github.com/madhav06/projectImages/blob/master/express.png)

### A brief note on mongoDB...

 :octocat: **What is mongoDB ?**

 > A NoSQL Database which stores "Documents" in collections instead of "Records" in tables as in SQL.
 > mongoDB often gives amazing performance because it is way more flexible.
 > We can use other DBs also but then it would not be MERN application.
 > Considered as a powerful database which can be easily integrated into a Node/Express environment.

  ![This is what monogDB does](https://github.com/madhav06/projectImages/blob/master/mongo.png)



- Our application UI for web version looks something like this:

![Web Version](https://github.com/madhav06/projectImages/blob/master/Screenshot%202020-10-19%20at%209.27.09%20AM.png)


- And the mobile app version looks something like this:

![Mobile App Versio](https://github.com/madhav06/projectImages/blob/master/Screenshot%202020-10-19%20at%209.27.34%20AM.png)

__We are making an application called **tourbar** where users can share places they have visited__

#### Adding validators for **Add Place Form** 

```Javascript
const VALIDATOR_TYPE_REQUIRE = 'REQUIRE';
const VALIDATOR_TYPE_MINLENGTH = 'MINLENGTH';
const VALIDATOR_TYPE_MAXLENGTH = 'MAXLENGTH';
const VALIDATOR_TYPE_MIN = 'MIN';
const VALIDATOR_TYPE_MAX = 'MAX';
const VALIDATOR_TYPE_EMAIL = 'EMAIL';
const VALIDATOR_TYPE_FILE = 'FILE';


for (const validator of validators) {
    if (validator.type === VALIDATOR_TYPE_REQUIRE) {
      isValid = isValid && value.trim().length > 0;
    }
    if (validator.type === VALIDATOR_TYPE_MINLENGTH) {
      isValid = isValid && value.trim().length >= validator.val;
    }
    if (validator.type === VALIDATOR_TYPE_MAXLENGTH) {
      isValid = isValid && value.trim().length <= validator.val;
    }
    if (validator.type === VALIDATOR_TYPE_MIN) {
      isValid = isValid && +value >= validator.val;
    }
    if (validator.type === VALIDATOR_TYPE_MAX) {
      isValid = isValid && +value <= validator.val;
    }
    if (validator.type === VALIDATOR_TYPE_EMAIL) {
      isValid = isValid && /^\S+@\S+\.\S+$/.test(value);
    }
  }
  return isValid;
```


#### Finishing Add Place then:

![Add Place](https://github.com/madhav06/projectImages/blob/master/addform.png)

- here User can click on edit to update the places they have visited.

![Edit Places](https://github.com/madhav06/projectImages/blob/master/editPlace1.png)

- Once clicked, they can update the details they want to change:

![Edit Places](https://github.com/madhav06/projectImages/blob/master/editPlace2.png)

- These will be the **API ENDPOINTS** in our application for backend.

![API Endpoints](https://github.com/madhav06/projectImages/blob/master/api_endpoints.png)

- Once frontend is done, for backends we need to install now required **Dependencies and Packages**

```Javascript
npm install --save express body-parser

npm install --save-dev nodemon

```

