# PMO_toolkit

# README 
A collection of Excel-based project management templates connected to Power BI, designed to help visualize project data more effectively. Some of the visuals such as risk and timeline reports are built using the Vega-Lite language through Deneb in Power BI.

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
 
# Data Dictionary – (bonus!)
The reports includes a Data Dictionary that documents the Power BI semantic model using Power BI’s system metadata (INFO.VIEW ). The goal is to provide transparent, always-up-to-date documentation of the dataset to reduce technical debt, improve knowledge transfer, and support long-term maintainability.

![Data](https://github.com/DL0K-pbi/PMO_toolkit/blob/main/Data%20Dictionary/Data%20Dictionary%20Image.png)
