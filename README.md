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
   1. **Built finance view**:
                - Contains Profit and Loss Statement,Net sales performance over time which is a line chart,Top/Bottom product and customers by Net Sales in a matrix format.
                - Contains the KPI's : Net Sales,Gross Margin percentage,Net profit percentage.
                - Contains a toggle button to switch between the current year target and the last year data.

   2.**Built sales view**:
                  - Contains customer performance table and product performance table which contains the customer and product at rows and Net Sales, Gross Margin and Gross margin percentage
                    in columns.
                  - Contains a performance matrix which is a scatter chart and contains the regional sales data against the Gross margin percentage and net sales.
                  - Unit Economics which is donut chart showing the percentage distribution of net sales,total post invoice deductions,pre invoice deductions and another one showing the percentages of total cost of goods sold and gross margin.
                  - Contains a toggle button to switch between the current year target and the last year data.
   
   3.**Built marketing view**:
                  - Contains product performance table which contains the customer and product at rows and Net Sales, Gross Margin and Gross margin percentage,Net profit,Net profit percentage in columns.
                  - Contains region/market performance table which contains the regional data against the metrics such as Net Sales,Gross Margin,Gross Margin percentage,Net profit,Net profit percentage.
                  - Performance matrix which is a scatter chart of product division against the net sales and net profit percentage metric.There is also a toggle button to switch between the net profit percentage and Gross Margin percentage.
                  - Donut chart showing the percentage of total goods sold and gross margin.The donut chart provides a clear visual representation of the relationship between the Total Cost of Goods Sold (COGS) and the Gross Margin Percentage for AtliQ Hardwares. This chart helps stakeholders understand the distribution of revenue between production costs and profit margin.
                  - Waterfall chart which shows the gross margin,operational costs and net profit.This chart helps us to understand the relationship between gross margin and net profit.

    4.**Built Supply Chain View**:
                  - Contains some key KPI's such as Forecast Accuracy percentage(FCA %),Net Error,Net Profit percentage.
                  - Contains a table which shows the FCA, FCA % of Last Year(LY), Net Error, Net Error Percentage,and Risk associated with different customers.This table equips the Supply Chain Team with key performance metrics that enable them to track and improve the accuracy of demand forecasting. By continuously refining forecasting processes, the team can achieve better inventory control, more efficient procurement, and ultimately reduce operational risks and costs, leading to a more streamlined and responsive supply chain.
                  - Accuracy/Net Error trend graph which shows the net error and the comparison between the FCA of this year and the previous year.By continuously monitoring this graph, the team can evaluate whether their predictions are becoming more accurate over time, identify patterns of error, and adjust their strategies to enhance forecasting accuracy, optimize inventory management, and ultimately improve the overall efficiency of the supply chain.
                 - There is also a product metrics table which gives the FCA,FCA %,Net Error,Net Error percentage and Risk associated with each of the product division.

   5.**Built Executive View**:
   
                        
 
