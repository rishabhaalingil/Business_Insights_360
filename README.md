# Objective
AtliQ Technologies, a fast-growing consumer electronics brand, struggled with data inefficiencies and missed insights, relying solely on Excel—which became a major issue during a financial downturn in Latin America.Leveraged Power BI to transform data analytics, enabling departments like Finance, Sales, Marketing, and Supply Chain to gain faster, actionable insights. The project involved a vast dataset with over 1.8 million records.

# Solution Highlights
1. Finance View: Drill down into Profit & Loss, Net Sales trends, and identify top products and customers by various metrics.
2. Sales View: Analyze Customer and Product performance metrics like Net Sales, Gross Margin %, and unit economics (COGS, deductions).
3. Marketing View: Gain a comprehensive overview of Product, Market, Regional, and Customer performance, including GM%, NP%, and unit economics with detailed COGS and expenses.
4. Supply Chain View: Measure Forecast Accuracy, Net Error, and Absolute Error, and track accuracy and error trends for supply chain optimization.
5. Executive View: A real-time executive dashboard to monitor performance by division, customers, products, and channels.

# Steps Followed
1. **Project Planning and Scoping**:
   The Project Planning and Scoping phase ensured that the Power BI dashboard for AtliQ Hardwares was delivered within scope, on time, and with the right set of features to meet business needs. By defining clear objectives, understanding stakeholder requirements, and setting boundaries, the project was structured to deliver meaningful insights across multiple business functions, enabling data-driven decisions. This involved:

   1. **Defining Project Objectives and Goals**:
      - Improve the efficiency of reporting and reduce the time spent on manual data manipulation.
      - Deliver a user-friendly dashboard that integrates various data sources (sales, inventory, finance, etc.) for a holistic view of the business.

   2. **Stakeholder Identification and Involvement**:
     Scoping the project also means identifying all key stakeholders (e.g., department heads, end users, decision-makers) who will be involved in the project or who will benefit from it. Stakeholders may include people from **Sales**, **Marketing**, **Finance**, and **Supply Chain** teams in the case of this Power BI dashboard project. The steps involved are:
     
      - Clarify stakeholder expectations: Understanding what each stakeholder group needs from the dashboard, which features and KPIs are most important to them.
      - Regular communication and feedback: Plan for ongoing discussions and feedback loops to ensure the project is aligned with user needs throughout the development process.

   3. **Scope Definition**:
     The scope of the project is defined by clearly outlining the specific deliverables, features, and functionality of the project. This includes deciding what will be included—and, just as importantly, what will not be included—in the final deliverable.

   4. **Estimating Time, Resources, and Budget**:
     A detailed project timeline should be created, with clearly defined milestones and deadlines. This includes estimating the time and resources required for each stage of the project.

   5. **Risk Identification and Mitigation**:
     Risk planning involves identifying potential challenges or risks that could hinder project progress. For each risk, mitigation strategies should be outlined.

   6. **Deliverables and Mitigation**:
     The final deliverables should be clearly defined in the planning stage. These include:
      - A fully functional Power BI dashboard that provides real-time insights across key departments.
      - User guides or training materials to help stakeholders navigate and utilize the dashboard.
      - Documentation for future updates or maintenance.

   7. **Communication Plan**:
     A solid communication plan is necessary to keep all team members and stakeholders updated. This includes:
       - **Regular progress updates**: Schedule recurring meetings to discuss the project’s progress, address any challenges, and align with stakeholders on evolving requirements.
       - **Documentation of key decisions**: Document any significant changes, feedback, or decisions made throughout the project.

2. **Data Collection,Exploration and validation**:
    1. Imported the data to MySql.
    2. Data Exploration using MySql.
    3. Validated data against benchmark numbers.Data validation in Power BI against the benchmark numbers provided by the product owner.Address gaps found during data validation
    4. Created a date dimension table.
         
3. **Data Transformation in Power Query**:
    1. **Reviewed Finance Mockups**: Analyzed the provided finance mockups to understand the required structure and data needed for reporting.
    2. **Transform Data in Power Query**: Utilized Power Query M formula language and other features (such as merging tables) to generate a unified table that combines both actual and estimated data.
    3. **Created Calculated Columns in Power Query Editor**: Created new calculated columns within Power Query to manipulate and shape the data as per reporting requirements.

4. **Data Modelling and Calculated Columns**:
    1. **Using DAX for Creating Calculated Columns**: Applied Data Analysis Expressions (DAX) to create calculated columns for advanced analysis and reporting.
    2. **Connected Facts and Dimension Tables in a Snowflake Schema**: Structured the data model by linking fact and dimension tables in a snowflake schema to optimize data relationships and enable efficient querying and reporting.

   
