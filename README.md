#Backend verification (user login)

learn to use [JWT](https://jwt.io/introduction) to authorize user login (auth route) or signup(users route). We can add 'x-auth-token' in the header with the user token to get authrized user info

in POST route, use express-validator middleware to check request format and handle error.
If everything pass, use try catch to find user by email, and bcryptjs to hash password (and compare if hashed password match the DB)
