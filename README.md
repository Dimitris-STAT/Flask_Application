# Report
  
To activate and use this web service, follow these steps:

1.Install Docker on your computer. Docker enables you to create and activate individual images and containers. The necessary creation commands can be found in the docker_compose and Dockerfile files.

2.Build the Docker images and containers by running the command "docker-compose up --build." This command will create the docker-compose_flask-service and mongo images along with their respective containers on your computer.

3.Once the installation is complete, the web service is automatically installed and ready to be used. The endpoints within the service_code.py file can now be executed.

4.Make sure your system has applications or programs that support HTTP methods like 'GET,' 'POST,' 'PUT,' 'PATCH,' and others. These methods are essential for implementing data endpoints. Web browsers typically only support the GET method.

5.After completing the above steps, you can choose and execute different endpoints according to your preference.

  
   
In the second stage, we analyze created endpoints and their implementation. Administrators can create other administrators through "createAdmin" endpoint. 

1) "AdminLogin" is used to access additional endpoints. Authorized endpoints are:

2) "createProduct": Create a new product using JSON data.

3) "deleteProduct": Delete a product by specifying its "_id".

4) Update product fields: Modify four specific fields of a product by providing its ID.
   
 
User-related Endpoints:
1) "createUser": Creates a user with a "category" field indicating they are a simple user.
2) "login": User login endpoint that generates a UUID code for authorization.
User Operations:
3) "getProduct": Searches for a product by name, _id, or category. Displays results alphabetically by name or by category.
4) "addToCart": Adds products to a temporary shopping cart. Calculates the total price based on the requested quantity.
5) "viewCart": Displays the shopping cart with product information and the final receipt.
6) "deleteFromCart": Removes a product from the cart based on its id. Updates the remaining products and the new total price.
7) "buyProducts": Displays the products and final cost after providing payment information. Clears the cart.
Other Endpoints:
1) "OrderHistory": Updates the user's data with the receipt from the last purchase using their email.
2) "deleteUser": Deletes the user's account and associated data from the system's database.

