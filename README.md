# PMO_toolkit

# README 
### Free Project Management Templates
A free collection of Excel-based project management templates connected to Power BI, designed to help visualize project data more effectively. Some of the visuals such as risk and timeline reports are built using the Vega-Lite language through Deneb in Power BI.

Many of these templates are adapted from various online resources and enhanced for easier integration with Power BI. I’m sharing them here in hopes they help others streamline their project reporting and analysis. 
 
If you find any of these templates helpful, could you leave review on my [LinkedIn](https://www.linkedin.com/in/devon-locher/), I would greatly appreciate it.
 
 
# Project Risk Matrix (Deneb)
Project risk refers to any potential event, condition, or uncertainty that could negatively affect a project's objectives, timeline, resources, or outcomes. 
Risks are evaluated by examining two key dimensions:

   • Probability – How likely the risk is to occur
   
   • Impact – How severe the consequences would be if the risk occurs

Using these two factors, risks are plotted on a Risk Matrix, which provides a standardized way to categorize risk levels such as Sustainable, Moderate, Severe, and Critical. This helps teams visually identify which risks require immediate attention versus those that can be monitored.

 ![Risk Gif](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/Risk%20Matrix/Risk%20Matrix%20Gif.gif)

 ![Risk image](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/Risk%20Matrix/Risk%20Dashboard%20Image.png)
 
# Project Risk Matrix (Deneb)
Risk Matrix updated to display very low to very high.



 
# Business Continuity Risk Matrix (Deneb)
In a BCP risk matrix, the impact axis is driven by time tolerance, while the likelihood axis reflects disruption probability.
The key recovery metrics (MTD, RTO, RPO, WRT) define how long the business can withstand disruption before impact becomes unacceptable.

![BCP](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/BCP%20Risk%20Matrix/BCP%20Residual%20Risk%20Image.png)
 
# Gantt Chart (Deneb)
This Gantt chart is a modified version of the visual created by David Bacci - credit goes to him for the original work. I’ve updated it to work with my weekly gantt excel template, added support for extra sections, and made a few small tweaks to color and status categories. 

![gantt chart image](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/Gantt%20Chart/Gantt%20Chart%20Image.png)
 
# Project Timeline - Quarterly (Deneb)
A project timeline provides a visual overview of key events, milestones, and deliverables across the duration of a project. It displays important dates in chronological order – such as the project start, feature releases, major milestones, and final completion – allowing stakeholders to quickly understand the project’s progress and schedule expectations. 

 ![T](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/Timeline/Timeline.gif)
 
# Scoping Matrix
The PBI Matrix provides a structured and consistent framework for evaluating business process requirements across functional areas during system selection initiatives. It translates qualitative inputs – such as functional needs, system capabilities, project risk, and stakeholder alignment – into weighted quantitative scores, enabling objective comparison among solutions.

The model includes configurable scoring criteria, allowing the evaluation process to be tailored for different projects or scoping exercises. It also incorporates a roles – and-responsibilities section, which is transformed into a RACI matrix within Power BI for improved visibility and accountability.

Additionally, the matrix features a vendor response section that consolidates key requirements and questions sent to vendors prior to demonstrations. This area captures vendor feedback and tracks all project-related comments, supporting a transparent and well-documented decision-making process.
 
![s](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/Project%20Scoping%20Matrix/Matrix%20Assessment%20Image.png)
 
# RACI Matrix (Deneb)
A RACI matrix is a simple but powerful project-management tool used to clarify roles and responsibilities for tasks within a project or process. A RACI matrix is used to clearly define who is responsible for doing the work, who is accountable for final decisions, who must be consulted, and who should be kept informed. It helps reduce confusion, improve communication, and ensure accountability across tasks and teams.

![RACI](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/RACI%20Matrix/RACI.png)
 
# Stakeholder Register
The stakeholder register summarizes all project stakeholders, outlining their roles, levels of influence, interests, and communication requirements to support effective project engagement and decision-making.
  
![Stake](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/Stakeholder%20Register/Stakeholder%20Register%20Image.png)
 
# List.zip - How Dynamic Excel Worksheets Keep Power BI Reports Reliable
Excel is often where business data begins. Teams use it to collect project updates, budgets, operational details, and other information that eventually feeds Power BI reports.
That flexibility is useful - until a column name changes.
A small adjustment in Excel, such as changing “Owner” to “Document Owner,” can interrupt a Power BI refresh or leave a report without the expected information. The issue is not the new name itself. The issue is that reports depend on consistent structure.
A dynamic worksheet-mapping approach helps solve that problem.

### A controlled bridge between Excel and Power BI

Instead of making Power BI depend directly on the changing column names in an Excel worksheet, a simple mapping table defines how source columns should be interpreted.
The table identifies:

•	The column name currently used in Excel.

•	The stable name Power BI should use.

•	The data type the report expects.

This gives business users a supported way to make limited source changes while preserving the structure used by the report.
For example, if an Excel header changes from “Owner” to “Document Owner,” the mapping can tell Power BI to continue treating that field as “Owner.” The report’s measures, visuals, and downstream logic can remain stable.
### Where `List.Zip` fits
Behind the scenes, Power Query uses `List.Zip` to pair related pieces of information by position. It can pair an Excel source name with a Power BI name, or pair a column with the data type it should receive.
That capability makes the mapping table dynamic. Rather than rewriting transformation logic each time a supported column change occurs, Power Query reads the mapping table when the report refreshes.
The result is a more maintainable process:
•	Users can make approved changes in Excel.
•	Report developers retain stable model logic.
•	Changes are easier to trace and review.
•	Routine adjustments do not automatically become support tickets.

### Flexibility still needs guardrails

Dynamic does not mean uncontrolled.
A mapping table should use approved data types, require complete entries, and clearly identify mappings that no longer match the source file. It should also preserve a clear distinction between the Excel header and the stable field name used by Power BI.
That balance matters. Excel remains flexible for the people closest to the data, while Power BI remains reliable for the people making decisions from it.
### A better operating model for Excel-based reporting
This approach is particularly useful when Excel is a legitimate business input - not just a temporary workaround.
By treating the mapping table as a controlled interface, organizations can reduce refresh failures, protect report logic, and make ownership clearer between data contributors and report developers.
The goal is simple: allow change where it is needed, without allowing small spreadsheet edits to disrupt trusted reporting.



# Data Dictionary – (bonus!)
Each report includes a built-in Data Dictionary: a simple reference that explains the report’s measures, fields, tables, and relationships. It helps users understand what the data means, how key metrics are defined, and how to interpret the report with confidence.

The Data Dictionary stays aligned with the Power BI model as it evolves, supporting consistent definitions, easier knowledge transfer, and long-term maintainability. Rather than relying on external spreadsheets or tribal knowledge, this data dictionary is generated directly from the model itself, ensuring it stays aligned with the current state of tables, columns, measures, and relationships.


![Data](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/Data%20Dictionary/Data%20Dictionary%20Image.png)


### 🔑 Keywords & Tags
**Project Management:**
#PMOToolkit #ProjectManagementOffice #ProjectManagementTemplates #FreeProjectManagementTemplates #PowerBITemplates #ExcelProjectManagement #OpenSourcePM #ProjectReporting 

**Risk Management:**
#RiskMatrix #RiskHeatmap #RiskAssessment #ProbabilityImpact #RiskManagement #CriticalRisks #ProjectRisk #ProjectGovernance 

**Scoping Matrix**
#ScopingMatrix #RequirementsMatrix #SystemEvaluation #VendorSelection #SystemSelection #SystemComparison #VendorComparison #RequirementsGathering #WeightedScoring #RACIMatrix #StakeholderAnalysis #ProcurementPlanning

**Planning & Analysis:**
#RolesAndResponsibilities #StakeholderRegister #StakeholderAnalysis #TeamAccountability #ScopingMatrix #RequirementsMatrix

**Scheduling:**
#GanttChart #ProjectSchedule #ProjectTimeline #MilestoneTracker #ProjectPlanner

**Data Management:**
#PowerBIDashboard #PowerQuery #DataDictionary #PowerBISemanticModel #PowerBIModel #DataDocumentation #OpenSource

**Business Continuity Planning:**
#BusinessContinuity #BCP #BusinessImpactAnalysis #OperationalRisk #DisasterRecovery #MTD #RTO #RPO #BusinessContinuityPlanning #OperationalResilience #ComplianceReporting

**Technical Info:**
#Deneb #VegaLight #Vega #CustomVisual #PowerBICustomVisual
