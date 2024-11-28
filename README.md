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


###2 
I chose **arrays of structures** to handle dishes and orders in this program because they allow me to store different types of data (such as `int`, `char`, `float`) together in a single array. Each structure, like `Dish` and `Order`, encapsulates all related information: for example, the `Dish` structure includes `char` for the dish ID and name, `float` for price, and `int` for preparation time. Similarly, the `Order` structure stores customer details, order ID, and order status.

Using arrays of structures offers several advantages. First, it simplifies data management, as each array element is a complete record (dish or order) containing all the necessary fields. Arrays allow easy indexing to access, update, or remove specific records. This method also avoids the complexity of dynamic memory allocation, which makes the code more manageable and easier to maintain. Overall, using structures provides an organized and efficient way to store and manipulate multiple types of data within a single array, making it ideal for this application.

### **Project Plan for Restaurant Order Management System**

---

#### **1. Project Overview:**

This project involves developing a **Restaurant Order Management System** that allows two types of users: **Customers** and **Admins**. The system will enable customers to place and manage their orders, while admins will have the ability to manage the menu and generate sales reports. The program interacts with two main text files: `dishes.txt` for menu items and `orders.txt` for customer orders.

---

#### **2. Requirements List:**

The following are the key requirements for this project:

1. **User Authentication**:
   - Admin users must authenticate using a username and password.
   
2. **Admin Functionalities**:
   - View all dishes in the menu.
   - Add new dishes to the menu.
   - Update existing dishes (name, description, price, preparation time).
   - Delete dishes from the menu.
   - Search for dishes by name.
   - Generate a sales report showing total revenue from orders.
   
3. **Customer Functionalities**:
   - View available dishes.
   - Place orders by selecting a dish and specifying quantity.
   - View current orders.
   - Cancel placed orders.
   - Search for dishes by name.
   
4. **Data Storage**:
   - All dish information will be stored in a file named `dishes.txt`.
   - All order information will be stored in a file named `orders.txt`.
   
5. **Sales Reporting**:
   - Admin should be able to generate a report showing the total sales from orders.
   
6. **File Handling**:
   - The program will read from and write to `dishes.txt` and `orders.txt` to handle menu and order data.

7. **User Interface**:
   - The system will have a text-based menu where users can select options to perform the various tasks.

---

#### **3. How Requirements Will Be Satisfied:**

1. **User Authentication**:
   - The system will prompt the admin for a username and password. If the credentials match predefined values (e.g., "admin" and "password123"), the admin will be granted access to the admin menu. If the credentials are incorrect, access will be denied.
   - The customer will be able to use the system directly without authentication.

2. **Admin Functionalities**:
   - **View All Dishes**: Admin can view all dishes stored in `dishes.txt`. The system will use `awk` to format and display the dish information.
   - **Add New Dish**: Admin can add a new dish by entering its details (ID, name, description, price, preparation time). The new dish will be appended to `dishes.txt` using the `echo` command.
   - **Update Existing Dish**: Admin can search for a dish by ID and update its details using the `sed` command.
   - **Delete Dish**: Admin can delete a dish from `dishes.txt` using `sed` to remove the line corresponding to the dish ID.
   - **Search Dishes**: Admin can search for dishes by name using `grep` to find matching records in `dishes.txt`.
   - **Generate Sales Report**: Admin can view a sales report, which sums the total revenue from orders in `orders.txt` using `awk`.

3. **Customer Functionalities**:
   - **View Dishes**: Customers can view the list of dishes available for order, displayed using `awk` from `dishes.txt`.
   - **Place Order**: Customers can select a dish, specify the quantity, and the system will calculate the total cost based on the dish's price and quantity. A new order will be added to `orders.txt` using the `echo` command.
   - **View Orders**: Customers can view the details of their placed orders, extracted from `orders.txt` using `awk`.
   - **Cancel Order**: Customers can cancel an order by entering its ID. The system will use `sed` to mark the order as "canceled" in `orders.txt`.
   - **Search for Dishes**: Customers can search for dishes by name using `grep`.

4. **Data Storage**:
   - **`dishes.txt`** will contain menu data, including dish IDs, names, descriptions, prices, and preparation times.
   - **`orders.txt`** will contain order data, including order IDs, customer details, dish ID, quantity, total cost, and order status (e.g., "Pending" or "Canceled").
   - These files will be updated and queried using bash commands like `echo`, `sed`, `awk`, and `grep`.

5. **Sales Reporting**:
   - **Admin** can generate a sales report by using an `awk` command that reads through `orders.txt`, calculates the total sales, and displays it along with individual order details.

6. **File Handling**:
   - The program will interact with `dishes.txt` and `orders.txt` through bash commands to read, write, update, and delete data as required by the operations being performed.

