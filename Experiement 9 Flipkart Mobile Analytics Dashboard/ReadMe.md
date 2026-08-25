# 📱 Flipkart Mobile Analytics Dashboard (Power BI)

## 📌 Project Overview

This project presents an interactive **Flipkart Mobile Analytics Dashboard** built using Microsoft Power BI based on the **Flipkart Mobiles Dataset**. The dashboard helps management monitor product pricing, discounting behaviour, customer ratings, brand performance, price categories, and storage configurations across the mobile-phone catalog.

This project was developed as part of the **Data Analytics for Business - Experiment 9** at Alliance University.

---

## 🎯 Objective

The objective of this dashboard is to:

* Monitor total mobile products, brands, and models
* Track average selling price and average customer rating
* Compare selling prices across mobile brands
* Compare original price and selling price by brand
* Analyze discounting behaviour across brands
* Analyze product rating distribution
* Analyze products across different price categories
* Analyze storage-capacity distribution
* Compare mobile products across memory and storage configurations
* Support data-driven pricing and inventory decisions

---

## 🛠️ Tools & Technologies

* Microsoft Power BI Desktop
* Microsoft Excel / CSV
* Power Query
* DAX (Data Analysis Expressions)

---

## 📂 Dataset

**Dataset Name:** Flipkart Mobiles Dataset

**Source:** Flipkart Mobile Product Dataset

The dataset contains mobile-product information used to analyze:

* Brand
* Model
* Color
* Memory
* Storage
* Rating
* Selling Price
* Original Price

## The dataset was imported into Power BI using Power Query with **UTF-8 encoding** and a **comma delimiter**. Duplicate product listings were removed and missing rating values were replaced with `0`.

# 📈 Dashboard Features

## KPI Cards

* Total Products
* Total Brands
* Total Models
* Average Selling Price
* Average Rating

## Interactive Filters

* Brand
* Price Category
* Memory
* Storage
* Rating Category

## Visualizations

### Average Selling Price by Brand

Compares the average selling price of mobile products across different brands using a bar chart.

### Original Price vs Selling Price by Brand

Compares average original price and average selling price across brands using a combo chart.

### Product Rating Distribution

Shows the distribution of products across different customer-rating categories using a donut chart.

### Average Discount % by Brand

Compares the average discount percentage offered by different mobile brands.

### Products by Price Category

Analyzes the distribution of products across:

* Budget (< ₹15K)
* Mid-Range
* High-End
* Premium

### Storage Distribution

Analyzes product distribution across different storage capacities, including:

* 32GB
* 64GB
* 128GB
* 256GB
* 512GB
* 1TB

The dashboard combines KPI cards, charts, and interactive slicers into a single analytical view.

---

# 📊 Key Insights

## Overall Performance

* **Total Products:** 3,006
* **Total Brands:** 17
* **Total Models:** 888
* **Average Selling Price:** ₹25,842
* **Average Rating:** 4.05

The catalog contains a large variety of mobile products across multiple brands and price segments.

## Major Findings

* Apple has the highest average selling price at approximately **₹86K**, placing it clearly in the premium segment.
* Google Pixel follows Apple at approximately **₹61K** average selling price.
* Samsung, vivo, and ASUS are positioned around the ₹20K–₹24K range.
* POCO and Motorola show the highest average discount percentages.
* Budget phones below ₹15K form the largest price category with approximately **1.5K products**.
* **64GB and 128GB** are the dominant storage configurations.
* Products rated **Very Good (4–4.5)** represent the largest rating category.
* The overall product catalog maintains a healthy average rating of **4.05**.

---

# 📐 DAX Measures Used

## Average Selling Price

```DAX
Average Selling Price =
AVERAGE(Flipkart_Mobiles[Selling Price])
```

Calculates the average selling price across the mobile-product catalog.

## Average Original Price

```DAX
Average Original Price =
AVERAGE(Flipkart_Mobiles[Original Price])
```

Calculates the average original/MRP price and is used in the Original Price vs Selling Price comparison.

## Average Rating

```DAX
Average Rating =
AVERAGE(Flipkart_Mobiles[Rating])
```

Calculates the average customer rating across products.

These DAX measures are used to power the dashboard's KPI cards and visualizations.

---

# 🏷️ Calculated Columns Used

## Rating Category

Products are grouped into five rating categories:

* Excellent (4.5–5)
* Very Good (4–4.5)
* Good (3–4)
* Average (2–3)
* Poor (1–2)

The column is used for the Product Rating Distribution donut chart and Rating Category slicer.

## Rating Category Sort

A numeric sorting column was created to ensure that rating categories appear in the correct order:

**Excellent → Very Good → Good → Average → Poor**

instead of alphabetical order.

## Storage Sort

A numeric sorting column was created to correctly arrange storage capacities:

