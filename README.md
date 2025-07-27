# Project Title: AdventureWorks Sales Intelligence Dashboard
    An interactive Power BI dashboard that uncovers sales trends, customer insights, and product performance using the AdventureWorks dataset. This project applies storytelling, AI visuals (Key Influencers & Decomposition Tree), and bookmarks to deliver business intelligence in a visually compelling way.
# Objective: 
- To analyze sales data from AdventureWorks and provide decision-makers with actionable insights on:
    - Overall business performance
    - Product and category trends
    - Customer segments
    - Key factors influencing revenue
      
# Key Features:
### 1. Perfomance Overview:
- 📊 Executive Cards
  - Track Total Revenue, Total Profit, Total Orders, and Return Rate
  - Designed using SVG visuals for modern, intuitive insights
- 📈 Trend Analysis
  - Monthly Revenue Trends: Visualized using a Line Chart segmented by Start of Month to highlight seasonal patterns, performance growth, and detect anomalies in revenue behavior.
- 🗂️ Category-Wise Order Distribution: Stacked Bar Chart representing Total Orders split by Product Category for quick comparison of category performance.
- 📊 Top Product Highlights
   - Top Product Type by Orders - Highlighted using a KPI Card to display the most ordered product subcategory across all transactions.
   - Top Product Type by Returns - A KPI Card showing the product subcategory with the highest return volume, helping identify quality or customer satisfaction issues.
   - Top 10 Product Insights - A Matrix visual ranking products by Total Orders, Revenue, and Return %, offering a multidimensional view of high-performing products and used conditional formating upon orders on value that shows positive and negative and add background for revenue that indicates min and max values.
- 📅 Monthly KPIs with Benchmarking
  - Monthly Revenue, Orders, and Returns with:
    - Trend Axis – Start of Month
    - Target Value – Compared to Previous Month for performance benchmarking
- 🧭 User Navigation Controls
  - Reset Filters are implemented by using bookmarks, Go to Filters Page, and Navigate Between Report Pages using interactive buttons
- 🕵️‍♀️ Hidden Slicers for Global Filtering
   - Year Slicer – Applied silently to filter all visuals
   - Continent Slicer – Used to drive consistent geographic-level analysis across visuals
   - Back Navigation button
<p align="center">
  <img src="https://github.com/user-attachments/assets/bd75f6e5-c634-4f92-ab57-5f4bc52caeab" width="600" height="300" alt="image" />
</p>
     
### 2. Product Details:
- 🔍 Dynamic Product Drillthrough
   - Automatically displays selected product details from the Performance Overview matrix via drillthrough.
   - Highlights the selected product name using a card visual.
- 🎯 Target Tracking with Gauge Charts
  - Monthly KPIs visualized using gauge charts:
     - Orders vs. Target
     - Revenue vs. Target
     - Profit vs. Target
  - Targets are dynamically calculated as a 10% increase over previous month's performance.
- 📈 Profit Trend Analysis
  - Line chart with Date Hierarchy showing both:
     - Total Profit
     - Adjusted Profit 
  - Interactive features like drill up/down and data markers enhance trend visibility.
- ⚙️ Custom Price Adjustment Parameter - Used Numeric Parameter to allow users to simulate Price Adjustment % slicer impact on profits in real-time.
- 📊 Product Metric Selector with Dynamic Visualization
    - A slicer allows users to switch between key metrics:
        - Orders, Revenue, Profit, Returns, Return %
    - Based on selection, a dynamic Area Chart updates accordingly with full drilldown capability on the Date Hierarchy.
- 🎛️ Interactive Filtering & Granularity Control
   - Enables users to view metrics at different time granularities:
      - Yearly, Monthly, Weekly
      - Makes the product-level analysis both deep and flexible.
- 🔁 Smooth Navigation
   - Interactive Buttons allow:
      - Seamless page transitions and Reset Filter button available to restore default view instantly
      - Back button to return to Performance Overview
<p align="center">
    <img width="600" height="300" alt="Screenshot 2025-07-27 202544" src="https://github.com/user-attachments/assets/a950c2f7-241b-4d11-907e-2f247ee7c206" />
</p>

### 3. Customer Detail:
- 📌 Customer Overview Cards
    - Unique Customers Count
    - Average Revenue per Customer
- 🎚️ Interactive Customer Metric Selection
   - Toggle between Total Orders and Revenue per Customer
   - All related visuals respond dynamically
- 📈 Customer Trend Analysis
   - Line Chart with Date Hierarchy
   - Tracks Total Customers and Revenue per Customer
   - Dynamically changes based on selected metric
