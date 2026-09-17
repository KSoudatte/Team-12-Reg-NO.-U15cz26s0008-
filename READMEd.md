README.txt
Project Title: Pharmacy – Medicine Sale & Billing System
1. Project Description
The Pharmacy – Medicine Sale & Billing System is a database management system designed to manage medicine details, customer information, medicine sales, sale items, suppliers, pharmacists, and billing.
The system helps maintain accurate medicine stock, record customer purchases, calculate bills, and manage pharmacy-related information efficiently.
2. Main Features
Medicine details management
Customer details management
Medicine quantity and stock management
Medicine sale management
Sale item management
Bill generation and calculation
Supplier details management
Pharmacist details management
Discount and GST/Tax calculation
Updated stock after medicine sale
3. Entities
The system contains the following entities:
CUSTOMER
SALE
BILL
MEDICINE
SALE_ITEM
SUPPLIER
PHARMACIST
4. Relationships
The ER diagram contains 7 entity-to-entity relationships:
CUSTOMER — MAKES — SALE
Cardinality: 1 : N
SALE — GENERATES — BILL
Cardinality: 1 : 1
SALE — CONTAINS — SALE_ITEM
Cardinality: 1 : N
MEDICINE — IS_INCLUDED_IN — SALE_ITEM
Cardinality: 1 : N
SUPPLIER — SUPPLIES — MEDICINE
Cardinality: 1 : N
PHARMACIST — PROCESSES — SALE
Cardinality: 1 : N
PHARMACIST — MANAGES — MEDICINE
Cardinality: 1 : N
5. Database Keys
Primary Keys
Customer_ID
Sale_ID
Bill_ID
Medicine_ID
Sale_Item_ID
Supplier_ID
Pharmacist_ID
Foreign Keys
CUSTOMER_ID in SALE
SALE_ID in BILL
SALE_ID in SALE_ITEM
MEDICINE_ID in SALE_ITEM
6. Bill Calculation
The system calculates:
Sale Amount = Price × Quantity
Final Bill Amount = Subtotal − Discount + GST/Tax
After a successful sale, the medicine stock is updated:
Updated Stock = Available Stock − Quantity Sold
7. ER Diagram Notation
Rectangle → Entity
Oval → Attribute
Diamond → Relationship
Underlined Attribute → Primary Key
FK → Foreign Key
1 : N → One-to-Many Relationship
1 : 1 → One-to-One Relationship
8. Objective
The main objective of this project is to provide a simple and organized system for managing pharmacy medicine sales and billing while maintaining customer, medicine, supplier, pharmacist, stock, and billing information in a structured database.
