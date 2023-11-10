# JWT
## npm install

## Set of requests

 1. Login to get token

		POST http://localhost:4000/login

		Content-Type: application/json
		{

		"username":"Someone"

		}

2. Use access token to get posts

		GET http://localhost:3000/posts
		Authorization:  Bearer ***accesstoken***

3. Get token after login using refresh token to get access token

		POST http://localhost:4000/token
		Content-Type: application/json
		{
		"token":"***refresh token***"
		}
4. You can view data again with access token to get like step 2
5.  Logout using access token to delete the refresh token.

	    DELETE http://localhost:4000/logout
		Content-Type: application/json
		{
		"token":"***refresh token***"
		}

