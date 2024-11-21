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

   - **Defining Project Objectives and Goals**:
     - Improve the efficiency of reporting and reduce the time spent on manual data manipulation.
     - Deliver a user-friendly dashboard that integrates various data sources (sales, inventory, finance, etc.) for a holistic view of the business.

   - **Stakeholder Identification and Involvement**:
     Scoping the project also means identifying all key stakeholders (e.g., department heads, end users, decision-makers) who will be involved in the project or who will benefit from it. Stakeholders may include people from **Sales**, **Marketing**, **Finance**, and **Supply Chain** teams in the case of this Power BI dashboard project. The steps involved are:
     
     - Clarify stakeholder expectations: Understanding what each stakeholder group needs from the dashboard, which features and KPIs are most important to them.
     - Regular communication and feedback: Plan for ongoing discussions and feedback loops to ensure the project is aligned with user needs throughout the development process.

   - **Scope Definition**:
     The scope of the project is defined by clearly outlining the specific deliverables, features, and functionality of the project. This includes deciding what will be included—and, just as importantly, what will not be included—in the final deliverable.

   - **Estimating Time, Resources, and Budget**:
     A detailed project timeline should be created, with clearly defined milestones and deadlines. This includes estimating the time and resources required for each stage of the project.

   - **Risk Identification and Mitigation**:
     Risk planning involves identifying potential challenges or risks that could hinder project progress. For each risk, mitigation strategies should be outlined.

   - **Deliverables and Mitigation**:
     The final deliverables should be clearly defined in the planning stage. These include:
     - A fully functional Power BI dashboard that provides real-time insights across key departments.
     - User guides or training materials to help stakeholders navigate and utilize the dashboard.
     - Documentation for future updates or maintenance.

   - **Communication Plan**:
     A solid communication plan is necessary to keep all team members and stakeholders updated. This includes:
     - **Regular progress updates**: Schedule recurring meetings to discuss the project’s progress, address any challenges, and align with stakeholders on evolving requirements.
     - **Documentation of key decisions**: Document any significant changes, feedback, or decisions made throughout the project.

 2. **Data Collection,Exploration and validation**:
       - Imported the data to MySql.
       - Data Exploration using MySql.
       - Validated data against benchmark numbers.Data validation in Power BI against the benchmark numbers provided by the product owner.
         Address gaps found during data validation
       - Created a date dimension table.
         
3. **Data Transformation in Power Query**:
       - Reviewed Finance Mockups
       - Transform data in power query:Used power query M formula language and some other features (such as merge tables) to generate a single table containing both actuals and estimates.
       - Created calculated columns in power query editor
   
4. **Data Modelling and Calculated Columns**:
       - Using DAX for creating calculated columns.
       - Connected facts and dimension tables in a snowflake schema.
   
5. **Dashboard Development**:
   1. **Built Finance View**:
    - Contains **Profit and Loss Statement**, **Net sales performance over time** (line chart), and **Top/Bottom product and customers by Net Sales** (matrix format).
    - Contains the KPIs: **Net Sales**, **Gross Margin percentage**, and **Net Profit percentage**.
    - Includes a **toggle button** to switch between the current year target and the last year data.

   2. **Built Sales View**:
    - Contains **customer performance table** and **product performance table** with rows for customer and product, and columns for **Net Sales**, **Gross Margin**, and **Gross Margin Percentage**.
    - Includes a **performance matrix** (scatter chart) with **regional sales data** against **Gross Margin Percentage** and **Net Sales**.
    - **Unit Economics** donut chart showing the percentage distribution of **Net Sales**, **Total Post Invoice Deductions**, **Pre Invoice Deductions**, and another one showing the percentages of **Total Cost of Goods Sold** and **Gross Margin**.
    - Contains a **toggle button** to switch between the current year target and the last year data.

   3. **Built Marketing View**:
    - Contains **product performance table** with rows for customer and product, and columns for **Net Sales**, **Gross Margin**, **Gross Margin Percentage**, **Net Profit**, and **Net Profit Percentage**.
    - Contains **region/market performance table** with regional data against the metrics such as **Net Sales**, **Gross Margin**, **Gross Margin Percentage**, **Net Profit**, and **Net Profit Percentage**.
    - Includes a **performance matrix** (scatter chart) of **product division** against **Net Sales** and **Net Profit Percentage**. Also includes a **toggle button** to switch between **Net Profit Percentage** and **Gross Margin Percentage**.
    - **Donut chart** showing the percentage of **Total Goods Sold** and **Gross Margin**. The donut chart provides a visual representation of the relationship between **COGS** and **Gross Margin Percentage** for AtliQ Hardwares.
    - **Waterfall chart** showing **Gross Margin**, **Operational Costs**, and **Net Profit**. This chart helps visualize the relationship between **Gross Margin** and **Net Profit**.

   4. **Built Supply Chain View**:
    - Contains key **KPIs**: **Forecast Accuracy Percentage (FCA%)**, **Net Error**, and **Net Profit Percentage**.
    - Includes a table showing **FCA**, **FCA % of Last Year (LY)**, **Net Error**, **Net Error Percentage**, and **Risk associated with different customers**. This equips the Supply Chain team with performance metrics to track and improve the accuracy of demand forecasting.
    - **Accuracy/Net Error trend graph** showing the **Net Error** and the comparison between **FCA** of this year and last year. This helps evaluate forecasting accuracy and improve strategies over time.
    - Contains a **product metrics table** showing **FCA**, **FCA %**, **Net Error**, **Net Error Percentage**, and **Risk** associated with each product division.

   5.**Built Executive View**:
   
                        
 
