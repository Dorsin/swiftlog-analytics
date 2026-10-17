# SwiftLog Analytics & Supply Chain AI Transformation Project

## Project Overview
SwiftLog Logistics is a nationwide supply chain and delivery operations network. This project focuses on end-to-end data auditing, relational database integration, statistical hypothesis testing, feature engineering, and predictive supply chain modeling across operational datasets.

## Relational Architecture & Dataset Coverage
The master analytical pipeline integrates 10 operational datasets sharing verified relational keys:
- **Orders & Customers:** Order status tracking (`Status_order`), customer urban locations, purchasing timelines.
- **Order Items & Products:** Unit pricing, item sales volumes, product categories.
- **Shipments & Delivery Performance:** Warehouse dispatches, transit delay durations (`DelayDays`), delivery status tracking (`Status_delivery`).
- **Warehouses, Inventory & Employees:** Regional warehouse locations, stock levels, staffing capacity.
- **Returns:** Product return tracking and failure reason classification.

*Note: The standalone reference dataset `SwiftLog_Suppliers.csv` is analyzed independently at the entity level to preserve strict relational data integrity, as it lacks direct foreign key bindings to products or dispatches.*

## Exact Repository Directory Structure
```text
Week5_DataScience_SwiftLog_DorianNJAMI/
│
├── Data/
│   ├── Cleaned_Datasets/
│   │   ├── Cleaned_SwiftLog_Customers.csv
│   │   ├── Cleaned_SwiftLog_Delivery_Perf.csv
│   │   ├── Cleaned_SwiftLog_Employees.csv
│   │   ├── Cleaned_SwiftLog_Inventory.csv
│   │   ├── Cleaned_SwiftLog_Order_Items.csv
│   │   ├── Cleaned_SwiftLog_Orders.csv
│   │   ├── Cleaned_SwiftLog_Products.csv
│   │   ├── Cleaned_SwiftLog_Returns.csv
│   │   ├── Cleaned_SwiftLog_Shipments.csv
│   │   ├── Cleaned_SwiftLog_Suppliers.csv
│   │   ├── Cleaned_SwiftLog_Warehouses.csv
│   │   ├── Feature_Engineered_Dataset.csv
│   │   └── SwiftLog_Master_Analytical_Dataset.csv
│   │
│   └── Original_Datasets/
│       ├── SwiftLog_Customers.csv
│       ├── SwiftLog_Data_Dictionary.csv
│       ├── SwiftLog_Delivery_Performance.csv
│       ├── SwiftLog_Employees.csv
│       ├── SwiftLog_Inventory.csv
│       ├── SwiftLog_Order_Items.csv
│       ├── SwiftLog_Orders.csv
│       ├── SwiftLog_Products.csv
│       ├── SwiftLog_Returns.csv
│       ├── SwiftLog_Shipments.csv
│       ├── SwiftLog_Suppliers.csv
│       └── SwiftLog_Warehouses.csv
│
├── Notebook/
│   └── Week5_DataScience.ipynb
│
├── Presentation/
├── Reports/
├── Visualizations/
└── README.md