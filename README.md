# API development using the 3 main open-source Swagger tools (Editor, Codegen and UI)
### Purposes: 
1. To utilize Swagger Editor to design an API contract using the OpenAPI specification and YAML
2. To utilize Swagger UI to generate API documentation
3. To use an API contract to create a working RESTful API

### Instruction to start off: npm start 

### 4 main paths created, and the commands are as follows:

1. Getting All Orders
- To test the /orders path. simply navigate to http://localhost:3000/orders in a browser. The data should appear on the screen.

2. Creating a New Order
- To test our /neworder path, use the curl command in a terminal. Open a terminal window (or command prompt) and navigate to the project directory. From here, run the following command:curl --header "Content-Type: application/json" -d "@new_order.json" http://localhost:3000/neworder

3. Updating an Existing Order

- Enter this curl command from the terminal: curl -X PUT -d complete http://localhost:3000/update/001
This command makes a PUT request which modifies the state of the order with an id of 001. It will change it to the text complete. Use the GET request again by refreshing the server on the browser to see the changes in the first order.

4. Deleting an Existing Order

- Enter curl command to make a DELETE request to our /delete/{id} endpoint:curl -X DELETE http://localhost:3000/delete/002
Using the GET request by refreshing the server on the browser should show that the order with an id of 002 has been removed from the orders list.

#### Sources:

- Full files available on: https://drive.google.com/drive/folders/17p544F7uN3IGg4joJgTZeJl9_goE4haF?usp=sharing
- Online Swagger Editor: https://editor.swagger.io
