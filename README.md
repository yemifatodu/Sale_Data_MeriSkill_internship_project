# **Sale_Data_MeriSkill_Internship_Project**

## **Project Objective**

The main goal of this project is to conduct a comprehensive analysis of sales data for the year 2019. The objective is to identify key trends, performance metrics, and insights that can inform strategic decision-making for future sales strategies, marketing efforts, and resource allocation. This project is part of the Meri Skill Internship and is stored in this GitHub repository to showcase the findings and analysis.

## **Project Context**

- **Dataset Origin:** The dataset used for this project was provided by Meri Skill as part of the Meri Skill Internship program. It serves as the foundation for analyzing sales performance in 2019.

- **Data Size:** The dataset contains detailed records of sales transactions for the year 2019, including information on sales amounts, quantities, timestamps, product categories, and geographic locations. This allows for a thorough analysis of sales trends and performance metrics.

- **Business Problem:** The core business problem addressed by this project is understanding sales performance in 2019 across various dimensions, such as time (monthly, hourly), product categories, and geographic locations. The goal is to identify high-performing periods, products, and regions, and to uncover any potential areas for improvement. The analysis provides actionable insights to enhance future sales strategies, optimize inventory management, and better align marketing efforts with consumer demand.

---

## **Data Analyst Experience and Project Insights**

As a data analyst for the Meri Skill Internship project, I applied several key skills to analyze the sales dataset for 2019. These skills were instrumental in deriving meaningful insights and recommendations from the data. Here’s how each skill contributed to the findings and insights:

### **1. Data Cleaning**

**Experience:**  
I meticulously cleaned the dataset using Microsoft Excel, addressing missing values, handling outliers, and ensuring data consistency.

**Relating to Findings:**
- **Accuracy of Insights:** By resolving inconsistencies and missing values, I ensured that the analysis was accurate and reliable. This cleaning process was crucial in identifying true sales trends without the distortion of erroneous entries.
- **Outlier Detection:** Handling outliers allowed for a precise analysis of sales performance. This was essential in identifying genuine high or low-performing periods and products, leading to actionable insights on where to focus marketing efforts or adjust inventory.

### **2. Exploratory Data Analysis (EDA)**

**Experience:**  
I conducted thorough exploratory analysis to understand the dataset, exploring distributions, correlations, and patterns.

**Relating to Findings:**
- **Trend Identification:** EDA helped identify key trends, such as peak sales months and high-performing products. For example, recognizing December as a top sales month highlighted the importance of holiday promotions.
- **Pattern Detection:** Exploring patterns revealed significant insights, such as peak sales hours and regional performance differences. These insights were crucial for tailoring sales strategies and optimizing operations based on time-of-day and location-specific trends.

### **3. Data Cleaning and Transformation Details**

**Column Name Changes:**
- Original column names were updated for clarity and consistency. For example, `column_1` was dropped and `column_7` was changed to represent months more clearly.

**Conversion of `order_date` to Date and Time Components:**

- **Date Component Extraction:** Converted `order_date` to contain only the date part for daily analysis.
- **Time Component Extraction:** Extracted the time part from `order_date` for hourly analysis.

**SQL Queries Used:**

- **Extract Date Only from `order_date`:**
  ```sql
  SELECT
    order_date,
    CAST(order_date AS DATE) AS order_date_only
  FROM
    sales_data;
  ```
  This query extracts the date component from `order_date`, allowing analysis based on the date alone.

- **Extract Time Only from `order_date`:**
  ```sql
  SELECT
    order_date,
    CAST(order_date AS TIME) AS order_time_only
  FROM
    sales_data;
  ```
  This query extracts the time component from `order_date`, enabling analysis based on the time of day.

### **4. Visual Analysis**

**Experience:**  
Utilizing Tableau, I performed visual analysis to detect patterns and trends through its advanced visualization capabilities.

**Relating to Findings:**
- **Visualization of Trends:** Tableau's visualizations made it easier to identify trends and anomalies, such as peak sales hours and high-performing product categories. Visual tools provided a clear representation of data, simplifying the understanding and communication of key findings.
- **Decision-Making Support:** Presenting data in a visual format allowed for intuitive insights. For instance, visualizing sales performance by city highlighted key markets and revenue generators, guiding strategic decisions on where to focus future marketing and sales efforts.

