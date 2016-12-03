# Authentication Server

Store user name and password (salt + hash) in mongodb.

- Install mongodb: https://docs.mongodb.com/manual/installation/

- Install a query tool for mongodb eg. https://robomongo.org/ (note latest version will be a paid version, older versions are free)

- Create a local file in root for storing a secret key for encryption (config.js) in following format. 
**Do not checkin this file with source code**

module.exports = { 
    secret: 'add a secret here'
}

- npm install

- npm run dev

- Test in postman

Signin endpoint http://localhost:3090/signup

eg. body

{
	"email": "01@example.com",
	"password":"test"
}

Signin endpoint http://localhost:3090/signin

eg. body

{
	"email": "01@example.com",
	"password":"test"
}

- further info: https://www.udemy.com/react-redux-tutorial/