- 📅 Time-Based Filtering - Between-style Year Slicer for easy temporal analysis
- 🍩 Customer Segmentation
   - Donut Charts:
      - Orders by Income Level
      - Orders by Occupation
- 💡 Smart Insights with Actionable Filters
    - Information Button:
      - Displays a dynamic message as “Among customers in skilled manual roles in 2022, Ruban Suarez drove the most revenue at $4,683.”
      - On click, filters all visuals to focus on this customer segment
- 🧾 Top Customer Detail Cards
    - This Cards Shows:
       - Full Name
       - Total Orders
       - Total Revenue
    - Displays accurate info for top 1 customer, else shows "Multiple Customers"
- 🏅 Top 100 Customers Table
  - Ranked by:
     - Customer Key
     - Total Orders
     - Revenue
  - Conditional Formatting:
      - Orders: Highlighted with color indicators (positive/negative)
      - Revenue: Background gradient from min to max
- 🔁 User Experience Enhancements
  - Reset bookmarks restore original filters with a single click
  - Navigation Buttons for:
      - Smooth transitions
      - Back to previous page
<p align="center">
   <img width="600" height="300" alt="Screenshot 2025-07-27 202711" src="https://github.com/user-attachments/assets/9289b6db-c114-43bc-94e7-97450cc1115c" />
</p>

### 4. Map:
- 🌍 Interactive Sales Map
    - Grayscale World Map visual
    - Bubble Size represents Sales Volume per country:
    - Larger bubble = higher sales
- 🌐 Continent-Based Drilldown Tiles
   - Quick filter buttons to view:
      - Select All – Shows global sales distribution
          - Europe
          - North America
          - Pacific
    - Dynamically filters map and related visuals to selected region
- 🔁 Smooth Page Navigation
     - Reset Filters – Clears applied filters instantly
     - Interactive buttons improve overall user experience
<p align="center">
  <img width="600" height="300" alt="Screenshot 2025-07-27 202834" src="https://github.com/user-attachments/assets/15aa397b-3bf4-402c-ae97-fec5144999ad" />
</p>

### 5. Decomposition Tree:
- 🔍 Root-Cause Analysis of Total Orders
   - Used Decomposition Tree visual to break down Total Orders across hierarchical dimensions:
       - Category Name → Subcategory Name → Product Name
- 🧠 AI Splitting & Manual Exploration
   - Allows both AI-driven and manual drill-down to identify segments with the highest or lowest impact on total orders.
   - Empowers users to spot trends, outliers, and performance drivers interactively.
- 📌 Contextual Card Display
   - Dynamic Total Orders Card updates based on the selected branch of the decomposition tree.
   - Ensures quick insight into the current selection's impact.
- 🚀 Business Value
   - Supports deep-dive diagnostics and data storytelling for order performance.
   - Ideal for identifying underperforming products or top-selling categories quickly.
- 🔁 Smooth Page Navigation
   - Reset Filters – Clears applied filters instantly
   - Interactive buttons improve overall user experience
<p align="center">
  <img width="600" height="300" alt="Screenshot 2025-07-27 202955" src="https://github.com/user-attachments/assets/ce053700-f3ef-4295-8cec-549fa06b90d3" />
</p>

### 6. Key Influencers:
- 🧠 AI-Powered Insight Generation - Leveraged Key Influencers Visual in Power BI to uncover patterns and drivers behind key metrics.
- 🔍 1. Home Ownership Analysis
  - Analyzed the likelihood of a customer being a homeowner, explained by:
    - Education Level
    - Occupation
    - Annual Income
    - Parental Status
    - Marital Status
  - Identifies top combinations of attributes that positively or negatively influence home ownership.
- 📈 2. Average Retail Price Drivers
   - Investigated what factors drive Average Retail Price, explained by:
      - Sum of Product Cost and expanded the explanation by Subcategory Name
      - Helps identify which product categories tend to have higher markups.
- 🎯 Business Value - Enables data-backed decision-making by highlighting hidden patterns in customer behavior and product pricing.
- 🔁 Smooth Page Navigation
  - Navigation Button included for seamless interaction
  - Reset button helps revert back to original influencer view
  <p align="center">
  <img width="600" height="300" alt="Screenshot 2025-07-27 203023" src="https://github.com/user-attachments/assets/ff37ed45-d165-4f16-94a4-5ecc38468150" />
  </p>

