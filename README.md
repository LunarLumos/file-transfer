# file-transfer
Apologies for the confusion earlier. Let's correct the approach and make sure we follow the proper academic structure for **Flowchart** and **Pseudocode**.

Here is a detailed and **correct version** for the **Admin Panel** process, including **Authentication** and menu-based navigation:

---

### **Flowchart for Admin Panel with Authentication (Detailed)**

**Step-by-step explanation** for the flowchart:

1. **Start**:
   - Begin the program.

2. **Login Prompt**:
   - Prompt the admin for a **Username** and **Password**.

3. **Authentication Check**:
   - If the **username** is `"admin"` and the **password** is `"password123"`, grant access to the admin menu.
   - If credentials are incorrect, show an **error message** and terminate the program.

4. **Admin Menu**:
   - Once authenticated, display a list of options in the **Admin Menu**:
     - **Option 1**: View All Dishes
     - **Option 2**: Add New Dish
     - **Option 3**: Update Dish
     - **Option 4**: Delete Dish
     - **Option 5**: Search Dishes
     - **Option 6**: Generate Sales Report
     - **Option 7**: Exit Program

5. **Process Admin’s Choice**:
   - The program will process the admin’s choice, and depending on the option selected, it will:
     - **Option 1**: Display all available dishes.
     - **Option 2**: Add a new dish to the menu.
     - **Option 3**: Update an existing dish.
     - **Option 4**: Delete a dish.
     - **Option 5**: Search for a dish.
     - **Option 6**: Generate a sales report.
     - **Option 7**: Exit the admin panel.

6. **Exit/Repeat**:
   - If the user chooses **Exit**, the program will end.
   - Otherwise, the program loops back to the **Admin Menu** after completing any selected task.

---

### **Flowchart Diagram (Detailed)**

Below is the **corrected flowchart**, structured for academic standards:

```plaintext
          +---------------------+
          |     Start           |
          +---------------------+
                    |
                    v
        +-----------------------+
        |  Prompt for Username  |
        |  and Password         |
        +-----------------------+
                    |
                    v
        +-----------------------+
        |  Check Credentials     |
        |  (username == admin    |
        |  and password == admin)|
        +-----------------------+
                    |
      +-------------+-------------+
      |                           |
      v                           v
 +---------------+          +--------------------+
 |  Invalid      |          |   Valid Credentials|
 |  Credentials |          |   Proceed to Admin |
 |  Display Error          |   Menu              |
 +---------------+          +--------------------+
            |                            |
            v                            v
       +---------------------+      +----------------------+
       |   Exit Program      |      |   Display Admin Menu |
       +---------------------+      +----------------------+
                                    |
                                    v
                        +--------------------------+
                        |  Wait for Admin Choice   |
                        +--------------------------+
                                    |
                                    v
                      +------------------------------+
                      | Perform Action Based on Choice|
                      +------------------------------+
                                |
    +---------------------+-----+-----+-----+-----+-----+
    |                     |     |     |     |     |     |
    v                     v     v     v     v     v     v
+------------+    +------------+  +-----------+  +-----------+  +-----------+  +-----------+
| View Dishes|    | Add Dish   |  | Update Dish|  | Delete Dish|  | Search Dishes|  | Sales Report|
| (Display All)   |    | Add Dish to  |  | Update Dish |  | Remove Dish |  | Search for a |  | Display Sales|
+------------+    | Menu       |  +-----------+  | Menu       |  | Item        |  | Report      |
                  +------------+               +-----------+               +-----------+
                                  |
                            +------------------+
                            | Exit Admin Panel |
                            +------------------+
                                  |
                              +-----------+
                              |    End    |
                              +-----------+
```

---

### **Pseudocode for Admin Panel with Authentication**

**Pseudocode** explains the sequence of operations in plain text:

