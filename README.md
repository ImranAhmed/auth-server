# Authentication Server

Store user name and password (salt + hash) in mongodb.

1.Install mongodb: https://docs.mongodb.com/manual/installation/

2.Install a query tool for mongodb eg. https://robomongo.org/ (note latest version will be a paid version, older versions are free)

3.Create a local file in root for storing a secret key for encryption (config.js) in following format. **Do not checkin this file with source code**

module.exports = { 
    secret: 'add a secret here'
}

4.npm install

5.npm run dev

Test in postman

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

further info: https://www.udemy.com/react-redux-tutorial/
