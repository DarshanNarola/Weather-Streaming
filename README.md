# Real-Time Weather Reporting System

## Overview
This project builds a **real-time weather reporting system** using live weather data. The pipeline ensures secure key storage, efficient data ingestion, and streaming capabilities.

## Architecture
The data flow is as follows:

1. **Weather API** - Fetches real-time weather data.
2. **Azure Key Vault** - Securely stores API keys.
3. **Azure Databricks** - Processes weather data for analytics.
4. **Azure Event Hub** - Streams the processed data for downstream consumers.

### Visual Representation
![Architecture Diagram](https://github.com/user-attachments/assets/e399f393-c41e-46c4-b226-ef9c2de01ceb))

## Technologies Used
- **Weather API**: Provides live weather data.
- **Azure Key Vault**: For securely storing and managing API keys.
- **Azure Databricks**: Handles data ingestion and analytics.
- **Azure Event Hub**: Facilitates real-time streaming.

## Prerequisites
- Azure Subscription
- Databricks Workspace
- Event Hub Namespace and Event Hub
- Weather API Access Key

## Setup Instructions

### Step 1: Weather API Setup
1. Sign up for a Weather API account.
2. Retrieve your API key.

### Step 2: Configure Azure Key Vault
1. Create an **Azure Key Vault** instance.
2. Store the Weather API key securely in Azure Key Vault.

### Step 3: Azure Databricks
1. Set up an Azure Databricks Workspace.
2. Use **Secrets Scope** in Databricks to access the Key Vault secrets.

### Step 4: Azure Event Hub
1. Create an Event Hub Namespace and Event Hub.
2. Configure the connection string.

### Step 5: Implement the Pipeline
1. Fetch data using Databricks (via the Weather API and Key Vault).
2. Stream processed data to Azure Event Hub.

## Execution
1. Run the Databricks notebook to fetch, process, and stream data.
2. Verify data in the Event Hub.

## Conclusion
This system ensures **secure key management**, scalable data processing, and real-time data streaming.