```plaintext
START

    // Step 1: Admin Login
    DISPLAY "Enter Username:"
    READ username
    DISPLAY "Enter Password:"
    READ password

    // Step 2: Authentication Check
    IF username == "admin" AND password == "password123" THEN
        DISPLAY "Login Successful"
        CALL admin_menu()   // Proceed to Admin Menu
    ELSE
        DISPLAY "Invalid credentials. Exiting..."
        EXIT   // Terminate the program if login fails
    END IF

    // Step 3: Admin Menu
    FUNCTION admin_menu()
        REPEAT
            DISPLAY "Admin Menu Options:"
            DISPLAY "1. View All Dishes"
            DISPLAY "2. Add New Dish"
            DISPLAY "3. Update Dish"
            DISPLAY "4. Delete Dish"
            DISPLAY "5. Search for Dishes"
            DISPLAY "6. Generate Sales Report"
            DISPLAY "7. Exit"
            
            DISPLAY "Enter your choice:"
            READ choice

            SWITCH choice:
                CASE 1: 
                    CALL display_dishes()   // Display all dishes
                    BREAK
                CASE 2: 
                    CALL add_dish()   // Add a new dish
                    BREAK
                CASE 3: 
                    CALL update_dish()   // Update an existing dish
                    BREAK
                CASE 4: 
                    CALL delete_dish()   // Delete a dish
                    BREAK
                CASE 5: 
                    CALL search_dishes()   // Search for dishes by name
                    BREAK
                CASE 6: 
                    CALL generate_sales_report()   // Generate a sales report
                    BREAK
                CASE 7: 
                    DISPLAY "Exiting Admin Panel."
                    EXIT   // Exit the program
                DEFAULT:
                    DISPLAY "Invalid choice! Please try again."
            END SWITCH
        UNTIL choice == 7   // Repeat until admin chooses to exit
    END FUNCTION

END
```

---

### **Key Points to Understand:**

1. **Login and Authentication**:
   - The admin must enter a **correct username** and **password**.
   - If the credentials are correct, the admin is granted access to the **Admin Menu**.

2. **Admin Menu**:
   - After successful login, the admin is shown a menu with options to manage dishes, view the sales report, or exit.
   - Based on the admin's choice, specific operations are triggered.

3. **Operations Available in Admin Menu**:
   - The admin can choose to **view all dishes**, **add a new dish**, **update an existing dish**, **delete a dish**, **search for dishes**, or **generate a sales report**.

4. **Repetition and Exit**:
   - The admin is given the choice to **exit** the menu or continue performing tasks until they decide to exit.

---

This is the correct **detailed flowchart** and **pseudocode** for the **Admin Panel with Authentication**. I hope this clears up any confusion! Let me know if you'd like further clarification.

### **Flowchart Diagram for Customer Panel**

Here is a detailed flowchart for the **Customer Panel** of the system. The customer can perform several actions, including viewing dishes, placing orders, canceling orders, viewing orders, and searching for dishes.

```
           +------------------------+
           |     Start Program       |
           +------------------------+
                    |
                    v
        +-------------------------------+
        |    Display Customer Menu      |
        |  1. View All Dishes           |
        |  2. Place Order               |
        |  3. Cancel Order              |
        |  4. View All Orders           |
        |  5. Search for Dishes         |
        |  6. Exit                      |
        +-------------------------------+
                    |
                    v
        +----------------------------+
        |    Customer Selects Action |
        +----------------------------+
                    |
                    v
        +---------------------------------------------+
        |           Is Action 1 (View Dishes)?      |
        +---------------------------------------------+
                    | No
                    | Yes
                    v
          +----------------------------+  
          |   Display All Dishes       |   
          +----------------------------+   
                    |                     
                    v
           +--------------------------+
           | Return to Customer Menu  |
           +--------------------------+
                    |
                    v
        +---------------------------------------------+
        |           Is Action 2 (Place Order)?       |
        +---------------------------------------------+
                    | No
                    | Yes
                    v
           +----------------------------+
           |    Collect Order Info      |
           +----------------------------+
                    |
                    v
           +----------------------------+
           | Validate Order Information |
           +----------------------------+
                    |
                    v
           +----------------------------+
           |    Save Order to File      |
           +----------------------------+
                    |
                    v
           +----------------------------+
           |  Display Order Confirmation|
           +----------------------------+
                    |
                    v
          +--------------------------+
          | Return to Customer Menu  |
          +--------------------------+
                    |
                    v
        +---------------------------------------------+
        |           Is Action 3 (Cancel Order)?      |
        +---------------------------------------------+
                    | No
                    | Yes
                    v
           +----------------------------+
           |    Cancel Order             |
           +----------------------------+
                    |
                    v
           +----------------------------+
           |  Display Cancel Confirmation|
           +----------------------------+
                    |
                    v
           +--------------------------+
           | Return to Customer Menu  |
           +--------------------------+
                    |
                    v
        +---------------------------------------------+
        |           Is Action 4 (View All Orders)?   |
        +---------------------------------------------+
                    | No
                    | Yes
                    v
           +----------------------------+
           |   Display All Orders       |
           +----------------------------+
                    |
                    v
           +--------------------------+
           | Return to Customer Menu  |
           +--------------------------+
                    |
                    v
        +---------------------------------------------+
        |           Is Action 5 (Search for Dishes)? |
        +---------------------------------------------+
                    | No
                    | Yes
                    v
           +----------------------------+
           |   Search for Dishes        |
           +----------------------------+
                    |
                    v
           +--------------------------+
           | Return to Customer Menu  |
           +--------------------------+
                    |
                    v
        +----------------------------+
        | Is Action 6 (Exit)?        |
        +----------------------------+
                    | Yes
                    v
            +----------------------+
            |    Exit Program      |
            +----------------------+

```

