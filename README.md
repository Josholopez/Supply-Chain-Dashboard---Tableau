# Supply-Chain-Dashboard in Tableau
Analysis of Just-in-Time (JIT) performance within the supply chain of a retail company using Tableau. The project evaluates inventory availability, order fulfillment speed, and delivery timelines to assess efficiency and alignment with JIT principles.

# Analysis Process

1. **Download Data**  
   - Obtain CSV files from the [DataCamp repositories](https://app.datacamp.com/learn/courses/case-study-supply-chain-analytics-in-tableau).  
   - Inspect and handle null or missing values in Power Query.
   - Ensure consistency across datasets.

3. **Build Data Model in Tableau**  
   - Connect all relevant datasets.  
   - Create relationships between tables to maintain independence and avoid unions that produce a single large dataframe (which can slow dashboard performance).

4. **Define Granularity**  
   - Identify the level of detail by checking distinct counts of primary keys.

5. **Create Calculated Fields & Parameters**  
   - Develop KPIs such as **Shipment Delay** and **Order Delay** by comparing actual vs. scheduled lead time (in days).

6. **Use Level of Detail (LOD) Expressions**  
   - Calculate measures that respect the current view’s dimensions while adding deeper insights.

7. **Apply Dashboard Actions**  
   - Implement filter actions on specific visualizations.  
   - Resolve issues where filters applied to unrelated dimensions resulted in blank views.

# Conclusions
**Shipment Delay Trends and Performance Analysis**
  - Significant shipment delays were observed until mid-2016, impacting overall delivery performance.
  - The average delay across the entire period was 19.3 days, indicating a substantial gap from expected timelines.
  - The trend shows continuous improvement, with delays reducing over time and reaching an average of -0.85 days by December 2017, meaning shipments were delivered slightly ahead of schedule.

**Delivery categories Insights**
  - Delivery categories represent the number of days required to deliver goods from the order placement date, calculated by comparing actual delivery times against scheduled timelines.
  - A total of 66,367 orders were recorded during the analyzed period.
  - Over 56% of orders fall under the “On Schedule” or “Before Schedule” categories, indicating strong overall performance.
  - Shipments delayed by more than 5 days account for only 10% of total orders, but targeted actions to reduce this metric are recommended to further improve service levels.

**Understock Trend and fulfillment Insights**
  - Several product categories are experiencing severe understock issues, impacting availability and fulfillment performance.
  - The “Indoor/Outdoor Games” category shows the highest average monthly understock, with -45.58 items, and an average fulfillment time of 5.5 days to warehouse.

## Dashboard Preview
Explore the dashboard in [Tableau Public](https://public.tableau.com/views/Supply_Chain_Analysis_17636475531170/Analysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).  
![Nagrywanie2025-11-20201312-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/26ba23c9-4dba-43b1-be86-7c144481ff35)


