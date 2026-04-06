# ShopNest Store: Power BI Data Analysis Project
## This project features a comprehensive Power BI dashboard designed to analyze the sales performance, logistics, and customer satisfaction of the **ShopNest Store**. By connecting multiple datasets—including orders, customers, products, and reviews—the dashboard provides actionable insights into revenue trends and operational challenges.

### Key Features & Insights

* **Revenue Performance**:
    * **Growth Trends**: Analyzed year-over-year revenue, showing a significant increase from 2016 to 2018. 
    * **Seasonal Patterns**: Identified peak sales in **Q4**, highlighting the impact of the festive season on business momentum. 
    * **Top Categories**: Discovered that **Health & Beauty**, **Watches & Gifts**, and **Bed Bath Table** are the primary revenue drivers. 

* **Logistics & Operational Efficiency**:
    * **Delivery Performance**: Compared on-time vs. delayed orders month-over-month. Insights show that delays tend to increase during peak sales periods at the end of the year. 
    * **Delay Hotspots**: Identified that high-volume categories like **Bed Bath Table** face the most logistical challenges. 

* **Customer & Geographic Analysis**:
    * **Regional Distribution**: Used a map visual to show high sales concentration in states like **São Paulo** and **Rio de Janeiro**, contrasted with lower performance in northern regions. 
    * **Payment Preferences**: Found a strong customer preference for **Credit Cards**, followed by **Boleto**. 
    * **Product Satisfaction**: Visualized the top 10 highest and bottom 10 lowest-rated products to help stakeholders address quality or service issues. 

---

### Technical Implementation

* **Data Modeling**: Established a robust relational schema connecting eight distinct datasets including Customers, Sellers, Orders, Order Items, Payments, Reviews, Products, and Geolocation. 
* **DAX Measures**: Developed custom calculations for key business metrics, including:
    * **Total Sales**: `sum(Price) + sum(Freight Value)`. 
    * **Delayed Orders**: Calculated using a `DISTINCTCOUNT` of Order IDs where the delivery date exceeded the estimate. 
    * **Average Rating**: Calculated using `AVERAGEX` across related review tables. 
* **UI/UX Strategy**: Implemented a strategic color scheme: **Green** for high performance, **Red** for areas requiring attention (like delayed orders), and **Blue** for neutral trend data. 

---

### Visualizations Included
* **Clustered Column & Bar Charts**: For category and monthly comparisons. 
* **Donut Chart**: For payment method distribution. 
* **Line Charts**: For seasonal and yearly revenue trends. 
* **Map Visual**: For interactive geographic sales analysis. 