---

### **Pseudocode for Customer Panel**

Here is a pseudocode for the **Customer Panel** based on the flowchart:

```plaintext
Start Program

// Customer Menu Function
CustomerMenu():
    REPEAT
        DISPLAY "Customer Menu:"
        DISPLAY "1. View All Dishes"
        DISPLAY "2. Place Order"
        DISPLAY "3. Cancel Order"
        DISPLAY "4. View All Orders"
        DISPLAY "5. Search for Dishes"
        DISPLAY "6. Exit"
        INPUT choice

        IF choice == 1 THEN
            ViewAllDishes()
        ELSE IF choice == 2 THEN
            PlaceOrder()
        ELSE IF choice == 3 THEN
            CancelOrder()
        ELSE IF choice == 4 THEN
            ViewAllOrders()
        ELSE IF choice == 5 THEN
            SearchDishes()
        ELSE IF choice == 6 THEN
            ExitProgram()
        ELSE
            DISPLAY "Invalid choice! Please try again."

    UNTIL False

// View All Dishes
ViewAllDishes():
    // Retrieve and display all dishes
    DISPLAY all dishes from dishes file
    RETURN to CustomerMenu()

// Place Order
PlaceOrder():
    DISPLAY "Enter your name"
    INPUT customer_name
    DISPLAY "Enter your address"
    INPUT customer_address
    DISPLAY "Enter your phone number"
    INPUT customer_phone
    DISPLAY available dishes
    DISPLAY "Enter Dish ID to order"
    INPUT dish_id
    DISPLAY "Enter quantity"
    INPUT quantity

    // Retrieve dish details from file
    IF dish_id exists in dishes file THEN
        CALCULATE total cost = price * quantity
        CREATE order_id
        SAVE order to orders file (order_id, customer_name, customer_address, customer_phone, dish_id, total_cost, status)
        DISPLAY "Order placed successfully! Your Order ID is: " + order_id
    ELSE
        DISPLAY "Dish not found. Please try again."

    RETURN to CustomerMenu()

// Cancel Order
CancelOrder():
    DISPLAY "Enter Order ID to cancel"
    INPUT order_id

    // Check if order exists in orders file
    IF order exists THEN
        UPDATE order status to "Canceled"
        DISPLAY "Order " + order_id + " canceled successfully!"
    ELSE
        DISPLAY "Order not found."

    RETURN to CustomerMenu()

// View All Orders
ViewAllOrders():
    DISPLAY all orders for the customer from orders file
    RETURN to CustomerMenu()

// Search for Dishes
SearchDishes():
    DISPLAY "Enter dish name to search for"
    INPUT search_term
    DISPLAY matching dishes from dishes file based on search_term
    RETURN to CustomerMenu()

// Exit Program
ExitProgram():
    DISPLAY "Exiting... Thank you for using Delicious Eats!"
    EXIT
```

### **Explanation of Key Functions in the Pseudocode**:

1. **CustomerMenu()**: This function is a loop that continually displays the customer menu until the user chooses to exit. The customer selects an option, and the corresponding action is taken (view dishes, place an order, cancel an order, etc.).

2. **ViewAllDishes()**: This function displays all available dishes that the customer can choose from. The dish details are retrieved from the `dishes.txt` file.

3. **PlaceOrder()**: The customer provides their name, address, and phone number. The customer then selects a dish and specifies the quantity. The total cost is calculated, and the order is saved in the `orders.txt` file.

4. **CancelOrder()**: This function allows the customer to cancel an existing order by providing the order ID. If the order is found, its status is updated to "Canceled."

5. **ViewAllOrders()**: The customer can view all their previous orders from the `orders.txt` file.

6. **SearchDishes()**: The customer can search for a dish by entering a part of the dish's name. The system will display matching dishes.

7. **ExitProgram()**: This function ends the program when the customer chooses to exit.

---

### **Conclusion**:
This flowchart and pseudocode outline the functionality and flow for the customer panel in a food ordering system. It provides a straightforward way to interact with the system, allowing customers to view dishes, place orders, cancel orders, and search for dishes. The flowchart and pseudocode are designed to ensure that each step is clear and that the user experience is smooth and logical.