### **5. SQL Queries**

     Date Extraction: Employed SQL queries to extract date and time components for detailed analysis.
    Data Aggregation: Used SQL to aggregate sales data by various dimensions, such as month, product category, and region.
    By applying these methods, I was able to uncover key insights and provide actionable recommendations for improving sales strategies and 
    optimizing operations.
--- 

### Analysis of the Sales Dashboard Chart (2019)

1. **Sales Trend Over Time (Top Left Chart)**:
   - The chart shows the sales trend over the months of 2019. Sales fluctuate throughout the year, with a noticeable peak towards the end of the year, indicating a strong sales performance during that period.

2. **Total Sales & Sales Quantity (Top Right Section)**:
   - The dashboard highlights total sales of $34,492,036.00 million and a sales quantity of 209,079.00 thousand units. This provides a summary of the sales performance for the year.

3. **Hourly Sales Distribution (Middle Right Chart)**:
   - This chart shows how sales vary by the hour. Sales seem to be higher during specific hours of the day, particularly in the late morning and early evening.

4. **Top 10 Selling Products (Bottom Left Charts)**:
   - Two charts illustrate the top 10 selling products based on quantity and sales. AAA and AA Batteries (4-pack) lead in quantity sold, while higher-priced items like the 27in 4K Gaming Monitor and Apple AirPods Headphones dominate in terms of sales revenue.

5. **Quantity Ordered by City (Middle Chart)**:
   - This bar chart shows the quantity of products ordered by different cities. Some cities have significantly higher order volumes, indicating strong regional demand.

6. **Sales by City (Middle Right Map)**:
   - The map displays sales distribution across different cities in the United States, with larger circles representing higher sales volumes. This gives a geographical perspective on sales performance.

7. **Sales Correlation Analysis (Bottom Middle Chart)**:
   - This matrix chart seems to explore the correlation between different products. Products with stronger correlations are grouped together, potentially indicating complementary purchase patterns.

8. **Trend of Year Quantity Distribution (Bottom Right Chart)**:
   - This bar chart shows the quantity of orders distributed across the months. There is a steady increase in the quantity ordered as the year progresses, peaking in December.

### Detailed Description of the Color Scheme

1. **Background and Borders**:
   - The entire dashboard is set against a bright green background, with dark blue borders outlining each section and chart. The contrast between the green background and blue borders makes the content stand out prominently.

2. **Text and Labels**:
   - The text within the charts is primarily white or black, which contrasts well with the bright green background, ensuring that all labels and figures are easily readable.

3. **Charts and Graphs**:
   - Most of the data points and lines within the charts are depicted in red. This strong color choice draws immediate attention to the trends and key data points, making it easy to identify patterns at a glance.

4. **Bar Charts**:
   - The bar charts use a gradient of colors for different products and cities, ranging from red to orange, to differentiate between different categories. The use of warm colors (red, orange, yellow) adds to the visual impact of the dashboard, highlighting significant data points.

5. **Map Visualization**:
   - The map is rendered in light gray with green circles of varying sizes to represent sales volume by city. The green circles match the overall color scheme, maintaining a consistent visual theme throughout the dashboard.

6. **Data Highlights**:
   - Important figures like total sales and sales quantity are displayed in white text against a green background. This color combination makes these key metrics stand out as the most prominent information on the dashboard.

In summary, the dashboard uses a bright and contrasting color scheme to make key data points and trends easily distinguishable, with a focus on red for highlighting and green as a thematic background color.

---

## **Sales Trend Analysis**

### **Top Sales Months**
- **December** emerged as the highest-performing month with substantial sales of $4,613,443.32 and a total of 28,114 units sold. This peak suggests a strong end-of-year performance, possibly due to holiday shopping.
- **October** followed with $3,736,726.86 in sales and 22,703 units sold, indicating a strong performance driven by factors such as promotions or seasonal demand.
- **April** also performed well with $3,390,670.22 in sales and 20,558 units sold, possibly due to spring promotions or product launches.

### **Bottom Sales Months**
- **January** recorded the lowest sales of $1,822,256.72 with 10,903 units sold, likely due to post-holiday seasonality effects.
- **September** and **February** also had relatively low sales figures, indicating potential seasonal declines or the need for targeted marketing efforts.

## ** Total Sales & Sales Quantity**

- **Total Sales** for 2019 amounted to $34,492,035.80, reflecting overall revenue performance.
- **Total Quantity Sold** reached 209,079 units, providing insight into the volume of products moved throughout the year.

### ** Hourly Sales Distribution**

