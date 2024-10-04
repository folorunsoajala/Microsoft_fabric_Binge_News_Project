# Life After DP-600 Associate Exam: A Journey through the Binge News Project
![](archieteture.png)

## Project Overview
After successfully completing the DP-600 exam, this project serves as a hands-on exploration of advanced data handling using Microsoft Azure and Fabric. The objective of the Binge Project is to set up a fully functional data pipeline that ingests, transforms, and visualizes real-time data, while applying incremental loading and performing sentiment analysis. This documentation serves as your roadmap through each stage of the project, helping you understand not just the how, but also the why behind each task.
watch introductory video [here](https://youtu.be/okrKwdn9Z34?si=H4GwhOyB-hIM-MRB)

![](Project_guide.png)

## Creating a Binge Resource in Azure
My journey begins with setting up a Binge resource on the Azure Portal. This acts as the foundation for managing all resources and processes needed for the project.
- Step 1: Navigate to Azure Portal and sign in using your Azure subscription account.
- Step 2: Create a new resource group. This group will serve as the umbrella for all resources related to this project, ensuring centralized management and easy monitoring.

![](Binge_resourece_group.png)

Next, head to the Azure Marketplace to create a Bing Search API. The Bing Search API will provide access to real-time news data, which will be central to our sentiment analysis.
- Step 3: In the Marketplace, search for Bing Search v7 and follow the prompts to set it up.
With these foundational resources in place, we move on to Microsoft Fabric to set up a workspace and data Lakehouse, which will store and process the ingested data.
watch the environment set-up video [here](https://youtu.be/JywiK_EPsgE?si=Tp7QZA_qs0OEqfiJ)

![](Binge_search_v7.png)

## Data Ingestion with Microsoft Fabric

Once my  Lakehouse is ready, the next step is to ingest data into it using Microsoft Fabric’s data pipeline.
- Step 1: Create a data pipeline workspace in Fabric.
- Step 2: In the pipeline, connect to the Bing Search API to fetch US 2024 election news using the Copy Data activity.
The data source will be the REST API, and the destination will be the Lakehouse created earlier. Set the data format as JSON to store the news articles in a file section of the Lakehouse.
- Step 3: After configuring the API and data destinations, save and run the pipeline to ingest the data into the Lakehouse.


