# GROCERY DATABASE MONGODB QUERIES

This repository contains a collection of MongoDB queries designed for managing a grocery store database. The database includes five key collections: customers, departments, employees, products, and suppliers.

## Collections

The database includes the following five collections:

### 1. Customers

Stores information about customers who shop at the grocery store.

### Fields:

- name: Customer’s full name. <code>String</code>
- phone: Contact phone number. <code>Number</code>
- money_spent: Total money spent by customer. <code>Number</code>
- address: Customer Address. <code>String</code>
- join_date: Customer joined date <code>Date</code>

### 2. Departments

Stores information about departments at the grocery store.

### Fields:

- department_name: Department name. <code>String</code>
- manager_name: Department manager name. <code>String</code>
- manager_start_date: Department manager start date. <code>Date</code>

### 3. Employees

Stores information about employees who work at the grocery store.

### Fields:

- employee_name: Employee full name. <code>String</code>
- phone_number: Employee phone number. <code>Number</code>
- salary: Employee salary. <code>Number</code>
- join_date: Employee join date. <code>Date</code>
- address: Employee address. <code>String</code>

### 4. Products

Stores information about products at the grocery store.

### Fields:

- name: Product name. <code>String</code>
- price: Product price. <code>Number</code>
- quantity: Product quantity at store. <code>Number</code>

### 5. Suppliers

Stores information about suppliers of the grocery store.

### Fields:

- supplier_name: Supplier name. <code>String</code>
- email: Supplier email address. <code>String</code>
- phone: Supplier phone number. <code>Number</code>
- address: Supplier Address. <code>String</code>
- supply_product: Supplier products. <code>Array</code>