Analyzing sales by hour reveals significant trends:
- **Peak Sales Hours**: The highest sales were recorded between 18:00 and 20:00, with the peak at 19:00 generating $2,412,938.53. This suggests that late afternoon to evening is a crucial time for maximizing sales.
- **Lowest Sales Hours**: Sales were lowest between 2:00 and 4:00, indicating a need to optimize strategies during these off-peak hours.

### ** Top Selling Products**

#### **By Quantity**
- **AAA Batteries (4-pack)**: The most purchased product with 31,017 units sold, highlighting its popularity.
- **AA Batteries (4-pack)** and **USB-C Charging Cable** also saw high sales volumes, indicating strong customer preference for these items.

#### **By Sales Value**
- **Macbook Pro Laptop** was the top-selling product by revenue, generating $8,037,600, reflecting high value and strong demand.
- **iPhone** and **ThinkPad Laptop** followed, emphasizing their significance in the product lineup.

### ** Sales by City**

#### **Top Cities by Quantity Ordered**
- **San Francisco** led with 50,239 units, demonstrating its role as a major market.
- **Los Angeles** and **New York City** also had high quantities ordered, indicating their importance in the sales strategy.

#### **Top Cities by Sales Revenue**
- **San Francisco** generated the highest revenue at $8,262,203.87, followed by **Los Angeles** and **New York City**, which are critical markets for revenue generation.

### ** Monthly Quantity Distribution**

The trend in quantity ordered over the year shows a clear pattern:
- **Highest Quantity**: December with 28,114 units.
- **Lowest Quantity**: January with 10,903 units.

This trend suggests strong seasonal fluctuations and highlights the need for strategic planning to address low-sales periods.

### ** Top Sales Hours by City**

#### **Top Performing Hours**
- **San Francisco**: Highest sales were at 19:00, reflecting peak purchasing times in this city.
- **Los Angeles** and **New York City** also showed strong performance in the late evening hours.

#### **Lowest Performing Hours**
- Sales were notably low in the early morning hours across various cities, suggesting potential for targeted marketing or promotional activities to boost sales during these times.

### ** Average Order Value (AOV)**
- **Average Order Value**: $185.49. This metric provides insight into customer spending behavior and can guide pricing and promotional strategies.

### ** Top 10 Customers by Total Sales**

- **668 Park St, San Francisco, CA** topped the list with $4,379.99 in total spending, showing a high-value customer segment.
- **391 1st St, Seattle, WA** and **795 1st St, Atlanta, GA** also featured prominently, highlighting key high-spending addresses.

### ** Sales Distribution by Product Category**

| Product                          | Total Sales        |
|----------------------------------|--------------------|
| Macbook Pro Laptop               | 8,037,600.00       |
| iPhone                           | 4,794,300.00       |
| ThinkPad Laptop                  | 4,129,958.66       |
| Google Phone                     | 3,319,200.00       |
| 27in 4K Gaming Monitor           | 2,435,097.50       |
| 34in Ultrawide Monitor           | 2,355,557.95       |
| Apple Airpods Headphones         | 2,349,150.00       |
| Flatscreen TV                    | 1,445,700.00       |
| Bose SoundSport Headphones       | 1,345,565.40       |
| 27in FHD Monitor                 | 1,132,424.54       |
| Vareebadd Phone                  | 827,200.00         |
| 20in Monitor                     | 454,148.70         |
| LG Washing Machine               | 399,600.00         |
| LG Dryer                         | 387,600.00         |
| Lightning Charging Cable         | 347,094.15         |
| USB-C Charging Cable             | 286,501.25         |
| Wired Headphones                 | 246,478.43         |
| AA Batteries (4-pack)            | 106,118.40         |
| AAA Batteries (4-pack)           | 92,740.83          |

#### **High-Performing Products**
- **Macbook Pro Laptop**: $8,037,600
- **iPhone**: $4,794,300
- **ThinkPad Laptop**: $4,129,958.66

These categories represent major revenue contributors and should be prioritized in future sales strategies.

### ** Sales Variance Between Cities**


| City           | Total Sales       |
|----------------|-------------------|
| San Francisco  | 8,262,203.87      |
| Los Angeles    | 5,452,570.77      |
| New York City  | 4,664,317.41      |
| Boston         | 3,661,641.99      |
| Atlanta        | 2,795,498.57      |
| Dallas         | 2,767,975.39      |
| Seattle        | 2,747,755.47      |
| Portland       | 2,320,490.60      |
| Austin         | 1,819,581.74      |

