📊 Marketing Campaign Dashboard (Power BI)

📌 Project Overview

This project presents an interactive Marketing Campaign Dashboard built using Microsoft Power BI based on the Marketing Campaign Performance Dataset. The dashboard helps management monitor campaign reach, conversion performance, acquisition cost, and return on investment across channels, audiences, and customer segments.

This project was developed as part of the Data Analytics for Business - Experiment 8 at Alliance University.

🎯 Objective

The objective of this dashboard is to:

Monitor total marketing campaigns and clicks

Track average conversion rate and ROI

Compare acquisition cost and ROI across campaign types

Analyze campaign distribution across customer segments

Compare campaigns across target audiences

Evaluate average ROI by marketing channel

Analyze monthly conversion-rate trends

Support data-driven marketing planning and decision-making

🛠️ Tools & Technologies

Microsoft Power BI Desktop

Microsoft Excel / CSV

Power Query

DAX (Data Analysis Expressions)

📂 Dataset

Dataset Name: Marketing Campaign Performance Dataset

Source: Academic Dataset for Marketing Campaign Analysis

The dataset contains campaign information used to analyze:

Campaign ID

Campaign Type

Channel Used

Customer Segment

Target Audience

Location

Clicks

Conversion Rate

ROI

Acquisition Cost

Date

📈 Dashboard Features

KPI Cards

Total Campaigns

Avg Conversion Rate

Total Clicks

Avg ROI

Interactive Filters

Location

Campaign Type

Visualizations

Acquisition Cost & ROI by Campaign Type — Combo Chart

Campaigns by Customer Segment — Donut Chart

Campaigns by Target Audience — Bar Chart

Average ROI by Channel — Bar Chart

Monthly Conversion Rate — Line Chart

📊 Key Insights

Overall Performance

Total Campaigns: 200K

Avg Conversion Rate: 8.01%

Total Clicks: 110M

Avg ROI: 5.00

Major Findings

Acquisition cost is distributed almost equally across the five campaign types.

Customer segments are evenly represented across the campaign portfolio.

Target audiences are also evenly distributed at approximately 40K campaigns per group.

Average ROI is approximately 5.0 across Facebook, Website, Google Ads, and Email.

Monthly conversion rate remains close to 8% throughout the year.

Facebook campaigns show a slightly higher ROI of 5.02 when the channel is selected.

October shows a slightly lower conversion rate of 7.98%, while Avg ROI increases to 5.02.

📐 DAX Measures Used

Total Campaigns

Total Campaigns =
DISTINCTCOUNT('marketing_campaign_dataset'[Campaign_ID])

Avg Conversion Rate

Avg Conversion Rate =
AVERAGE('marketing_campaign_dataset'[Conversion_Rate])

Total Acquisition Cost

Total Acquisition Cost =
SUM(marketing_campaign_dataset[Acquisition_Cost])

DateTable

DateTable =
CALENDAR(
    MIN(marketing_campaign_dataset[Date]),
    MAX(marketing_campaign_dataset[Date])
)

The DateTable supports monthly conversion-rate analysis and time-based filtering.

📊 Dashboard Analysis

Acquisition Cost & ROI by Campaign Type

Compares acquisition cost and ROI across:

Influencer

Search

Display

Social Media

Email

Campaigns by Customer Segment

Analyzes campaign distribution across:

Foodies

Tech Enthusiasts

Outdoor Adventurers

Health & Wellness

Fashionistas

Campaigns by Target Audience

Analyzes campaign distribution across:

Men 18–24

Men 25–34

All Ages

Women 25–34

Women 35–44

Average ROI by Channel

Compares average ROI across:

Facebook

Website

Google Ads

Email

Monthly Conversion Rate

Tracks conversion-rate performance from January to December and helps identify monthly trends.

💼 Business Benefits

Helps monitor marketing campaign performance

Supports ROI and conversion-rate analysis

Enables comparison of campaign types and channels

Helps identify customer and audience distribution

Supports marketing budget allocation

Enables interactive campaign analysis

Supports data-driven marketing decisions

📚 Learning Outcomes

Data Cleaning using Power Query

Data Modeling in Power BI

Creating DAX Measures

KPI Development

Marketing Analytics

Campaign Performance Analysis

Interactive Dashboard Design

Data Visualization

Business Intelligence Reporting

📁 Repository Structure

Marketing-Campaign-Dashboard/
│
├── Dataset/
│   └── Marketing_Campaign_Dataset.xlsx
│
├── Dashboard/
│   └── Marketing Campaign Dashboard.pbix
│
├── Report/
│   └── Experiment_8_Report.pdf
│
└── README.md


👨‍💻 Author

Priyansh Nolkha

Master of Computer Applications (MCA)
Alliance University