5. **Dashboard Development**:

   1. **Built Finance View**:
      - Contains **Profit and Loss Statement**, **Net Sales Performance Over Time** (line chart), and **Top/Bottom Product and Customers by Net Sales** (matrix format).
      - Contains the KPIs: **Net Sales**, **Gross Margin Percentage**, and **Net Profit Percentage**.
      - Includes a **toggle button** to switch between the current year target and the last year data.

   2. **Built Sales View**:
      - Contains **Customer Performance Table** and **Product Performance Table** with rows for customer and product, and columns for **Net Sales**, **Gross Margin**, and **Gross Margin Percentage**.
      - Includes a **Performance Matrix** (scatter chart) with **regional sales data** against **Gross Margin Percentage** and **Net Sales**.
      - **Unit Economics** donut chart showing the percentage distribution of **Net Sales**, **Total Post Invoice Deductions**, **Pre Invoice Deductions**, and another one showing the percentages of **Total Cost of Goods Sold** and **Gross Margin**.
      - Contains a **toggle button** to switch between the current year target and the last year data.

   3. **Built Marketing View**:
      - Contains **Product Performance Table** with rows for customer and product, and columns for **Net Sales**, **Gross Margin**, **Gross Margin Percentage**, **Net Profit**, and **Net Profit Percentage**.
      - Contains **Region/Market Performance Table** with regional data against the metrics such as **Net Sales**, **Gross Margin**, **Gross Margin Percentage**, **Net Profit**, and **Net Profit Percentage**.
      - Includes a **Performance Matrix** (scatter chart) of **Product Division** against **Net Sales** and **Net Profit Percentage**. Also includes a **toggle button** to switch between **Net Profit Percentage** and **Gross Margin Percentage**.
      - **Donut Chart** showing the percentage of **Total Goods Sold** and **Gross Margin**. The donut chart provides a visual representation of the relationship between **COGS** and **Gross Margin Percentage** for AtliQ Hardwares.
      - **Waterfall Chart** showing **Gross Margin**, **Operational Costs**, and **Net Profit**. This chart helps visualize the relationship between **Gross Margin** and **Net Profit**.

   4. **Built Supply Chain View**:
      - Contains key **KPIs**: **Forecast Accuracy Percentage (FCA%)**, **Net Error**, and **Net Profit Percentage**.
      - Includes a table showing **FCA**, **FCA % of Last Year (LY)**, **Net Error**, **Net Error Percentage**, and **Risk Associated with Different Customers**. This equips the Supply Chain team with performance metrics to track and improve the accuracy of demand forecasting.
      - **Accuracy/Net Error Trend Graph** showing the **Net Error** and the comparison between **FCA** of this year and last year. This helps evaluate forecasting accuracy and improve strategies over time.
      - Contains a **Product Metrics Table** showing **FCA**, **FCA %**, **Net Error**, **Net Error Percentage**, and **Risk** associated with each product division.

   5. **Built Executive View**:
      - Contains some key **KPIs** such as **GM %**, **Net Sales**, **Net Profit Percentage**, and **FCA %**. These KPIs also contain the data from the **Last Year** and the **Target for the Present Year**, which can be selected from a toggle button on the page. The difference between the numbers is also calculated and displayed on the KPI, thereby easily letting the user compare the performance of this year compared to the last year and also helps them compare the numbers with the target of the present year.
      - **Key Insights by Subzone Table** showing **Net Sales**, **Gross Margin %**, **Revenue Contribution % (RC%)**, **AtliQ Market Share %**, **Net Profit Percentage**, **Net Error Percentage**, and **Risk** associated with different subzones. This lets stakeholders analyze performance across different subzones.
      - **Ribbon Chart** showing the **Market Share Growth** of the different contributors across different years.
      - **Revenue By Division** and **Revenue By Channel** - donut charts showing the percentage of revenue generated by different divisions and the revenue generated by different types of channels, respectively.
      - **Line and Clustered Column Chart** showing **Net Sales** as columns and **Gross Margin %**, **Net Profit %**, and **AtliQ Market Share %** as lines across different years.
      - Contains two tables showing the **Top 5 Customers** and **Top 5 Products** based on their **Net Sales** and also shows their **Revenue Contribution %** and **Gross Margin %**.

   6. **Added Filters and Slicers**:
          - Added filters of fiscal years and quarters to all the views.
          - Added Year to Date and Year to Go filters to all the views to compare the sales data from the beginning of the year to the present date and the target and forecast data from the present date till the end of the year.This helps us to understand  how much we need to sell in the rest of the year to meet the target or meet our forecast plan.
          - Added Last Year and Target buttons on all the views to compare the data of the previous year vs the target to attained for the current year.
          - Also added regional, segment-wise, and customer-based filters to all the views to allow stakeholders to filter the data based on these dimensions, enabling more granular analysis and helping users to view the data from different perspectives according to specific regions, business segments, or individual customer performance.

 6. **Deploying the Solution**

    1. **Published the Report to Power BI Service**
        - The report, once finalized and tested locally, was uploaded to the **Power BI Service** platform. This allows for easy sharing and distribution of the report among stakeholders, including team members, managers, and other relevant personnel. The report was published to a **workspace** within Power BI Service, ensuring that authorized users can access it online.
        - By doing so, we enabled **real-time access** to the most up-to-date data and provided the opportunity for **interactive exploration** of the data through Power BI’s rich visualizations.

    2. **Installed a Personal Gateway and Connected Local Computer with Power BI Service for Automatic Data Refresh of MySQL Database**
        - To ensure the data in the Power BI reports remained up-to-date, I installed a **personal gateway** on the local computer. The gateway acts as a bridge between on-premises data sources (in this case, the **MySQL database**) and the Power BI Service in the cloud.
        - This setup allows Power BI to **automatically refresh the data** on a scheduled basis, without needing manual intervention. This ensures the reports always reflect the most current data, making the reporting process more efficient and up-to-date.

    3. **The Excel Files Were Uploaded to the SharePoint Folder via Teams for the Automatic Data Refresh of the Excel Files Data**
        - By uploading the **Excel files** to **SharePoint**, I enabled **automatic data refresh** for the reports that pull data from these files. Power BI is able to connect to **SharePoint Online** and automatically refresh the data whenever the Excel files are updated, ensuring the reports always reflect the latest changes without needing to manually upload or modify the data.
        - The integration between **Teams**, **SharePoint**, and **Power BI** creates a streamlined workflow, where stakeholders can update the data in the Excel files within the Teams environment, and Power BI automatically pulls the latest version for report generation.

