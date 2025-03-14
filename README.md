# Reataurant-Management-Database
This project involves the creation of a Restaurant Management Database using PostgreSQL. The database is designed to streamline various aspects of restaurant operations, including menu management, staff scheduling, customer feedback, and sales tracking. The project was inspired by real-world observations at The View restaurant, where I work. The database aims to provide a robust and efficient system for managing restaurant activities.

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
- **restaurant**: Stores restaurant details, including the restaurant name.

section: Manages different sections of the restaurant (e.g., Pizza, Burgers).

menu_items: Tracks menu items, including names, descriptions, prices, and associated sections.

job_titles: Stores job titles for staff (e.g., Chef, Supervisor).

staff: Manages staff details, including roles, working hours, and salaries.

timesheet: Tracks staff working hours, attendance, and status.

customer_orders: Records customer orders, including order details and payment methods.

order_items: Links customer orders to menu items and tracks quantities.

customer_feedback: Collects and manages customer reviews, ratings, and comments.