### 7. Category Tooltip: 
A dedicated tooltip page designed to enrich the user experience with on-hover insights for each product category.
- 📊 Area Chart – Displays Weekly Orders Trend for the selected category, helping identify short-term patterns or spikes.
- 🧾 Multi-row Card – Presents quick-glance KPIs:
     - Total Orders
     - Total Profit
     - Total Revenue
     - Total Returns
     - Return Rate (%)
- 🎯 Purpose:
   - Provides instant context while hovering over visual elements on bars in "Orders by Category".
   - Enables data-driven decision-making without navigating to another page.
   - Enhances the interactivity and user-friendliness of the report.
<p align="center">
  <img width="358" height="233" alt="Screenshot 2025-07-27 203052" src="https://github.com/user-attachments/assets/cd29d7ca-5f53-4583-94da-9226f11b1a94" />
</p>

# Pages Included:
| **Page Name**                | **Purpose**                                                                                                                                                                           |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Performance Overview**  | Highlights overall KPIs with SVG visuals, monthly revenue trends, top products, and benchmarking. Hidden slicers (Year & Continent) and Reset Filter button using bookmarks included. |
| **2. Product Details**       | Drillthrough page from top products matrix. Contains dynamic KPIs, target-based gauges, metric selector, price adjustment simulation, and area chart with time granularity controls.  |
| **3. Customer Detail**       | Deep dive into customer insights via metrics like orders, revenue, and segmentation by income & occupation. Interactive top customer card, trend lines, and smart insight buttons.    |
| **4. Map**                   | Grayscale bubble map visualizing sales per country. Continent-based filter tiles (Europe, NA, Pacific), global reset functionality, and smooth navigation.                            |
| **5. Decomposition Tree**    | AI-driven + manual breakdown of Total Orders by Category, Subcategory, and Product. Contextual card updates dynamically based on selection. Reset filters and navigation included.    |
| **6. Key Influencers**       | AI visual to explain drivers for Home Ownership and Average Retail Price. Interactive explanation fields and reset/navigation buttons for smooth UX.                                  |
| **7. Category Tooltip Page** | Tooltip page enhancing the bar chart in Page 1. Area chart (Weekly Orders) and multi-row card display Total Orders, Revenue, Profit, Returns, and Return Rate on hover.               |
# Tools & Technologies Used:
- 💻 Power BI
   - Data Modeling - Structured relationships, star schema setup using AdventureWorks DW dataset.
   - DAX Measures - Created custom KPIs (Revenue, Profit, Returns, Return Rate, Weekly Orders, etc.), metric selectors, and target-based measures.
   - Bookmarks & Buttons - Reset Filter functionality applied across first 5 pages using hidden slicers and bookmark logic.
   - Navigation buttons for seamless page switching and storytelling flow.
- AI Visuals
   - Key Influencers for identifying drivers of Home Ownership and Average Retail Price.
   - Decomposition Tree to break down Total Orders dynamically by category hierarchy.
- Tooltip Page - Category-level tooltip page designed to appear on hover, using area charts and multi-row cards for deeper insights.
- SVG & Conditional Formatting
   - SVG icons integrated into KPIs for enhanced visuals.
   - Dynamic formatting applied to visuals for emphasis based on thresholds.
- Interactive Elements
   - Drillthrough pages (Product Details).
   - Slicer buttons (Continent, Year) for interactivity and intuitive UX.
- 📊 Dataset -
   - AdventureWorks DW Dataset - Microsoft’s sample data warehouse containing sales, product, and customer dimensions.
- 🧰 Additional Tools - GitHub -Project hosted for version control and portfolio showcasing.
### Key Insights Uncovered:
- 🌍 Geographic Insights - Europe generated the highest total sales, making it the top-performing continent by revenue.
- 👥 Customer Insights
   - The top customer by revenue is Mr. Maurice Shah.
   - Among customers in skilled manual occupations in 2022, Ruban Suarez drove the highest revenue at $4,683.
- 🛒Product Performance Insights
  - The most ordered product subcategory is Tires and Tubes, indicating high demand and consistent turnover.
  - The most returned product is Shorts, which may indicate quality concerns, size mismatches, or customer dissatisfaction.
  - Mountain Bikes have the highest average retail price at $1,637, positioning them as the most premium product line in the catalog.  
## 🛠️ How to View This Power BI Dashboard

GitHub does not support direct preview of `.pbix` (Power BI) files. To explore this dashboard:

### 📥 Steps to Download and Open:

1. Click on **`AdventureWorks Project Dashboard.pbix`** in this repository.
2. Then click **“View Raw”**  to save the file locally.
3. Open the file using **Power BI Desktop** on your Windows system.



