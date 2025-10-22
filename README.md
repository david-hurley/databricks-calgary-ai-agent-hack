# Databricks Calgary AI Agent Hackathon - October 23 2025

In this hackathon, teams will use the [Alberta Water Well Information Database](https://www.alberta.ca/alberta-water-well-information-database) to create AI Agents in Databricks. Teams can explore the data on a map using the [Alberta Water Well Data Explorer](https://groundwater.alberta.ca/waterwells/d/). This map contains information on all drilled and tested water wells in Alberta. 

### Getting Started
1. Open your Databricks workspace
2. From the Workspace tab, select Create and choose Git folder
   <img width="1719" height="360" alt="image" src="https://github.com/user-attachments/assets/acf48aab-e09e-4eb0-be55-c1afefc0a767" />
3. Enter `https://github.com/david-hurley/databricks-calgary-ai-agent-hack.git` in the Git repository URL box and click Create Git Folder
4. You should now have a directory called `databricks-calgary-ai-agent-hack`
5. Navigate into the setup directory and open the `001-setup` notebook and select `Run all`, the play button in the top right - DO NOT MODIFY THIS NOTEBOOK
6. When the notebook is finished running, navigate to the Catalog tab and expand the `calgary_agent_hackathon` catalog and `alberta_water_well_data` schema. You should see the newly created tables.
   <img width="626" height="275" alt="image" src="https://github.com/user-attachments/assets/99bc8776-f711-4034-b6ec-e0d003cf6ee4" />
7. Navigate to the assets directory and download `Alberta Water Well Info.docx`. This document provides relevant dataset information and links.

### Some Ideas for AI Agents
**New Water Well Planning Agent:**

A user might ask `I am planning a new well on my property, can you help me create the plan?`. The Agent would:
1. search historical data for nearby drilled and tested wells
2. get the contact information of drilling companies that drilled the nearby wells
3. summarize the most common water bearing soil material and depths of material
4. get the typical pump intake depths and recommended flow rates
5. summarize any known water quality issues from nearby wells (i.e. exceedances)  

**Water Quality Risk Agent**

A user might ask `Should I be testing my well more frequently for water quality risks?`. The Agent would:
1. search test wells near the user
2. compile any known aesthetic and health releated risks from gas, bacteria, water quality, and isotope testing
3. provide a risk assessment for the users well

**Drilling Contractor Performance Agent**

A user might ask `What drilling companies near me have the best performance record?`. The Agent would:
1. get all in business drilling companies that have drilled wells nearby in the past
2. get information about nearby well water quality
3. get information about yield and completion quality (i.e. seal and screen placement)
4. group by drilling companies and create a scorecard

**Water Well PDF Processing and Verification**

Every drilled and test well has a associated PDF report. You could download a selection of these reports and build a Agent that would extract text from PDFs and verify extraction. This would emmulate a common use case of parsing unstructured documents and building verification.
1. parse the PDF to text or markdown
2. verify the field extraction against the existing table data

### Databricks AI Features 
- [Genie Spaces](https://docs.databricks.com/aws/en/genie/): get answers to questions using natural language. Genie converts text to SQL and understand data metadata and entity relationships
- [Unity Catalog Registered Functions](https://docs.databricks.com/aws/en/udf/unity-catalog): create SQL and Python functions, registered in Unity Catalog, and add as tools for LLMs
- [Playground](https://docs.databricks.com/aws/en/generative-ai/agent-framework/ai-playground-agent): attach tools to various LLMs to test Agents
- [Agent Bricks](https://docs.databricks.com/aws/en/generative-ai/agent-bricks/): no/low-code way to build Agents
- [AI SQL Functions](https://docs.databricks.com/aws/en/large-language-models/ai-functions): inline SQL functions to perform tasks such as natural language query, summarize, extract, and more
- [Spatial SQL Functions](https://docs.databricks.com/aws/en/sql/language-manual/sql-ref-st-geospatial-functions): toolbox of functions for doing spatial operations

### Data Terms of Use

**Terms of use**

**Non-commercial reproduction**

Unless indicated otherwise, the data contained in the repository may be copied and distributed for non-commercial use without charge or further permission from Government of Alberta Communications and Public Engagement. We only ask that: the data will not be modified, users exercise due diligence in ensuring the accuracy of the data, the Government of Alberta be identified as the source of the data, and the reproduction is not represented as an official version of the data reproduced, nor as having been made in affiliation with or with the endorsement of the Government of Alberta.

**Commercial reproduction**

The data contained in the repository may not be copied and/or distributed for commercial purposes without prior written permission from Government of Alberta Communications and Public Engagement.
