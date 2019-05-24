** POST requests
1. Add a user and receive token
https://rent-mytools.herokuapp.com/api/auth/register

Upon receiving a token it's recommended to save it in local storage.

Example
All fields required except thumbnail_url
{
first_name:"Test",
last_name:"Test,
username:"Test",
password:"Test234",
thumbnail_url:"http://whatever.com"
}

1. Login an existing user and receive token
https://rent-mytools.herokuapp.com/api/auth/login

Upon receiving a token it's recommended to save it in local storage.

Example
all fields required
{
    username:"Test",
    password:"Test"
}

1. Add a tool
https://rent-mytools.herokuapp.com/api/tools

Example
user_id, tool, and price are required fields
{
    userId:"1",
    tool:"hammer",
    price:"10.50",
    description:"Ya hit stuff, it gets nailed",
    imageUrl:"http://imgurl.com",
    isRented:"false"
}

1. Add a tool to rented list
https://rent-mytools.herokuapp.com/api/toolrental

Example
All fields required (renterId === userId)

{
    renterId:"1",
    toolId:"1"
}

**Get requests

1. Get All Tools
http://https://rent-mytools.herokuapp.com/api/tools

1. Get tool by ID
(:id === toolId)
http://https://rent-mytools.herokuapp.com/api/tools/:id

1. Get all users
http://https://rent-mytools.herokuapp.com/api/users


1. Get user by ID
http://https://rent-mytools.herokuapp.com/api/users/:id

1. Get all rented tools
http://https://rent-mytools.herokuapp.com/api/toolrental



**Delete requests

1. Delete a user
http://https://rent-mytools.herokuapp.com/api/users/:id

1. Delete a tool
http://https://rent-mytools.herokuapp.com/api/tools/:id

1. Delete a rental from rented list
http://https://rent-mytools.herokuapp.com/api/toolrental/:id


**Update Requests

1. Update a user
https://rent-mytools.herokuapp.com/api/users/:id
Example
All fields required
{
first_name:"Test",
last_name:"Test,
username:"Test",
password:"Test234",
thumbnail_url:"http://test.com"
}

1. Update a tool
https://rent-mytools.herokuapp.com/api/tools/:id

Example
user_id, tool, and price are required fields

{
    userId:1,
    tool:"hammer",
    price:"10.50",
    description:"Ya hit stuff, it gets nailed",
    imageUrl:"http://imgurl.com",
    isRented:false

   
}






