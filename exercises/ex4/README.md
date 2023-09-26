# Exercise 4 - Creating the Charts in Sales Order Management Dashboard for displaying Data

## Exercise 5.1 Creating the first Chart for displaying **Quantity per Product Category**

This exercise focuses on creating the first chart for displaying **"Short Qty per Sales Organization"** in a dashboard. The purpose of this chart is to provide an overview of the Quantities of various products with it's sales organization, allowing users to identify shortage of any item.

To complete this exercise, you will need to follow these steps:

1. Select the appropriate chart type for displaying Short Qty per Sales Organization, such as a bar chart or a pie chart.
2. Choose the appropriate visualization settings, such as the color scheme, labels, and axes, to ensure that the data is easy to read and visually appealing.
3. Select the appropriate fields from the data source to display Short Qty per Sales Organization.
4. Configure any necessary filters or sorting options to ensure that the data is displayed accurately and in the desired order.

Your objective is to create a chart that accurately displays the Short Qty per Sales Organization in a clear and visually appealing way, allowing users to quickly identify quantity of different sales organization and make informed decisions. Best of luck!

 ![Chart1](images/sacchart1.png)

### Step by Step Solution Guide

After assigning the dataset, you can start building your first charts

1. 👉 Drag and drop from the left panel a **Chart** widget into the first container

   ![SAC Chart](images/sacchart1drag.png)

2. 👉 Select the chart and add the following properties in a **Builder** on the right panel 
    - Dimensions: **SalesOrganization**

   ![SAC Chart](images/chart1properties.png)

3. 👉 Add a new **Calculation** as a **Measure**
    - Type: **Calculated Measure**
    - Name: **Short Qty**
    - Formula: **["unified_sales_delivery_view_model":OrderQuantity"] - ["unified_sales_delivery_view_model":DeliveredQuantity]** (This will be the Analytic Model Name which you created in SAP Datashpere in Exercise 2)

   ![SAC Chart](images/chartcalculatedc.png)

4. 👉 Add a **Threshold****
    - Click on the Chart, scroll down to the Chart Add-Ons section and click on Threshold
    - Add Measure as **Short Qty**
    - Add **Range** (as shown in the screenshot below)
    - Click on **Apply**

   ![SAC Chart](images/threshold.png)

5. 👉 Make Threshold visible on the Chart (refer to the screenshot)
    - In Measure section, click on **Threshold Icon** of **Short Qty** 
    - Click on **Show Threshold** and select **Story Defined**, then select **Short Qty**

   ![SAC Chart](images/showthreshold.png)

6. 👉 Give some proper name ("Short Qty per Sales Organization") and your first chart is ready.

   ![SAC Chart](images/sacchart1.png)


## Exercise 5.2 Creating another Chart for displaying **Discount per Product Category**

This exercise focuses on creating another chart for displaying **"Monthly Case Fill- 12 Month Trend"** in the dashboard. The purpose of this chart is to provide an overview of the sales organization with their Case Fill % of 12 months.

To complete this exercise, you will need to follow these steps:

1. Select the appropriate chart type for displaying quantity by product category, such as a bar chart or a pie chart.
2. Choose the appropriate visualization settings, such as the color scheme, labels, and axes, to ensure that the data is easy to read and visually appealing.
3. Select the appropriate fields from the data source to display discount by product category.
4. Configure any necessary filters or sorting options to ensure that the data is displayed accurately and in the desired order.
5. Optionally you can add a reference line for the average discount.

Your objective is to create a chart that accurately displays the Monthly Case Fill- 12 Month Trend in a clear and visually appealing way, allowing users to quickly identify trends and make informed decisions. Best of luck!
 
 ![Chart2](images/sacchart2.png)

### Step by Step Solution Guide

Similar to the previous approach create another chart to visualize the **Discount** per Product Category**

1. 👉 Drag and drop from the left panel a **Chart** widget into the second container

   ![SAC Chart](images/sacchart2drag.png)

2. 👉 Select the chart and add the following properties in a **Builder** on the right panel 
    - Dimensions: **Product_Category_Enhanced_Ecommerce**

   ![SAC Chart](images/chart2properties.png)

3. 👉 Add a new **Calculation** as a **Measure**
    - Type: **Calculated Measure**
    - Name: **DiscountC**
    - Formula: **["AM_Product_Sales_Country_Discount":discount]** (This will be the Analytic Model Name which you created in SAP Datashpere in Exercise 1)

   ![SAC Chart](images/chart2calculatedc.png)

4. 👉 Format it as a **Percentage****
    > Note: Uncheck the *Use unit of underlying measures* to activate the percentage option in Scale Dropdown

   ![SAC Chart](images/chart2formatt.png)

5. 👉 Click on the **...** "More Actions" and rank the **Product_Category_Enhanced_Ecommerce** as **Top 10**, to display top products per category.

   ![SAC Chart](images/char2top10.png)

6. 👉 Exclude the **(not set)** and **${productitem.product.origCatName}** attributes by selecting them and pressing **X**

   ![SAC Chart](images/char2exclude.png)

7. 👉 Give some proper name ("Discount per Product Category") and your second chart is ready. Optionally you can add a reference line for the average discount.

   ![SAC Chart](images/sacchart2.png)

## Congratulations!

Congratulations on completing your Exercise 5! You have successfully created Charts in Sales Order Management Dashboard for displaying Data!

Let's Continue to - [Exercise 5 - Creating the Table in Sales Order Management Dashboard for displaying Data](../ex5/README.md)