**32GB → 64GB → 128GB → 256GB → 512GB → 1TB**

This ensures the Storage Distribution chart follows capacity order rather than alphabetical order.

---

# 📊 Dashboard Analysis

## Average Selling Price by Brand

The dashboard compares average selling prices across brands.

Apple has the highest average selling price at approximately **₹86K**, followed by Google Pixel at approximately **₹61K**. Samsung, vivo, and ASUS are positioned around the ₹20K–₹24K range.

---

## Original Price vs Selling Price by Brand

This visualization compares the average original price with the average selling price for each brand.

Apple has the highest original price at approximately **₹89K** and selling price at approximately **₹62K**, creating the largest absolute price gap among the brands.

---

## Product Rating Distribution

The rating distribution shows:

* **Very Good (4–4.5): 65.3%**
* **Excellent (4.5–5): 17.2%**
* **Good (3–4): 12.9%**
* Average and Poor ratings represent smaller portions.

This indicates generally strong customer-rated quality across the mobile catalog.

---

## Average Discount % by Brand

POCO leads the average discount percentage at approximately **14.35%**, followed by Motorola at approximately **12.54%**.

Infinix and realme show comparatively lower discount percentages.

---

## Products by Price Category

The Budget category below ₹15K contains the highest number of products at approximately **1.5K products**.

It is followed by:

* Mid-Range
* High-End
* Premium

This indicates that the mobile catalog has a strong concentration in the budget segment.

---

## Storage Distribution

The dominant storage configurations are:

* **64GB — 754 products**
* **128GB — 752 products**
* **32GB — 550 products**

Higher-capacity configurations such as 256GB, 512GB, and 1TB form a relatively small portion of the catalog.

---

# 🔎 Filtered Dashboard Analysis

## Brand = Apple

When Apple is selected:

* Total Products: **324**
* Total Brands: **1**
* Total Models: **24**
* Average Selling Price: **₹85,963**
* Average Rating: **3.83**

Apple has a strong premium positioning, with storage concentrated around 128GB and 256GB.

---

## Price Category = Budget (< ₹15K)

When the Budget category is selected:

* Total Products: **1,526**
* Total Brands: **15**
* Total Models: **560**
* Average Selling Price: **₹9,452**
* Average Rating: **4.03**

POCO and Motorola continue to show relatively high discounting within the budget segment.

---

## Rating Category = Very Good (4–4.5)

When the Very Good rating category is selected:

* Total Products: **1,964**
* Total Brands: **17**
* Total Models: **619**
* Average Selling Price: **₹18,082**
* Average Rating: **4.25**

The Very Good category is broadly distributed across brands, price points, and storage tiers.

---

# 💼 Business Benefits

* Helps monitor mobile-product pricing
* Supports brand-wise price comparison
* Enables discounting analysis
* Helps evaluate product quality through ratings
* Supports price-segment analysis
* Helps identify dominant storage configurations
* Enables interactive brand and product analysis
* Supports inventory planning
* Helps identify price-to-rating opportunities
* Supports data-driven pricing and business decisions

---

# 📚 Learning Outcomes

* Data Cleaning using Power Query
* Data Import and Transformation
* Data Modeling in Power BI
* Creating DAX Measures
* Creating Calculated Columns
* KPI Development
* Product Analytics
* Pricing Analytics
* Discount Analysis
* Customer Rating Analysis
* Interactive Dashboard Design
* Data Visualization
* Business Intelligence Reporting

---

# 📁 Repository Structure

```text
Flipkart-Mobile-Analytics-Dashboard/
│
├── Dataset/
│   └── Flipkart_Mobiles.csv
│
├── Dashboard/
│   └── Flipkart Mobile Analytics Dashboard.pbix
│
├── Report/
│   └── Experiment_9_Flipkart_Mobile_Analytics_Dashboard.docx
│
└── README.md
```

---

# 🔗 GitHub Repository

[Flipkart Mobile Analytics Dashboard — GitHub Repository](https://github.com/Priyanshnolkha/Data-Analytics-For-Business-Projects/tree/main/Experiement%209%20Flipkart%20Mobile%20Analytics%20Dashboard)

---

# 👨‍💻 Author

**Priyansh Nolkha**

Master of Computer Applications (MCA)
Alliance University, Bengaluru


---

# ✅ Conclusion

The Flipkart Mobile Analytics Dashboard provides an interactive business intelligence solution for analyzing mobile-product pricing, discounting, ratings, brands, price categories, and storage configurations.

The dashboard combines **Power Query, DAX, KPI cards, interactive slicers, bar charts, column charts, a combo chart, and a donut chart** to transform the Flipkart mobile dataset into actionable business insights.

The analysis supports **pricing strategy, discount evaluation, product quality monitoring, and inventory-planning decisions** across the Flipkart mobile portfolio.

