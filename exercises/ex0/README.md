# Discover - Understand SAP Datasphere and Databricks setup and given data models

> **IMPORTANT**: This section is for informational purposes only and does not require any actions to be taken by the participants. Its aim is to provide a better understanding of the preconfigurations. The goal is to provide a clear understanding of the concepts and techniques involved, without the need for any hands-on implementation.

## Role of SAP Business Technology Platform (SAP BTP)
 - With SAP Datasphere, customers can federate queries across source systems (SAP and Google) without the need for data replication. 
 - SAP Analytics Cloud (SAC) customers can execute live on the fly analysis across cross-cloud data sources in real-time (and live analytics to SAP HANA systems).
 - Unified SAP data model and semantics propagated from SAP S/4HANA and SAP CX systems to SAP Datasphere and SAC

## Role of Databricks
 -  Serve as a powerful data processing and ETL (Extract, Transform, Load) platform to prepare the data for analytics. ​
 - Perform real-time processing on incoming data streams from SAP Datasphere.​
 - Store the processed data in a suitable format, such as Delta Lake, which is optimized for both batch and real-time processing.​
 - Optimize query performance through features like query optimization and caching to make real-time analytics in SAP Analytics Cloud responsive and efficient.​

In this hands-on session, you will work with a sample Databricks dataset. 
To analyze sales order management you can combine external source systems like Databricks and federate data from it to get real-time data.

To achieve this we have created data sets of Databricks. In Databricks, data sets are pre-loaded and publicly accessible data sets. You can use them to develop and test your queries, and/or gain insights into a variety of topics.

## Databricks Model Overview
​![databricks tables](./images/deltalake.png)

## SAP S/4HANA Sample Sales Data loaded in SAP Datasphere
​![ds tables](./images/dstables.png)

## Overview - Establishing live data integration between Databricks and SAP Datasphere
// TODO

## Solution Overview

The architecture below highlights the main purpose of this integration, federating data residing in Databricks delta lake into SAP Datasphere. ​
We do this to achieve richer analytics by incorporating data that would otherwise remain unused in 3rd party systems with the already valuable insights delivered by SAP data. ​
We show the different mechanisms by which data can be federated and used in SAP Analytics Cloud without being replicated.​

​![Final View](./images/architecture.png)

## Summary

The goal of this introduction was to give a clear understanding of the concepts and techniques involved in creating a Datasphere live data connection to Google BigQuery and exploring the provided data model. 

Continue to - [Exercise 1 -  Build and expose data views on SAP Datasphere](../ex1/README.md)