Sales performance varies significantly between cities:
- **San Francisco**: Highest revenue at $8,262,203.87.
- **Los Angeles** and **New York City**: Important markets with substantial sales figures.

Understanding this variance helps tailor regional marketing efforts and resource allocation.



### ** Top 10 Customer Purchase Frequency**

Here's the data presented in a tabular format:

| Purchase Address                          | Purchase Count |
|-------------------------------------------|----------------|
| 193 Forest St, San Francisco, CA 94016    | 9              |
| 223 Elm St, Los Angeles, CA 90001         | 8              |
| 279 Sunset St, San Francisco, CA 94016    | 8              |
| 716 5th St, San Francisco, CA 94016       | 7              |
| 727 9th St, San Francisco, CA 94016       | 7              |
| 640 West St, San Francisco, CA 94016      | 7              |
| 662 Chestnut St, San Francisco, CA 94016  | 7              |
| 284 Walnut St, San Francisco, CA 94016    | 7              |
| 176 North St, San Francisco, CA 94016     | 7              |
| 197 Center St, San Francisco, CA 94016    | 7              |


- **193 Forest St, San Francisco, CA**: 9 purchases, indicating a highly engaged customer.
- **223 Elm St, Los Angeles, CA**: 8 purchases, highlighting another frequent buyer.

Identifying these high-frequency customers can help in developing loyalty programs and personalized marketing strategies.

### ** Sales Contribution by Product**

Here's the data presented in a tabular format:

| Product                        | Total Sales     | Sales Contribution Percentage |
|--------------------------------|-----------------|-------------------------------|
| Macbook Pro Laptop             | 8,037,600       | 23.30%                         |
| iPhone                         | 4,794,300       | 13.90%                         |
| ThinkPad Laptop                | 4,129,958.66    | 11.97%                         |
| Google Phone                   | 3,319,200       | 9.62%                          |
| 27in 4K Gaming Monitor         | 2,435,097.50    | 7.06%                          |
| 34in Ultrawide Monitor         | 2,355,557.95    | 6.83%                          |
| Apple Airpods Headphones       | 2,349,150       | 6.81%                          |
| Flatscreen TV                  | 1,445,700       | 4.19%                          |
| Bose SoundSport Headphones     | 1,345,565.40    | 3.90%                          |
| 27in FHD Monitor               | 1,132,424.54    | 3.28%                          |
| Vareebadd Phone                | 827,200         | 2.40%                          |
| 20in Monitor                   | 454,148.70      | 1.32%                          |
| LG Washing Machine             | 399,600         | 1.16%                          |
| LG Dryer                       | 387,600         | 1.12%                          |
| Lightning Charging Cable       | 347,094.15      | 1.01%                          |
| USB-C Charging Cable           | 286,501.25      | 0.83%                          |
| Wired Headphones               | 246,478.43      | 0.71%                          |
| AA Batteries (4-pack)          | 106,118.40      | 0.31%                          |
| AAA Batteries (4-pack)         | 92,740.83       | 0.27%                          |

- **Macbook Pro Laptop**: Contributed 23.30% to overall sales.
- **iPhone**: 13.90%
- **ThinkPad Laptop**: 11.97%

Understanding each product's contribution helps in strategic decision-making regarding product focus and inventory management.

### ** Sales by Weekday**


| **Weekday** | **Total Sales**          |
|-------------|--------------------------|
| Tuesday     | $5,087,956.76             |
| Wednesday   | $4,988,822.23             |
| Sunday      | $4,932,169.64             |
| Saturday    | $4,904,356.99             |
| Monday      | $4,883,326.70             |
| Friday      | $4,855,938.36             |
| Thursday    | $4,839,465.13             |

- **Tuesday** emerged as the most profitable day with $5,087,956.76 in sales.
- **Wednesday** and **Sunday** also performed well, indicating strong sales potential during these weekdays.



Based on the findings from the 2019 sales data analysis, here are some recommendations:

### **1. Optimize Seasonal Strategies**
- **Focus on Peak Periods:** Since December is the highest-performing month, intensify marketing efforts and promotions during this period to maximize revenue. Similarly, plan for high-impact campaigns in October and April, which also showed strong performance.
- **Address Low-Performing Months:** Develop targeted marketing strategies to boost sales in January, September, and February. Consider offering discounts or special promotions to counteract seasonal declines.

