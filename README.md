Project Overview:
This repository contains a full-stack relational database implementation designed to manage airline retail operations. The system handles customer profiles, inventory management, order processing, and line-item tracking. It features a normalized schema (3NF), complex analytical views, and optimized query logic.

Technical Architecture:
The database is built on a relational model with five core entities designed to maintain data integrity and minimize redundancy:

Customers: Stores demographic and contact information, including credit limits and geographic data.

Orders: Tracks transaction headers, including dates and financial totals, linked to customer profiles.

Products & Parts: A two-tier inventory system where products are linked to specific components (parts).

Order Line Items: A junction table managing the many-to-many relationship between orders and products, including quantity and unit pricing.

Key Features
Relational Integrity: Implemented using Primary and Foreign Key constraints with CASCADE delete protection.

Advanced Data Types: Utilized custom ENUM types to track order status (Ordered, Out_For_Shipping, Delivered).

Analytical Views:

Dynamic Views: To filter and monitor specific customer segments.

Materialized Views: To pre-calculate complex aggregations for high-frequency financial reporting.

Complex Query Logic: Includes multi-table joins, aggregate functions (SUM, AVG, COUNT), and conditional filtering using HAVING and LIKE clauses.

Tech Stack
Database Engine: PostgreSQL

Core Concepts: DDL/DML Scripting, 3NF Normalization, Referential Integrity, Materialized Views.
