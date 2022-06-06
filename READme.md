# Project 0
## Revature
### By Luis Marquez

Project 0 demonstrates a way to create a back-end platform using Java, Spring Boot and JPA.

The project comprises two modules, and this is the demonstration of the first module, showing the server side of the full-stack website.

It’s important to use port 8083 and mail deliverer as a test platform.

This is the UML of the database schema for this project:
![Databse UML schema](http://gfusoa.com/images/databaseSchema.PNG)

To use the backend, it is important to follow the procedure:

Registration of a user: `http://34.207.111.83:8083/users`

Un example of input on body(raw/JSON):

`{
“username”: “admin1”,
“password”: “pass”,
“email”: “admi21@gmail.com”,
“firstname”: “Admin1”,
“lastname”: “Admin1_Lastname”,
“role”: “ADMIN”
}`

Login of user: `http://34.207.111.83:8083/login`

Un example of input on body(raw/JSON):

`{
“username”: “admin1”,
“password”: “pass”
}`

Update user: `http://34.207.111.83:8083/users/2`

Un example of input on body(raw/JSON):

`{
“username”: “admin2”,
“password”: “pass”,
“email”: “admin22@gmail.com”,
“firstname”: “Admin2”,
“lastname”: “Admin2_Lastname”
}`

Get a list of users: 
`http://34.207.111.83:8083/users`

Get user by Id: `http://34.207.111.83:8083/users/1`

Delete user: `http://34.207.111.83:8083/users/2`

Registration of product: `http://34.207.111.83:8083/products`

Un example of input on body(raw/JSON):

`{
“product_name”: “Apple”,
“product_price”: 1.35,
“product_quantity”: 20
}`

List of products: `http://34.207.111.83:8083/products/`

List of products by Id: `http://34.207.111.83:8083/products/1`

Update product: `http://34.207.111.83:8083/products/1`

Un example of input on body(raw/JSON):

`{
“product_name”: “Orange”,
“product_price”: 1.6,
“product_quantity”: 100
}`

Delete of product: `http://34.207.111.83:8083/products/2`

Create order: `http://34.207.111.83:8083/orders`

Un example of input on body(raw/JSON):

`{
“user_id”: 2
}`

Order List: `http://34.207.111.83:8083/orders`

Add the product to order: `http://34.207.111.83:8083/orders/1/products/1`

Logout: `http://34.207.111.83:8083/logout`