### **2. Enhance Time-of-Day Marketing**
- **Leverage Peak Sales Hours:** Given that peak sales hours are between 18:00 and 20:00, allocate more resources and marketing efforts during these times. Optimize online and offline campaigns to capture the increased consumer activity.
- **Improve Off-Peak Sales:** Develop strategies to increase sales during the early morning hours (2:00 to 4:00). Consider targeted promotions or incentives to drive sales during these less active times.

### **3. Tailor Regional Strategies**
- **Focus on High-Revenue Cities:** Concentrate marketing and sales efforts in high-revenue cities like San Francisco, Los Angeles, and New York City. These cities are significant revenue generators and should be prioritized in resource allocation and promotional activities.
- **Address Low-Performing Cities:** Investigate the reasons behind lower sales in cities like Austin and Portland. Develop region-specific strategies to enhance performance in these areas, possibly through localized promotions or increased visibility.

### **4. Prioritize High-Performing Products**
- **Product Focus:** Prioritize products with high sales value and contribution, such as the Macbook Pro Laptop, iPhone, and ThinkPad Laptop. Ensure sufficient inventory and consider bundling these items with other products to boost overall sales.
- **Review Low-Contribution Products:** Evaluate the sales performance of lower-contribution products and consider strategies to either enhance their appeal or reduce their inventory if they are not meeting sales expectations.

### **5. Develop Customer Loyalty Programs**
- **Engage High-Frequency Customers:** Implement loyalty programs or personalized offers for high-frequency customers, such as those with multiple purchases from addresses like San Francisco. This can help retain valuable customers and encourage repeat purchases.

### **6. Optimize Product Category Strategy**
- **High-Contribution Categories:** Focus on product categories with high sales contributions, such as laptops and phones. Ensure these categories are well-promoted and consider expanding the range or offering complementary products.
- **Evaluate Lower-Contribution Categories:** Review the performance of lower-contribution products and assess if adjustments in marketing or inventory are needed to improve their performance.

### **7. Implement Weekly Sales Strategies**
- **Boost Sales on High-Performing Days:** Since Tuesday, Wednesday, and Sunday are top-performing days, consider running special promotions or events on these days to leverage higher sales potential.
- **Address Lower-Performing Days:** Develop strategies to increase sales on lower-performing days like Friday and Thursday, such as offering exclusive deals or promotions.


---

### **6. Conclusion**

The comprehensive analysis of the 2019 sales data reveals several key trends and insights that are crucial for strategic planning. Here’s a summary of the major findings:

1. **Sales Performance:** December was identified as the peak month for sales, driven likely by holiday shopping, while January experienced a significant drop, reflecting typical post-holiday seasonality. This highlights the importance of targeted marketing and promotions during high and low sales periods.

2. **Product Insights:** High-value products such as the MacBook Pro Laptop and iPhone generated substantial revenue, indicating strong demand for premium items. Conversely, lower-value products contributed less to overall sales, suggesting a need for a strategic review of product offerings and inventory management.

3. **Geographic Analysis:** San Francisco emerged as the top-performing city in terms of both sales volume and revenue, emphasizing its importance as a key market. Understanding regional sales patterns can help in optimizing marketing strategies and resource allocation.

4. **Temporal Patterns:** Sales data showed peak performance during late afternoon to early evening hours, with significant drops during early morning hours. This temporal insight suggests opportunities for targeted sales promotions during peak hours and strategies to boost sales during off-peak times.

5. **Customer Insights:** High-frequency customers, particularly those with multiple purchases, should be a focus for loyalty programs and personalized marketing efforts. Identifying these key customers can enhance customer retention and boost sales.

**Summary:**
This report underscores the importance of leveraging sales data to inform strategic decisions. By focusing on high-performing products, optimizing marketing strategies based on geographic and temporal patterns, and targeting high-value customers, businesses can enhance their sales performance and better align their strategies with market demands. Future work may include deeper dives into specific regions or products, as well as exploring additional data sources for a more comprehensive analysis.


**Additional Resources:**

- [GitHub Repository](https://www.linkedin.com/in/yemi-fatodu/) – Access the full project, including data analysis scripts and detailed findings.
- [Tableau Public Visualizations](https://public.tableau.com/app/profile/yemi.fatodu1473/viz/MeriSkillInternship1SalesDashBoard/Dashboard1) – Explore the interactive visualizations that complement the analysis and provide deeper insights into the data.




