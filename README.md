Get all depencdecies
`npm install`

To run the tests
`npm test`

Test api in Postman:
Test register user:
url: http://localhost:3900/api/users
pass user details in the body as json:
{
"name": "John",
"email": "john@gmail.com",
"password": "password1234"
}

    To test login:
    url: http://localhost:3900/api/auth
    pass user email(username) and password in the body as json:
    {
        "email": "john@gmail.com",
        "password": "password1234"
    }

Note:
MongoDB used to store user details.
Used Json Web Token to secure route.
Done only a unit test for checking the web token.
Could have done integration test for api routes by using test framework 'supertest' with test database.
