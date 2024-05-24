# backend-final-project-IBM
#Developing Back-End Apps with Node.js and Express
#From IBM on Coursera

In this final project, we will build a server-side online book review application and integrate it with a secure REST API server which will use authentication at session level using JWT. You will then test your application using Promises callbacks or Async-Await functions.


#Try it yourself
npm install
npm start
Testable locally via CLI
Get the book list available in the shop
curl -i localhost:5000/
Get the books based on ISBN
curl -i localhost:5000/isbn/1
Get all books by the author
curl -i localhost:5000/author/Unknown
Get all books based on title
curl -i localhost:5000/title/Fairy%20tales
Get a book review
curl -i localhost:5000/review/6
Register new user
curl --header "Content-Type: application/json" \
    --request POST \
    --data '{ "username":"john", "password":"fake" }' \
    localhost:5000/register
Login as a registered user
curl --header "Content-Type: application/json" \
    --request POST \
    --data '{ "username":"john", "password":"fake" }' \
    localhost:5000/customer/login
Testable via Postman
For this part it is necessary that the app is accessible from the Internet via the free Postman account that you have created, since curl cannot access req.session from CLI

