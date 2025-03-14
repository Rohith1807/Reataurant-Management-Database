# Restaurant-Management-Database
# 📝 Overview
This project is a Restaurant Management Database designed to streamline the operations of a restaurant. It includes tables for managing menu items, staff, customer orders, timesheets, and customer feedback. The database is built using PostgreSQL and incorporates triggers for automated ID generation and data validation.


# ⚙️ Key Features
# 1. **Core Functionality:**
- Menu item management.
- Staff scheduling and timesheets.
- Sales tracking and reporting.
- Customer feedback collection.
- Advanced queries for analyzing sales data, customer ratings, and inventory status.

# 2. **Database Design:**
  - **Normalization**: The database follows normalization principles to minimize redundancy and ensure data integrity.
  - **Primary and Foreign Keys**: Each table has a primary key, and foreign keys are used to establish relationships between tables.
  - **Triggers**: Automate tasks such as updating sales totals and calculating staff sick leave.
  - **Joins**: Combine data from multiple tables to generate insights like revenue by section and popular menu items.
  - **Cascading**: Ensures data consistency by automatically updating or deleting related records.

# 📋 Tables Included
- `restaurant`: Stores restaurant details, including the restaurant name.
- `section`: Manages different sections of the restaurant (e.g., Pizza, Burgers).
- `menu_items`: Tracks menu items, including names, descriptions, prices, and associated sections.
- `job_titles`: Stores job titles for staff (e.g., Chef, Supervisor).
- `staff`: Manages staff details, including roles, working hours, and salaries.
- `timesheet`: Tracks staff working hours, attendance, and status.
- `customers_orders`: Records customer orders, including order details and payment methods.
- `order_items`: Links customer orders to menu items and tracks quantities.
- `customer_feedback`: Collects and manages customer reviews, ratings, and comments.

# 📋 Triggers
- `set_menuitem_id`: Generates composite IDs for menu items.
- `generate_unique_staff_id`: Generates custom IDs for staff.
- `calculate_total_amount`: Automates sales total calculation.
- `check_hours_before_insert_or_update`: Enforces weekly working hour limits.
- `calculate_sick_leave_hours`: Tracks sick leave based on hours worked.
- `update_sales_and_totals`: Synchronizes order_items and sale_items.

# 📁 Code and Resources
- `CREATE TABLE` commands were manually written.
- Mock Data(`Insert`): Generated using ChatGPT and customized to fit the project requirements.
- `Triggers`: Initial scripts were generated using ChatGPT and then modified to meet specific needs.
- `ER diagram` is shared for better understanding.
- All code and related resources are organized in the shared directory.

# 💡How to Use
1. Clone the repository.
2. Set up a PostgreSQL database.
3. Run the provided SQL scripts to create tables, insert mock data, and set up triggers.
4. Use the sample queries to generate insights and analyze data.

# 🔍 Conclusion
This project has been a valuable learning experience in database design and management. While there are areas for improvement, the current implementation provides a solid foundation for managing restaurant operations efficiently. Future enhancements will focus on expanding functionality and refining existing features.
