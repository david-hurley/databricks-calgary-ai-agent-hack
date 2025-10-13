# Databricks Calgary AI Agent Hackathon - October 23 2025

In this hackathon, teams will use the [Alberta Water Well Information Database](https://www.alberta.ca/alberta-water-well-information-database) to create AI Agents in Databricks. Teams can explore the data on a map using the [Alberta Water Well Data Explorer](https://groundwater.alberta.ca/waterwells/d/). This map contains information on all drilled and tested water wells in Alberta. 

### Getting Started
1. Open your Databricks Free Edition workspace
2. From the `workspace` tab, select `create` and choose `git folder`
3. Enter `https://github.com/david-hurley/databricks-calgary-ai-agent-hack.git` in the Git Repository URL box and click `Create Git Folder`
4. Navigate into the newly created `databricks-calgary-ai-agent-hack` folder and into `setup`
5. Open the `001-setup` notebook and `run all`, the play button in the top right - do not modify this notebook
6. When the notebook is finished running, navigate to the `Catalog` tab and into `calgary_agent_hackathon.alberta_well_water_data` - you should see all of the newly created tables
7. Refer to `assets/Alberta Water Well Info.docx` for information about each table such as column descriptions and entity relationship diagrams

### Some Ideas for AI Agents
- **New Water Well Planning Agent:**
    
    A user might ask `I am planning a new well on my property, can you help me create the plan?`. The Agent could:
    1. search historical data for nearby drilled and tested wells
    2. get the contact information of drilling companies that drilled the nearby wells
    3. summarize the most common water bearing soil material and depths of material
    4. get the typical pump intake depths and recommended flow rates
    5. summarize any known water quality issues from nearby wells (i.e. exceedances)  

ADD MORE

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
Unless indicated otherwise, this website (and materials on it) may be copied and distributed for non-commercial use without charge or further permission from Communications and Public Engagement. We only ask that:
the materials will not be modified,
users exercise due diligence in ensuring the accuracy of the materials,
the Government of Alberta be identified as the source of the materials, and
the reproduction is not represented as an official version of the materials reproduced, nor as having been made in affiliation with or with the endorsement of the Government of Alberta.

**Commercial reproduction**
This website (and materials on it) may not be copied and/or distributed for commercial purposes without prior written permission from Communications and Public Engagement.

### Acknowledgement
Thanks to Ryan Bondyra for requesting access and permission and collating the Alberta Water Well dataset
