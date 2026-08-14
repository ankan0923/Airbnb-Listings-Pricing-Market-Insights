🏠 Airbnb Listings — Pricing & Market Insights
Python Pandas Power BI Jupyter Status

Analyzing Pricing, Room Types, Neighbourhoods, Reviews, Availability & Host Behaviour

📌 Project Overview
This is an end-to-end Data Analyst portfolio project based on Airbnb listing data.

The project transforms raw Airbnb data into actionable insights using Python, Pandas, statistical analysis, visualization, Power BI, and DAX.

Workflow:

Data Cleaning → Data Transformation → EDA → Visualization → Power BI Dashboard → Business Insights → Recommendations

🎯 Business Objectives
Identify the distribution of Airbnb listings across neighbourhoods.
Understand which room types dominate the market.
Analyze average and median listing prices.
Understand the Airbnb price distribution.
Compare pricing across room types and neighbourhoods.
Explore the relationship between price and reviews.
Analyze availability by room type.
Understand review activity.
Segment hosts by portfolio size.
Identify pricing and availability opportunities.
🔄 Project Workflow
Raw Airbnb Dataset
        ↓
Data Quality Assessment
        ↓
Missing Value Analysis
        ↓
Duplicate Detection & Removal
        ↓
Outlier Detection & Treatment
        ↓
Data Type Conversion
        ↓
Feature Engineering
        ↓
Exploratory Data Analysis
        ↓
Python Visualizations
        ↓
Power BI Dashboard
        ↓
Business Insights
        ↓
Recommendations
🧹 Data Cleaning
The dataset was prepared through:

Missing-value analysis and treatment
Duplicate detection and removal
Numerical data validation
Outlier detection using descriptive statistics, boxplots and IQR
Business-rule validation
Data type conversion
Final data-quality checks
Important numerical fields included:

price, minimum_nights, number_of_reviews, reviews_per_month, calculated_host_listings_count, availability_365, and number_of_reviews_ltm.

Note: Extreme values were investigated before treatment because expensive or highly reviewed Airbnb listings may be genuine observations.

⚙️ Feature Engineering
Business-oriented features were created:

Feature	Purpose
price_category	Groups listings into Budget, Standard, Premium and Luxury
availability_rate	Converts annual availability into a percentage
review_activity	Segments listings by review activity
host_type	Segments hosts by portfolio size
stay_category	Groups listings by minimum-stay requirement
📊 Power BI Dashboard
The final report contains two pages.

📄 Page 1 — Airbnb Listings Analysis Dashboard
KPI Cards
KPI	Final Dashboard Value
Total Listings	490
Total Neighbourhoods	15
Median Price	149.00
Average Price	174.95
Average Reviews	59.28
Average Minimum Stay	6.83
Average Availability	242.89 days
Visuals
Listings by Neighbourhood
Room Type Mix
Listings by Price
Listings by Room Type
Price vs Number of Reviews
Story
The Airbnb inventory is heavily concentrated in Entire home/apartment listings. The median price of 149 is below the average price of 174.95, indicating that higher-priced listings pull the average upward. Most listings are concentrated in lower-to-mid price ranges, with a smaller premium-price tail.

📄 Page 2 — Pricing & Host Analysis
Visuals
Average Availability by Room Type
Listings by Review Activity
Average Price by Last Review Month & Room Type
Average Price by Neighbourhood
Listings by Host Type
Median Price by Room Type
Detailed Listing Table
Story
The second page provides deeper analysis of pricing, availability, reviews and host behaviour. Neighbourhood-level pricing highlights areas with higher pricing levels, while host segmentation shows the distribution between single-property and multi-property hosts.

Room types with very small sample sizes should be interpreted carefully. For example, a median price based on only one Shared Room listing is not representative of the wider market.

🧮 DAX Measures
Total Listings
Total Listings =
DISTINCTCOUNT(listings[id])
Average Price
Average Price =
AVERAGE(listings[price])
Median Price
Median Price =
MEDIAN(listings[price])
Average Reviews
Average Reviews =
AVERAGE(listings[number_of_reviews])
Average Minimum Stay
Average Minimum Stay =
AVERAGE(listings[minimum_nights])
Average Availability
Average Availability =
AVERAGE(listings[availability_365])
Total Neighbourhoods
Total Neighbourhoods =
DISTINCTCOUNT(listings[neighbourhood])
💡 Key Business Insights
🏠 1. Room Type Concentration
Entire home/apartment listings dominate the inventory, representing approximately 83% of the listings shown in the final dashboard.

