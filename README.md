# Using the project
The `server` folder has the server code
- Clone the repo and open a terminal. Go to the server folder.
```
cd server
```
- Install dependencies
```
npm install
```
- Start the server
```
npm start
```
The server serves `contacts` resource providing standard REST API to work with this resource. To fetch all contacts, for example, make a `GET` request to
```
http://localhost:4000/contacts
```

## APIs
| **Operation**                         | **HTTP Request**                                                                                                      |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| Fetch all contacts                    | `GET http://localhost:4000/contacts`                                                                                  |
| Fetch contact by id (id = 3)          | `GET http://localhost:4000/contacts/3`                                                                                |
| Add new contact                       | `POST http://localhost:4000/contacts` <br> Pass `{ "name": "Mark Smith", "number": "1234567890" }` as JSON in the body |
| Update contact with given id (id = 3) | `POST http://localhost:4000/contacts/3` <br> Pass `{ "name": "Mark Smith II", "number": "1234567891" }` as JSON body   |
| Delete contact with given id (id = 3) | `DELETE http://localhost:4000/contacts/3`                                                                             |