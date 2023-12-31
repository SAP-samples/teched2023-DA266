# Exercise 3 - Create a Sales Order Management Dashboard on SAP Analytics Cloud

This exercise will focus on leveraging previously created views to create rich Sales Order Management reports in SAP Analytics Cloud and get data in real-time. By integrating these data sources, the reports will allow for powerful data analysis and visualization of the sales performance of different product categories. The information gathered from these reports can be used to make informed decisions about product assortment, pricing, and promotions. The use of Databricks and SAP source systems will ensure that the data used in these reports is accurate, up-to-date, and consistent, providing a solid foundation for effective Sales Order Management decision-making.

## Exercise 3.1 Creating the Layout for the Sales Order Management Dashboard

This exercise focuses on creating the layout for a Sales Order Management Dashboard based on the displayed image. Determine the appropriate size and placement of each component to ensure a clear and concise presentation of the data.

  ![Layout](images/layout-result.png)

### Step by Step Solution Guide

1. 👉 Open the [SAP Analytics Cloud](https://techedsac-da266.ap11.hcs.cloud.sap/sap/fpa/ui/app.html#/home) using the provided credentials.
   
  ![SAC Home](images/sachome.png)


2. 👉 Go to the **Stories** and create a new **Canvas**
    
    >Use the Optimized Design mode, which provides an improved experience when designing dashboards. This mode has some useful new features, but it does not include all the features that are currently supported in the Classic Design mode.
    
    ![New View](images/newcanvas.png)


3. 👉 Drag and drop a **Text** field to give the dashboard name *"Sales Order Management Dashboard"*

4. 👉 Drag and drop 5 **Panels** into the canvas to shape a layout for the charts (see the screenshot below)
 
    ![Layout](images/saclayout.png)

## Exercise 3.2 Assigning the data from SAP Datasphere to Dashboard

This exercise focuses on adding the **"unified_sales_delivery_view_model"** model from SAP Datasphere as a data source in SAP SAC.

### Step by Step Solution Guide

1. 👉 Go to the **Tools** and press **Add new Data**, then select **Data from an existing dataset or model**
    
    ![SAC Data](images/sacdata.png)

2.  👉 Select the connection **SAP Datasphere** as a source, your space and the dataset
    - Connection: **TECHED2023**
    - Space: **TECHED_\<USER_NO>**
    - Dataset: **unified_sales_delivery_view_model**
  
    ![SAC Data](images/select_datasphere.png)

You have now successfully imported Data from your SAP Datashpere instance to SAC. 

## Congratulations!

Congratulations on completing your Exercise 3! You have successfully created the layout for "Sales Order Management Dashboard" and assigned data from SAP Datasphere to Dashboard!

Let's Continue to - [Exercise 4 - Creating the Charts in Sales Order Management Dashboard for displaying Data](../ex4/README.md)
