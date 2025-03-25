# **Table of Contents:**


## Task - Call Centre Trends Analysis
Visualizing customer and agent behavior Create a dashboard in Power BI for Call Centre Manager that reflects all relevant Key Performance Indicators (KPIs) and metrics in the dataset.<br><br>

**:red_circle:<b> Problem Statement : </b>**

The purpose of this analysis is to create a dashboard in PowerBI for call canter manager that reflects all relevant Key Performance Indicators (KPIs) and metrics in the dataset.<br><br>

**:red_circle: <b>The KPI which are included in this dashboard are </b> :**

• Overall customer satisfaction

• Overall calls answered/abandoned

• Calls by time

• Average speed of answer

• Agents performance quadrant i.e. average handle time(talk duration) vs calls answered <br><br>

**:red_circle:<b> Flow of work : </b>**

**Step :one:- Upload Data**

The Dataset used for this analysis was presented by PWC_Switzerland... :link:[ Link ](https://cdn.theforage.com/vinternships/companyassets/4sLyCPgmsy8DA6Dh3/01%20Call-Center-Dataset.xlsx)

**Step :two:-Cleaning data**

Data transformation was done in Power Query, and the dataset was loaded into Microsoft Power BI Desktop for modelling. The call canter dataset is given by a table named Call Center which has 10 columns and 5000 rows of observation

The tabulation below shows the Call center table with its column names and their description:

| Column Name | Description |
|--- | --- |
| Call Id | Represents every unique observation in the dataset |
| Agent | Describes the name of the agent |
| Date | Describes the date of the call |
| Time | Represents the time of the call |
| Topic | Describes the topic of the caller |
| Answered | (Y/N) Describes if the call was Answered or not |
| Resolved | Describes if the problem was Resolved or not |
| Speed of answer(in seconds) |	Represents the speed of answer in seconds|
| AvgTalkDuration	| Represents the average talk duration of call |
| Satisfaction rating |	Represents the satisfaction rating of the agent during the call |<br>

**Step :three:-Transform data**

Data Cleaning and transformation for the dataset were done in power query as follows: 

• Unnecessary columns were removed <br>
• Each of the columns in the table was validated to have the correct data type <br>
• Unnecessary rows were removed <br>

**Step :four:-Data Visualization**

Data visualization for the datasets was done in Microsoft Power BI Desktop: 

The Call Center Manager Page Shows KPIs including overall customer satisfaction, overall calls answered/abandoned, calls by time, average speed of answer, agents performance quadrant i.e. average handle time(talk duration) vs calls answered

**Step :five:-Data Analysis**

Measures used in visualization are:

• %TotalCallsAnswered = DIVIDE([CallsAnswered],COUNT('Call Center Data'[Call Id]))

• CallsAnswered = CALCULATE(COUNT('Call Center Data'[Answered (Y/N)]),'Call Center Data'[Answered (Y/N)]="Y")

• CallsMissed = CALCULATE(COUNT('Call Center Data'[Answered (Y/N)]),'Call Center Data'[Answered (Y/N)]="N")

• IssueResolved = CALCULATE(COUNT('Call Center Data'[Resolved]),'Call Center Data'[Resolved]="Y")