7. **User Interface**:
   - The system will provide a text-based menu for both **Admin** and **Customer**:
     - The admin menu will offer options to manage dishes, view dishes, and generate sales reports.
     - The customer menu will offer options to view dishes, place orders, cancel orders, and view their orders.

---

#### **4. Plan for Implementation:**

The development of the project will be carried out in several phases:

1. **Phase 1: System Design & Setup**
   - Define the structure of `dishes.txt` and `orders.txt` files.
   - Design the user interface (menus for Admin and Customer).
   - Set up functions for viewing, adding, and deleting dishes from `dishes.txt`.

2. **Phase 2: Order Management Features**
   - Implement order placement functionality (add order to `orders.txt`).
   - Implement order cancellation functionality (mark order as canceled in `orders.txt`).
   - Implement the order display function (view orders placed by customers).

3. **Phase 3: Admin Features**
   - Implement the functionality for searching, adding, updating, and deleting dishes.
   - Implement sales reporting functionality to calculate total sales using `awk`.

4. **Phase 4: Testing & Debugging**
   - Test all functionalities (order placement, dish management, report generation).
   - Debug any issues that arise during testing.

5. **Phase 5: Final Review & Deployment**
   - Conduct a final review of the program and ensure that all features are working correctly.
   - Prepare documentation for users (Admin and Customer) on how to use the system.

---

#### **5. Conclusion:**

By following the outlined project plan, this **Restaurant Order Management System** will be developed to meet all functional requirements. The use of bash commands for file manipulation and data processing ensures that the system remains lightweight and efficient. This plan provides a clear roadmap for the development of the system, from the initial design phase to final deployment.

Sure, here are concise answers for each question:

### 1. **How does memory management play a role in the structured programming design of the food delivery system?**

Memory management is essential for optimizing the resources in the food delivery system. Structured programming involves breaking down the program into logical blocks, and efficient memory management ensures that each block has the appropriate memory allocated to it. For instance, dynamically allocating memory for customer orders or dish details helps the system handle unpredictable data sizes without wasting resources. This makes the program more scalable and avoids memory overflow or exhaustion, ensuring smooth operations.

### 2. **Would dynamic memory allocation be necessary for handling orders?**

Yes, dynamic memory allocation is necessary for handling orders in a food delivery system. Since the number of orders placed at any time can vary, dynamically allocating memory for each order (such as customer details, order items, and prices) allows the system to efficiently store and manage data without reserving excessive memory. As each order is created or modified, memory can be allocated or freed as needed.

### 3. **How would you avoid memory leaks in such a system?**

To avoid memory leaks, the system must ensure that all dynamically allocated memory is properly freed after it's no longer needed. This can be achieved by using functions such as `free()` in C to release memory that was previously allocated using functions like `malloc()` or `calloc()`. It's also important to set pointers to `NULL` after freeing them, which prevents accidental access to deallocated memory. Additionally, using proper memory management tools, like memory debuggers (e.g., Valgrind), can help identify any memory leaks during the development phase. Regularly testing the system for memory usage is essential for maintaining its stability.

### 4. **Why is dynamic memory allocation important for this system?**

Dynamic memory allocation is important because it provides flexibility in handling various amounts of data. The food delivery system's size and number of orders will change over time, and dynamic allocation allows it to use only the memory that is actually needed. This reduces the risk of memory waste (when data does not require fixed-sized memory) and ensures that resources are efficiently managed, especially when handling large datasets like orders, customer details, and menu items.

### What I Have Learned

- **Structured Programming**: Learned to modularize code in C for better maintenance and readability.
- **Bash Integration**: Used Bash for file handling and system-level operations, improving automation and efficiency.
- **File Management**: Gained experience managing data with text files (`dishes.txt`, `orders.txt`) and using tools like `awk`, `grep`, and `sed`.
- **Memory Management**: Learned that while static arrays suffice for simple systems, dynamic memory allocation (`malloc`, `free`) is crucial for scalability.

### System Improvements and Development

- **Database Integration**: Move from text files to a relational database for better performance, scalability, and data integrity.
- **User Authentication**: Implement secure password hashing and role-based access control (RBAC).
- **Dynamic Memory**: Use dynamic memory allocation for handling large data sets and prevent memory leaks.
- **Payment Gateway**: Integrate online payment systems (e.g., Stripe, PayPal) for secure transactions.
- **UI Enhancement**: Transition from text-based to GUI or mobile interface for improved user experience.
- **Order Tracking**: Implement real-time status updates and notifications for customers.
- **Analytics**: Add sales analytics and data visualization for performance insights.
- **Scalability**: Improve load handling with cloud infrastructure and optimization techniques.

By making these improvements, the system would be more robust, secure, and scalable, offering a better user experience and easier management.

