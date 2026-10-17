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

## Repository Directory Structure
```text
Week5_DataScience_SwiftLog_DorianNJAMI/
│
├── Data/
│   ├── Cleaned_Datasets/         # Processed CSVs, Master Analytical Dataset, & Feature Engineered Dataset
│   └── Original_Datasets/        # Raw 11 operational logistics CSV datasets
│
├── Notebook/
│   ├── Week5_DataScience.ipynb   # Main Jupyter Notebook containing complete analysis & pipeline
│   └── Week5_DataScience.html    # HTML export of the complete notebook
│
├── Presentation/
│   └── Executive_Presentation.pptx # Executive PowerPoint presentation (12 slides)
│
├── Reports/
│   ├── Data_Profiling_Report.html  # Automated profiling quality report
│   ├── Executive_Summary.pdf       # Standalone executive report
│   └── Technical_Report.pdf        # Complete technical report
│
├── Visualizations/
│   ├── Charts/                   # Extracted high-resolution PNG visualizations (Visual_01 to Visual_17)
│   └── Dashboards/
│
└── README.md