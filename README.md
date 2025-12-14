# invetory_tracking

## Group Members
- **Munezero Denys** – 24RP11881  
- **Ajeneza Aline** – 24RP04472  

PROJECT NAME:INVETORY TRACKER


How the PHP Inventory Tracker Works:

The inventory tracker system built in PHP works by connecting the user interface (forms and tables) with a MySQL database to manage product stock automatically.

User Input (Frontend):

The user adds products using a PHP/HTML form (product name, quantity, price, category, etc.).

Forms use POST method to send data securely.

Data Processing (PHP Backend):

PHP receives the form data using $_POST.

Input is validated (empty fields, correct data types).

Prepared statements (PDO or MySQLi) are used to prevent SQL injection.

Database Storage (MySQL):

Products are stored in an inventory table.

Each item has fields like product_id, product_name, quantity, price, and created_at.

Stock Tracking:

When items are added, quantity increases.

When items are sold or removed, quantity decreases.

PHP updates the database in real time using UPDATE queries.

Viewing Inventory:

PHP fetches data using SELECT queries.

Results are displayed in a table showing current stock levels.

Low-stock items can be highlighted automatically.

Editing & Deleting Items:

Admin can update product details or delete items.

Actions are confirmed before execution to avoid mistakes.

Security & Control:

Sessions ($_SESSION) ensure only authorized users access the system.

Passwords are securely hashed using password_hash().

Reports & Insights (Optional):

The system can calculate total stock value.

Shows best-selling or low-stock items.
