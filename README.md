[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2023-DA266)](https://api.reuse.software/info/github.com/SAP-samples/teched2023-DA266)

# DA266 - Federate Queries to Databricks from SAP Datasphere for Real-Time Analytics

## Description

This repository contains the material for the SAP TechEd 2023 session called DA266 - Federate Queries to Databricks from SAP Datasphere for Real-Time Analvtics.

## Overview

This session introduces attendees to analyze Sales order Monthly order fill rate. Order fill rate is the number of product units initially shipped as a percentage of all units ordered. An order fill rate can apply to both inbound units for a warehouse as well as outbound units for distributors and carriers.

You can see how to do unified analytics by creating unified business models that combine federated non-SAP data from Databricks with SAP business data to derive real-time business insights.  

## Requirements

The requirements/Existing SetUp to follow the exercises in this repository are:
1. A [SAP Datasphere System](https://www.sap.com/india/products/technology-platform/datasphere.html), configured with spaces and users with assigned roles. 
To get started, sign up for your [SAP Datasphere free tier tenant.](https://www.sap.com/products/technology-platform/datasphere/trial.html)

2. A [SAP Analytics Cloud account](https://www.sap.com/india/products/technology-platform/cloud-analytics.html) with live data connections to SAP Datasphere system to access SAP Datasphere Analytic Model or Perspective within SAP Analytics Cloud.
To get started, sign up for your [SAP Analytics Cloud Trial.](https://www.sap.com/products/technology-platform/cloud-analytics/trial.html)

3. A [Databricks workspace](https://docs.databricks.com/en/administration-guide/workspace/index.html) in any of the three supported hyperscalers
([AWS](https://aws.amazon.com/solutions/partners/databricks/),
[Azure](https://learn.microsoft.com/en-us/azure/databricks/marketplace/),
[GCP](https://cloud.google.com/databricks)) with a Databricks cluster. for cluster creation you can follow the article [Create a cluster](https://docs.gcp.databricks.com/clusters/configure.html).

## Exercises

- [Getting Started](exercises/ex0/)
- [Exercise 1 - Build and expose data views on SAP Datasphere](exercises/ex1/)
    - [Exercise 1.1 - Creating a view "Unified Sales Delivery View"](exercises/ex1#exercise-11-sub-exercise-1-description)
- [Exercise 2 - Creating a new analytical model for "Unified Sales Delivery View"](exercises/ex2/)
- [Exercise 3 - Create a Sales Order Management Dashboard on SAP Analytics Cloud](exercises/ex3/)
    - [Exercise 3.1 - Creating the Layout for the Sales Order Management Dashboard](exercises/ex3#exercise-31-creating-the-layout-for-the-sales-order-management-dashboard)
    - [Exercise 3.2 - Assigning the data from SAP Datasphere to Dashboard](exercises/ex3#exercise-32-assigning-the-data-from-sap-datasphere-to-dashboard)
- [Exercise 4 - Creating the Charts in Sales Order Management Dashboard for displaying Data](exercises/ex4/)
    - [Exercise 4.1 - Creating the first Chart for displaying **Short Qty per Sales Organization**](exercises/ex4#exercise-41-creating-the-first-chart-for-displaying-quantity-per-product-category)
    - [Exercise 4.2 - Creating another Chart for displaying **Monthly Case Fill- 12 Month Trend**](exercises/ex4#exercise-42-creating-another-chart-for-displaying-discount-per-product-category)
- [Exercise 5 - Creating the Table in Sales Order Management Dashboard for displaying Data](exercises/ex5/)
- [Exercise 6 - Creating **Input Controls** for the dashboard](exercises/ex6/)

## Contributing
Please read the [CONTRIBUTING.md](./CONTRIBUTING.md) to understand the contribution guidelines.

## Code of Conduct
Please read the [SAP Open Source Code of Conduct](https://github.com/SAP-samples/.github/blob/main/CODE_OF_CONDUCT.md).

## How to obtain support
Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2023 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
