# Projects Portfolio Dashboard & Analytics

A **Power Platform projects portfolio management and analytics solution** built with **Microsoft Dataverse, Model-driven Apps, and Power BI**.

The solution allows project information to be managed in Dataverse and analyzed through an interactive Power BI report.

![Portfolio Overview](/Power-BI-Dashboards/Projects%20Portfolio/images/page1.png)

## Tech Stack

* **Microsoft Dataverse** - Project data storage
* **Power Apps Model-driven App** - Project management
* **Power BI** - Analytics and visualization
* **Power Query** - Data transformation
* **DAX** - Calculations and dynamic reporting
* **GitHub** - Project documentation and version control

## Solution Architecture

```text
Model-driven App
       ↓
   Dataverse
       ↓
   Power Query
       ↓
    Power BI
       ↓
┌───────────────────────┐
│ Portfolio Overview    │
│ Project Explorer      │
│ Project Details       │
└───────────────────────┘
```

## Key Features

* Centralized project management using Dataverse
* Model-driven App for entering and managing projects
* Interactive Power BI portfolio dashboard
* Project filtering by:

  * Primary Technology
  * Complexity
  * Data Source
* Project type and complexity analysis
* Platform usage analysis
* Data source analysis
* Project duration tracking
* Project-level drill-through
* Dynamic technology logos
* Dynamic GitHub and demo links
* Conditional technical details based on project type

## Power BI Pages

### 1. Portfolio Overview

Provides a high-level view of the project portfolio, including:

* Total Projects
* Completed Projects
* Projects In Progress
* Average Duration
* Projects by Technology
* Projects by Type & Complexity
* Top Platforms
* Projects Over Time
* Common Data Sources

![Portfolio Overview](/Power-BI-Dashboards/Projects%20Portfolio/images/page1.png)

---

### 2. Project Explorer

Allows users to explore and filter individual projects before opening the detailed project view.

![Project Explorer](/Power-BI-Dashboards/Projects%20Portfolio/images/page2.png)

---

### 3. Project Details

A drill-through page providing detailed information about the selected project.

Includes:

* Project description
* Primary technology
* Status
* Complexity
* Project type
* Timeline
* Duration
* Tools used
* Technical details
* GitHub repository
* Live demo

![Project Details](/Power-BI-Dashboards/Projects%20Portfolio/images/page3.png)

## Data Model

The main project table contains one record per project.

A separate mapping table is used for projects with multiple platforms:

```text
fm_project
     │
     │ 1 : *
     ↓
ProjectPlatforms
```

Example:

| Project Name | Platform   |
| ------------ | ---------- |
| Project A    | Power Apps |
| Project A    | SharePoint |
| Project A    | Dataverse  |

This allows platform usage to be analyzed independently while maintaining the relationship with the main project table.

## DAX & Data Modeling

The project uses DAX for:

* Project counts
* Project duration
* Average duration
* Conditional technical fields
* Dynamic project information
* Portfolio-wide calculations

Power Query is used to transform Dataverse multi-select fields and create normalized mapping tables.

## Project Resources

Each project can contain its own:

* GitHub repository URL
* Demo URL

These are stored in Dataverse and used as dynamic links on the Project Details page.

## What This Project Demonstrates

* Dataverse data modeling
* Model-driven App development
* Power BI dashboard development
* Power Query transformations
* DAX
* Data relationships
* Drill-through
* Interactive filtering
* Dynamic content
* Power Platform integration
* Dashboard UI/UX design


## Key Skills Demonstrated

This project demonstrates practical experience with:
```text
Microsoft Power Platform
├── Dataverse
├── Model-driven Apps
│
Power BI
├── Power Query
├── DAX
├── Data Modeling
├── Relationships
├── Drill-through
├── Interactive Filtering
├── Conditional Formatting
└── Dashboard Design

```