📍 2. Neighbourhood Concentration
Sixth Ward has the highest number of listings among the analysed neighbourhoods, showing strong inventory concentration.

💰 3. Average vs Median Price
The median price is 149, compared with an average price of 174.95. This suggests that high-priced listings are influencing the average.

📊 4. Price Distribution
Most listings are concentrated in lower-to-mid price ranges, while a smaller number of premium listings create a long upper tail.

⭐ 5. Reviews & Price
Review activity is concentrated among a subset of listings. The price-versus-review relationship is not simply linear, suggesting that price alone does not determine review performance.

📅 6. Availability
Availability differs by room type. High availability should be considered alongside pricing, demand, reviews and seasonality.

👤 7. Host Segmentation
The dataset contains single-property, small, medium and large hosts, indicating different host operating models.

⚠️ 8. Small-Sample Warning
Some room types have very few listings. Their price statistics should therefore not be interpreted as representative market prices.

📌 Business Recommendations
1. Neighbourhood-Level Pricing
Benchmark prices against similar listings in the same neighbourhood and room type.

2. Use Median Alongside Average
Monitor both median and average price because extreme listings can distort the average.

3. Optimize High-Availability Listings
Investigate listings with high availability for pricing competitiveness, demand, visibility, seasonality, promotions and minimum-stay restrictions.

4. Segment Pricing by Room Type
Use different pricing strategies for entire homes, private rooms, hotel rooms and shared rooms.

5. Investigate Premium Neighbourhoods
High-price neighbourhoods may offer premium opportunities, but hosts should also evaluate competition, reviews, availability and room type.

6. Improve Review Performance
Low-review listings can be investigated for opportunities involving guest experience, listing quality, pricing and property presentation.

🛠️ Tools & Technologies
Tool	Purpose
Python	Data cleaning and analysis
Pandas	Data manipulation
NumPy	Numerical analysis
Matplotlib	Visualization
Seaborn	Statistical visualization
Jupyter Notebook	Analytical workflow
Power BI	Dashboard and reporting
DAX	KPI calculations
GitHub	Portfolio and version control
📂 Repository Structure
airbnb-listings-analysis/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── README.md
│   └── airbnb_cleaned.csv
│
├── notebooks/
│   └── airbnb_data_cleaning_eda.ipynb
│
├── powerbi/
│   ├── README.md
│   └── Airbnb_Analysis_Dashboard.pbix
│
├── reports/
│   └── business_insights.md
│
└── images/
    ├── dashboard_overview.png
    └── pricing_host_analysis.png
🚀 How to Run
1. Clone the repository
git clone https://github.com/YOUR_USERNAME/airbnb-listings-analysis.git
cd airbnb-listings-analysis
2. Install dependencies
pip install -r requirements.txt
3. Run the notebook
jupyter notebook
Open:

notebooks/airbnb_data_cleaning_eda.ipynb
4. Open the Power BI dashboard
Open:

powerbi/Airbnb_Analysis_Dashboard.pbix
using Power BI Desktop.

📋 Project Deliverables
✅ Data quality assessment
✅ Missing-value analysis
✅ Duplicate detection and removal
✅ Outlier detection and treatment
✅ Data type conversion
✅ Feature engineering
✅ Exploratory Data Analysis
✅ Python visualizations
✅ Power BI Executive Dashboard
✅ Pricing & Host Analysis page
✅ DAX KPI measures
✅ Business insights
✅ Business recommendations
✅ GitHub documentation
🎓 Skills Demonstrated
Data Analytics: Data Cleaning • Data Wrangling • EDA • Statistical Analysis • Outlier Analysis • Feature Engineering

Python: Pandas • NumPy • Matplotlib • Seaborn • Jupyter Notebook

Power BI: Dashboard Design • KPI Cards • Slicers • DAX • Interactive Visualizations • Data Storytelling

Business Intelligence: Pricing Analysis • Market Segmentation • Neighbourhood Analysis • Host Analysis • Availability Analysis • Review Analysis

🏆 Project Outcome
This project demonstrates how raw Airbnb data can be transformed into reliable business intelligence:

Raw Data → Clean Data → Analysis → Dashboard → Insights → Business Recommendations

The final dashboard helps stakeholders understand listing concentration, pricing patterns, room-type mix, neighbourhood differences, review activity, availability and host behaviour.

👤 Author
Ankan Chowdhury
Aspiring Data Analyst

Core Skills: SQL • Power BI • Python • Excel • Tableau

Focus Areas: Data Cleaning • Dashboarding • Business Trends • Customer Analysis
