# Technical Skills API


## [Click here to see the report](https://glitchmemahmud.netlify.app/)

## Endpoints

### Fetch All skills

GET `/api/technicalskills`

Returns the Status and data of the API.

### Status

GET `/status`

Returns the status of the API.

### Single User Skills in details###

GET `api/technicalskills/169`

Returns Details of that id.
###Filter id List based in skills###

GET `/api/technicalskills?language=java`

Returns a list of Users based on types.

### Create a User with skills

POST `/api/technicalskills`

Allows you to create new user details. doesn't Requires authentication.

The request body needs to be in JSON format and include the following properties:

{
"language": ["1","2"],
"yearexp": "exp",
"lastused": "date",
"st_id": "id"
}

The response body returns a message
`

- "status": "true",
- "msg": "Add data success"
  `

### Get newly created user

GET `/api/technicalskills/{{id}}`

Allows you to view.

### Update a User with id

PUT `/api/technicalskills`

Allows you to update user details. doesn't Requires authentication.

The request body needs to be in JSON format and include the following properties:

{
"language": ["1","2"],
"yearexp": "exp",
"lastused": "date",
"st_id": "id"
}

The response body returns a message
`

- "status": "true",
- "msg": "update data success"
  `

### Delete a User

Delete `/api/technicalskills/{{id}}`

Allows you to delete users. doesn't Requires authentication.

The response body returns a message
`

- "status": "false",
- "msg": "not found"
  `
