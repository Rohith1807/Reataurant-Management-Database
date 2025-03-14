# Restaurant-Management-Database
# Overview
This project is a Restaurant Management Database designed to streamline the operations of a restaurant. It includes tables for managing menu items, staff, customer orders, timesheets, and customer feedback. The database is built using PostgreSQL and incorporates triggers for automated ID generation and data validation.


# Key Features
1. **Core Functionality:**
- Menu item management.
- Staff scheduling and timesheets.
- Sales tracking and reporting.
- Customer feedback collection.
- Advanced queries for analyzing sales data, customer ratings, and inventory status.

2. **Database Design:**
- **Normalization**: The database follows normalization principles to minimize redundancy and ensure data integrity.
- **Primary and Foreign Keys**: Each table has a primary key, and foreign keys are used to establish relationships between tables.
- **Triggers**: Automate tasks such as updating sales totals and calculating staff sick leave.
- **Joins**: Combine data from multiple tables to generate insights like revenue by section and popular menu items.
- **Cascading**: Ensures data consistency by automatically updating or deleting related records.

# Tables Included
- `restaurant`: Stores restaurant details, including the restaurant name.
- `section`: Manages different sections of the restaurant (e.g., Pizza, Burgers).
- `menu_items`: Tracks menu items, including names, descriptions, prices, and associated sections.
- `job_titles`: Stores job titles for staff (e.g., Chef, Supervisor).
- `staff`: Manages staff details, including roles, working hours, and salaries.
- `timesheet`: Tracks staff working hours, attendance, and status.
- `customers_orders`: Records customer orders, including order details and payment methods.
- `order_items`: Links customer orders to menu items and tracks quantities.
- `customer_feedback`: Collects and manages customer reviews, ratings, and comments.
