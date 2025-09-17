# Gather data

## Backstory
Currently Fabrikam’s data estate and pipelines are heavily fragmented. Hack your way to bring data from disparate sources and unify them in RTI. Using various connectors available in Eventstream, you can get data from streaming sources, and CDC from databases. Rich transformations are possible within Eventstream to cleanse and transform the data. Schema registry allows you to setup a robust and resilient streaming pipeline that can respond to changing schemas.

## Setup
For running this Act, 
1. You will need Eventstream, Eventhouse and Azure blob storage. 
2. Use the attached "Manufacturing Simulator" notebook to generate manufacturing/production data. The notebook will generate data and push it to an Eventstream that you can configure. 
3. Assets, Operators and Sites data will be generated in the Lakehouse.
4. Use the attached "Shipping Simulator" notebook to generate shipping data. The notebook will generate data and push it to an Azure blob storage that you can configure. 
5. Assets, Operators and Sites data is available in the Lakehouse.

## Challenges 

### 1. Enrich Manufacturing data with AnomalyFlag column and datatype changes
    Hint: Use SQL transformation on DefectProbability  column in stream – DefectProbability>0.1 = Anomaly.
    Hint: SQL Operator by default works only if there are no other operators in this stream. Can a DerivedStream help?
    Hint: Keep all fields excepts the last 3: EventProcessedUtcTime, PartitionId, EventEnqueuedUtcTime

### 2. Ingest Manufacturing data
Assets, Operators, and sites are static data you need refer from Lakehouse
Production data that is streaming from Eventstream.

    Hint: Use accelerated shortcuts for static data

## 3. Ingest Shipping data
Shipping events are pushed to an Azure blob storage in real-time

    Hint: Use Continuous ingestion from Azure Storage
Shipping provider details from GitHub assets

    Hint: Use Local file ingestion method

## 4. Ingest Customer and Products data 
Both of these static data is present in a SQL database
    Hint: Use Azure SQL CDC connector

## 5. Make weather data available to all Fabrikam distributors and setup hourly alerts for US region
    Hint: Create derived stream
    Hint: Use Activator alerts on temperature


