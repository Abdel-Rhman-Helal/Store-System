# Store Management System (SMS)

## Table of Contents

1. [Overview](#overview)  
   1.1 [Directory Setup](#directory-setup)  
2. [Project Description](#project-description)  
3. [Intended Users](#intended-users)  
4. [Version History](#version-history)  
5. [Project Scope](#project-scope)  
6. [Terminology](#terminology)  
7. [User Groups & Goals](#user-groups--goals)  
8. [System Features](#system-features)  
9. [Technical Limitations](#technical-limitations)  
10. [System Architecture](#system-architecture)  
11. [Functional Specifications](#functional-specifications)  
12. [User Interfaces & Dependencies](#user-interfaces--dependencies)  
13. [Quality Attributes](#quality-attributes)  
14. [System Diagrams](#system-diagrams)  

---

## Overview<a name="overview"></a>

The **Store Management System (SMS)** is a desktop-based solution developed to enhance and automate retail operations. This document introduces the system's purpose and usage guidelines for customers, store managers, and delivery staff.

### Directory Setup<a name="directory-setup"></a>

Ensure the `pyqt5` directory is located in the `C:` drive. This folder should contain all the image assets used within the application interface.

---

## Project Description<a name="project-description"></a>

This system is built to simplify the shopping workflow by combining product browsing, cart management, and administrative control into a single interface. It supports multiple user types with role-specific capabilities, providing a complete experience from item selection to delivery.

---

## Intended Users<a name="intended-users"></a>

- **Customers**: Can view products, manage their shopping cart, place orders, and check past purchases.  
- **Administrators**: Oversee inventory, handle user data, and maintain system integrity.  
- **Delivery Staff**: Responsible for confirming order deliveries and reviewing assigned tasks.

---

## Version History<a name="version-history"></a>

| Version | Author | Change Summary      | Date       |
|---------|--------|----------------------|------------|
| 0.1     | B3B3   | Initial version      | 30-11-2023 |
| 0.2     | B3B3   | Added Use Cases      | 11-12-2023 |
| 0.3     | B3B3   | Created Class Diagram| 17-12-2023 |
| 0.4     | B3B3   | Added Sequence Diagrams | 21-12-2023 |

---

## Project Scope<a name="project-scope"></a>

The system is designed to support a digital storefront accessible to both internal and external users. Its key functionalities include order processing, inventory management, and delivery tracking. The system operates offline and interacts with a local database.

---

## Terminology<a name="terminology"></a>

- **FOEHU**: Faculty of Engineering, Helwan University  
- **B3B3**: Project development team name  
- **SMS**: Store Management System  
- **SQLite3**: The local database system used  

---

## User Groups & Goals<a name="user-groups--goals"></a>

### Developers (System Engineers)
- **Goal**: Acquire practical experience in software engineering through implementation and documentation.

### Customers
- **Goal**: Easily locate products, place orders efficiently, and reduce shopping time and effort.

### Delivery Staff
- **Goal**: Complete deliveries to customers and track order assignments.

### Administrators
- **Goal**: Maintain store operations, monitor system status, and resolve potential issues quickly.

---

## System Features<a name="system-features"></a>

1. Product categorization and insertion  
2. Product deletion and inventory pruning  
3. Product listing and display for all users  
4. Shopping cart functionality (add/remove items)  
5. User registration and secure login  
6. Order confirmation and purchase tracking  
7. Delivery confirmation by designated personnel  
8. Order status checking by users

---

## Technical Limitations<a name="technical-limitations"></a>

- **Login Security**: Only authenticated users can interact with the system's features.  
- **Local Storage Security**: All user and order data is stored securely within the local SQLite3 database on the user’s device.

---

## System Architecture<a name="system-architecture"></a>

The complete system architecture is outlined in the design document under Figure 1. It describes the relationships between users, the database, and the application layers.

---

## Functional Specifications<a name="functional-specifications"></a>

### Add Product to Inventory
Admins can insert new items under specific categories.

### Remove Product
Admins can delete items no longer available in the store.

### Display Products
All registered users and admins can browse the full catalog.

### Cart Management
Customers can add or remove items from their shopping carts.

### Order Management
Customers can finalize their purchases, view history, and check delivery statuses.

### Account System
Users can create new accounts or log in with existing credentials.

### Delivery Processing
Delivery staff confirm when orders have been fulfilled and mark them accordingly.

---

## User Interfaces & Dependencies<a name="user-interfaces--dependencies"></a>

### User Interface
The UI is built using PyQt5 and incorporates image resources for better usability. Screenshots are available in the documentation.

### Software Integration
- **Database**: Communicates with SQLite3 for storing user data, product information, and order logs.

---

## Quality Attributes<a name="quality-attributes"></a>

1. **Performance**: All system interactions should be fast and responsive.  
2. **Availability**: The application should run reliably without frequent failures.  
3. **Usability**: Interfaces should be intuitive and user-friendly.  
4. **Security**: Personal user data should be protected and visible only to the admin when necessary.

---

## System Diagrams<a name="system-diagrams"></a>

For deeper insight into the project’s flow and relationships, refer to the following diagrams in the supplementary materials:

- Use Case Diagram  
- Class Diagram  
- Entity Relationship (ER) Diagram  
- Sequence Diagram

---

This system provides a comprehensive platform for managing online and offline store operations. It brings together developers, customers, and staff in a unified application designed for efficiency, reliability, and scalability.