7. **Data Validation**:


   1. **Exported the Report to Excel Using the "Analyze in Excel" Option and Analyzed Results in PivotTables**
      - Using Power BI’s “Analyze in Excel” feature, I exported the report data into an Excel file. This feature allowed for a seamless integration between Power BI and Excel, enabling users to manipulate and analyze the data outside of Power BI while retaining the report's data structure and relationships. Once in Excel, the data was analyzed using PivotTables to derive insights and trends, allowing for more detailed and customizable analysis. PivotTables provided the flexibility to perform data aggregation, comparison, and visualization based on different filters and dimensions.

   2. **Data Validation Was Carried Out with the Benchmark Numbers from the Previous Years and Also the Target Values of the Current Year**
       - To ensure the accuracy and integrity of the data, a thorough data validation process was conducted. This involved comparing the current report’s data against benchmark numbers from previous years, which served as a point of reference for consistency and historical performance. In addition, the current year's target values were also used for validation to ensure that the results align with the expected goals and objectives. Any discrepancies between the actual data and benchmark/target figures were flagged for further review and corrective actions, ensuring the report’s data is reliable and actionable.

   3. **User Acceptance Testing (UAT) Is Done for the First Round of Testing by End-Users So That Obvious Issues Can Be Identified Before the Solution Is Released to a Broad Range of Users**
       - As part of the quality assurance process, a round of User Acceptance Testing (UAT) was carried out with a select group of end-users. This stage of testing allowed real users to interact with the report and provide feedback on its functionality, usability, and accuracy. The goal was to identify and resolve any obvious issues, such as data errors, interface problems, or user experience concerns, before the solution is rolled out to a larger audience. The feedback collected during this phase was used to make necessary adjustments and ensure that the final solution meets user expectations and delivers the required value.


8. **Stakeholder Review and Feedback Implementation**:
    1. **The reports were reviewed by the stakeholders and their suggestions were provided.Steps were taken to implement these suggestions**.
       - After the initial report was shared with stakeholders, a thorough review process was conducted to gather their feedback. This included gathering input on report content, layout, accuracy, and overall usefulness.
       - Based on their input, a set of actionable steps was taken to refine and enhance the report. These adjustments not only addressed specific stakeholder concerns but also ensured that the report better aligned with the business objectives. By actively involving stakeholders in the process and incorporating their feedback, we ensured that the final report is more tailored to their needs, which leads to more effective decision-making.
   
   2. **Stakeholder mapping was done to understand the stakeholder expectation and personalities**.
      - To ensure that the report met the diverse needs of all involved parties, a stakeholder mapping exercise was conducted. This involved identifying and categorizing key stakeholders based on their roles, influence, and expectations of the report. By understanding the priorities of each stakeholder group—whether they were more focused on high-level metrics, in-depth analysis, or actionable insights—we were able to tailor the content to suit their needs.
      - Additionally, understanding the personalities and preferences of different stakeholders allowed for more effective communication.
  
   3. **Focussed on fixing the data quality issues and improve the performance optimization**.
      - A significant emphasis was placed on ensuring that the report’s data was accurate, reliable, and of the highest quality. The data quality review involved identifying and addressing any inconsistencies, missing values, or errors in the dataset that could lead to inaccurate insights.
      - In addition to data quality, the performance optimization of the report was prioritized. This involved analyzing the report's responsiveness and load times, particularly when handling large datasets or complex visualizations. Steps were taken to streamline calculations, optimize queries, and reduce unnecessary processing time, resulting in faster report generation and smoother user experience.

