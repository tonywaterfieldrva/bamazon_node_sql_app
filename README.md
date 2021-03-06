# bamazon_node_sql_app

The objective of the activity is to create an "Amazon"-like store front CLI application using node and mysql.  The app will use 2 tables in mysql database bamazon.

The app will perform the following specifications:

    mySQL database table `products`.  (An "orders" table was additionaly created to record each sale)

    Provide a list of products for sale with inventory on hand information

    Inquirer command line prompts will accept order input of item number and quantity
        a function will take the response and access the record in products table
        
        If order quantity can be fullfilled, a database insert into the orders table will record the order data.  The new order record will then be retrieved and sent to the terminal screen as a recordset or console log message.  The qoh available will be updated in the products table.

        If inventory on hand is below the order quantity the order will be rejected and a console.log message will indicate order was rejected, provide a maximum amount available and relist the product list.  The inquirer prompt will request a new order request.

 Requried npm node packages:
    
    * inquirer
    * mysql
    * moment

    package.json contains initialization parameters 


Inital run of bamazonCustomer.js and details of first item ordered

![imagecapture](images/successful_order1.PNG)

Bottom half of above screenshot.  Item 5001 has inventory deducted by 50 from 199 to 149.

![imagecapture](images/successful_order2.PNG)

Demostrates a rejected order where ordered quantity exceeded quantity on hand.  
Message indicates order rejected and provides the maximum available quantity that can be ordered.

![imagecapture](images/rejected_order.PNG)
<<<<<<< HEAD

CHALLENGE #2  bamazonManagers.js

A Managers javascript that allow Managers the following options

View Product List
View Low Inventory Level
Update Inventory Quantity
Add New Sale Product to Inventory

Initial run of bamazonManagers.js

![imagecapture](images/manager1_init.PNG)

View Product List results

![imagecapture](images/manager2_viewlist.PNG)

View Low Inventory Level and Update Inventory Quantity

![imagecapture](images/manager2_viewlowinv.PNG)

Add New Product to Inventory

![imagecapture](images/manager3_addproduct.PNG)
