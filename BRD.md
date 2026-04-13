# Business Requirements Document (BRD) for MVP Smart Inventory System

## 1. Executive Summary  
The purpose of this document is to outline the Minimum Viable Product (MVP) for the Smart Inventory System. This MVP will focus on essential features that provide the foundational elements necessary to manage stock and warehouse operations effectively. The aim of this document is to clarify the scope, features, and requirements needed to launch the product while ensuring a lean and efficient development process.

### MVP Scope  
The MVP will focus on core functionalities that are required for the system to operate efficiently in a real-world environment, targeting immediate needs while allowing for future enhancements.

## 2. Core MVP Features  
1. **Product/Supplier/Warehouse CRUD**  
   - Ability to Create, Read, Update, and Delete products, suppliers, and warehouses.  
2. **Stock In/Out**  
   - Manage stock levels with functionalities to record stock increase (inbound) and decrease (outbound).  
3. **Basic Auto-PO**  
   - Automatic generation of Purchase Orders (POs) based on predefined stock thresholds.  
4. **Goods Receipt**  
   - Record receipt of goods against POs, allowing for verification and tracking.  
5. **Basic Analytics**  
   - Provide essential reports on stock levels, sales, and usage trends.
6. **User Authentication/RBAC**  
   - Secure user access with Role-Based Access Control (RBAC), managing permissions for Admin and Warehouse Manager roles.
7. **Audit Logging**  
   - Enable tracking of changes and actions taken within the system for accountability and auditing purposes.
8. **Notifications**  
   - Notify users about critical updates such as low stock alerts and received goods.

## 3. Primary User Roles  
1. **Admin**  
   - Full access to all system features, user management, and settings.  
2. **Warehouse Manager**  
   - Manage stock, processes orders, and oversee warehouse operations.

## 4. Simplified Technical Architecture  
- Frontend: Web-based UI using React.js  
- Backend: Node.js with Express  
- Database: PostgreSQL  
- Hosting: AWS

## 5. Essential Database Tables  
1. Users  
2. Products  
3. Suppliers  
4. Warehouses  
5. Stock Movements  
6. Purchase Orders  
7. Goods Receipts  
8. Notifications  
9. Audit Logs  
10. Roles  
11. Permissions  
12. Analytics

## 6. Core API Endpoints  
1. `POST /api/products`  
2. `GET /api/products`  
3. `GET /api/products/:id`  
4. `PUT /api/products/:id`  
5. `DELETE /api/products/:id`  
6. `POST /api/suppliers`  
7. `GET /api/suppliers`  
8. `UPDATE /api/suppliers/:id`  
9. `POST /api/stock-in`  
10. `POST /api/stock-out`  
11. `POST /api/purchase-orders`  
12. `GET /api/purchase-orders/:id`  
13. `POST /api/goods-receipts`  
14. `GET /api/analytics`  
15. `POST /api/login`  
16. `GET /api/logout`  
17. `GET /api/notifications`  
18. `GET /api/audit-logs`  
19. `POST /api/users`  
20. `PUT /api/users/:id`  
21. `DELETE /api/users/:id`

## 7. 8-Week Development Roadmap  
- **Sprint 1 (Weeks 1-2)**: User authentication, User roles and permissions setup  
- **Sprint 2 (Weeks 3-5)**: Core CRUD functionalities for Products, Suppliers, and Warehouses. Implement Stock In/Out features.  
- **Sprint 3 (Weeks 6-8)**: Basic Auto-PO, Goods Receipt, Analytics, Notifications, and auditing features.

## 8. Simplified Workflows  
### Stock Tracking  
- Input stock levels, record stock in/out, generate reports.
### Basic PO Workflow  
- Generate POs based on stock threshold, accept goods receipt.
### Essential Notifications  
- Notify users on low stock, received goods, and user activity.

## 9. Simplified Technology Stack  
- Frontend: React.js  
- Backend: Node.js  
- Database: PostgreSQL

## 10. Clear MVP vs Future Phase Features  
### MVP Features  
- Product management  
- Stock tracking  
- Basic PO automation  
- User authentication  
  
### Future Phase Features  
- Advanced Analytics and Forecasting  
- Enhanced User Roles and Permissions  
- Integration with external systems

---  
This document is intended to provide a concise, clear understanding of the MVP for the Smart Inventory System, demonstrating its practicality and potential for scalability.  