# Significance
The implementation of Power BI for AtliQ Technologies has had a transformative impact on the company, particularly by improving data-driven decision-making across critical departments. Below are the key ways this project has helped AtliQ Technologies:

1.**Improved Data Efficiency and Reporting Speed**:

The company was previously reliant on Excel for data analysis, which was not only time-consuming but also prone to errors, especially when handling large datasets like those with over 1.8 million records. Power BI streamlined the reporting process, allowing users to generate and access real-time reports with just a few clicks. This significantly reduced manual efforts and time spent on report generation, enabling employees to focus on more strategic tasks.

2.**Enhanced Decision-Making Capabilities**:

 With Power BI, AtliQ’s finance, sales, marketing, and supply chain teams can now access detailed, interactive dashboards that provide real-time insights into key performance metrics (KPIs). This has empowered stakeholders to make more informed decisions by having immediate access to performance data on Net Sales, Gross Margin, Forecast Accuracy, and more. By providing these insights across multiple functions, the company has improved its ability to react quickly to changes in the market or business performance.
 
3.**Data Integration and Holistic View**:

The project integrated data from various departments such as finance, sales, marketing, and supply chain into a unified system. By bringing all of this data into Power BI, AtliQ has been able to break down silos, providing a holistic view of business operations. Stakeholders can now easily analyze performance across different segments, regions, customers, and products in one place, which enhances collaboration and alignment between departments.

4.**Accurate Forecasting and Supply Chain Optimization**:

With key metrics like Forecast Accuracy, Net Error, and Net Profit Percentage, the Supply Chain team has been able to track and optimize their forecasting process. The inclusion of Risk Metrics also provides critical insights into the potential supply chain issues, helping the company to better anticipate and mitigate risks. This leads to better inventory management and a more efficient supply chain process overall, helping AtliQ reduce operational costs and improve service levels.

5.**Greater Transparency and Stakeholder Alignment**:

The integration of performance data into real-time dashboards has fostered transparency across different levels of the organization. Stakeholders, from department heads to top executives, can now access detailed and up-to-date performance metrics. This improves alignment and ensures everyone has the same understanding of the company's performance against targets, historical benchmarks, and future forecasts, reducing misunderstandings and enabling better strategic planning.

6.**User Empowerment and Self-Service Analytics**:

With the intuitive interface of Power BI, AtliQ employees no longer have to rely on IT or data teams to generate reports. The self-service nature of Power BI enables users to slice and dice the data based on their specific needs—whether by region, product, or customer segment. This autonomy increases the speed of decision-making and reduces bottlenecks, allowing teams to quickly identify opportunities, risks, and actionable insights.

7.**Cost and Resource Savings**:

Automating data refresh processes through Power BI's integration with MySQL and SharePoint significantly reduces the manual effort required to maintain accurate and up-to-date reports. This automation also lowers the risk of human errors and ensures consistent data quality across reports. The time saved by departments no longer needing to manually update or compile reports can be redirected towards value-added activities, enhancing productivity across the organization.

8.**Better Alignment with Strategic Goals**:

With the capability to compare current performance against targets and historical benchmarks, AtliQ can assess how well it is progressing toward its strategic goals. The ability to drill into data and filter it by year, customer, segment, or region helps managers understand the reasons behind variances and adjust strategies accordingly. Whether it's identifying top-performing customers or pinpointing underperforming products, Power BI ensures the company stays focused on its core objectives.

9.**Scalability for Future Growth**:

As AtliQ continues to expand and its dataset grows, Power BI’s scalability ensures that the company can continue to derive insights from larger volumes of data. The flexible architecture of the Power BI dashboard allows it to accommodate new data sources and additional KPIs, future-proofing the company’s analytics infrastructure.

10.**Competitive Advantage**:

By embracing data analytics with Power BI, AtliQ Technologies has gained a significant edge over competitors who may still rely on manual or outdated reporting methods. With faster, more accurate insights, AtliQ can respond more swiftly to market changes, better serve its customers, and strategically position itself for long-term success in the consumer electronics space.


 
