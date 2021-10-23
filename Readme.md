

Nodejs Backend:

Github link:https://github.com/mrsuber/recipe-web-app,


--> user Management:
            can create user:
                POST request:  http://localhost:5000/api/auth/register,  
                    body `{
	"username":"mohamad",
	"email":"msb2@gmail.com",
	"password":"msb1@@@@"
}`
--> user Management:
            can update user:
                Put request:  http://localhost:5000/api/private/updateuser/id,  
                    body `{
	"password":"msb2@@@@"
}`

--> user Management:
            can delet user:
                DELETE request:  http://localhost:5000/api/private/deleteuser/id,  

--> user Management:
            can login user:
                POST request:  http://localhost:5000/api/auth/login,  
                   body `{
        "email":"msb@gmail.com",
	"password":"msb2@@@@"

}`

--> user Management:
            can get all user:
                GET request:  http://localhost:5000/api/private/getallusers,  
--> user Management:
            can A  user:
                GET request:  http://localhost:5000/api/private/finduser/id,  
--> user Management:
            can get user statistics:
                GET request:  http://localhost:5000/api/private/stats,  
--> user Management:
            reset user password:
                first: POST request:  http://localhost:5000/api/auth/forgotpassword,  
                body`{
	"email":"msb@gmail.com"
}`
            second, collet token form cosole post
                PUT request http://localhost:5000/api/auth/resetpassword/token
                body:`{
	"password":"msb2@@@@"
}`

Note, headers should containg Authentication Bearer token to get users,delet users and all recipe managements


--> recipe Management:
            can get all recipe:
                GET request:  http://localhost:5000/api/private/getallrecipe,  
--> recipe Management:
            can get one recipe:
                GET request:  http://localhost:5000/api/private/getarecipe/id,  

--> recipe Management:
            can get update recipe:
                PUT request:  http://localhost:5000/api/private/updaterecipe/id,  

--> recipe Management:
            can get delete recipe:
                DELETE request:  http://localhost:5000/api/private/deleterecipe/id,  
--> recipe Management:
            can get create recipe:
                POST request:  http://localhost:5000/api/private/createnewrecipe/id,  
