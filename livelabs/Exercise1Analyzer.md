---
title: "Exercise 1: Intro and UI"
---

# Webex Contact Center Reporting - Analyzer

# Table of Contents

- [1. Login into Analyzer and review user interface](#1-login-into-analyzer-and-review-user-interface)
- [2. Execute Stock Report and use it to create custom reports](#2-execute-stock-report-and-use-it-to-create-custom-reports)
- [3. Create an Agent Historical Call Visualization](#3-create-an-agent-historical-call-visualization)
- [4. Create a Call Realtime Report](#4-create-a-call-realtime-report)
- [5. Create Dashboard](#5-create-dashboard)

**Quick Links**

* [Portal](https://portal.wxcc-us1.cisco.com/portal)
* [Analyzer](https://analyzer.wxcc-us1.cisco.com/analyzer/home)

# Introduction
<iframe width="560" height="315" src="https://www.youtube.com/embed/453BlLMFetU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

## Lab Objective

This lab is designed to give you basic understanding of Analyzer, user interface features , how execute stock reports and use them to create custom reports per your need.  

We will also be creating two new reports (one for Call and one for agent) to capture relevent information and then will use these reports in a dashboard, while doing this we will learns about capabilities and features you can use to capture the required insights.

## Pre-requisite

1. All previous labs completed
2. Admin or supervisor credential with Analytics access in user profile
3. Make sure to make few test calls and answered by the agent the day you attempting this lab (to ensure we have some data to analyze)


# 1. Login into Analyzer and review user interface

<iframe width="560" height="315" src="https://www.youtube.com/embed/E4Ch2gUSRi4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 


**Section Information**
- Login Into Analyzer 
- Four Repositories
- Review Stock reports and Dashboard
- Search Folder & Visualization
- List or Grid View
- Visualization Summary information
- Report Details information

1. Click on the `Burger` sign next to `HOME`
2. You can see 3 modules on the left pane : `Visualization , Dashboard and Variables`
3. In the middle of the page you would notice 4 Repositories : `Total Agent Activity Records, Total Agent Session Records, Total Customer Activity Records and Total Customer Session Records`
4. Click on More details on Total Customer Session Records: Make a note of `total` customer sessions records and `period`  those records were executed
5. Click on `Visualization`: you will notice `Stock Reports` Folder , Click on `Stock reports --> Business Metrics`
6. Click on `GRID` option on left upper side (under the user name), this will show you reports in GRID view 
    Make a note of `Type, Temporal Scope, Last Modified , Created By and ID`
7. Click on Search `Folder & Visualization` and enter `Agent realtime`
    This is execute a global search and list the matching report





# 3. Create an Agent Historical Call Visualization 

<iframe width="560" height="315" src="https://www.youtube.com/embed/xKoAPtAtXzo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  

**Section Information**
- Create a Historical Agent report
- Repository and Interval Selection
- Using Measures and Profile Variables
- How to use Enhanced Field
- How to creat new Formulas


1. Go to `Home --> Visualization` and Click on your `Folder` created in previous excercise.
2. Click on `Create New` --> `Visualization`
3. On the top pane Click next to `Type` and select `Agent Session Record`
4. On left pane click next to `Start Time` and select `Last 7 Days`
5. Click on `Compute` and select under `Interval` Daily
6. Click on `+ Row Segment`, search for Field `Agent`. Select `Agent Name` and drag it to `Row segment` area (Green color pane)
7. Click on `Interval` on `Column Segment` and drag it to `Row Segment` under `Agent Name`
8. Click on `+ Profile Variable` , search for `connected` and click on `Measure` drop-down. Select `Connected Count` and drag it to `Profile Variable` pane (Green). Here click on `Formula`  and select `Sum of Connected Count`, change the name to `Inbound Calls` and Click `Save`
9. Repeat `step 7` and drag `Outdial Connected Count` and Save `Sum of Outdial Connected Count` as `Outdial Calls`
10. Click `Save` option on the top pane
11. Name the report as `Agent Call Volume Last7Days`  and click `OK`
12. Click on `Preview`, You can see `Calls handled (Inbound and Outbound)` by all the agents for `last 7 days.`
13. Lets see how can we leverage `Enhanced Field` to create Grouping of `Segment fields`.
14. Go to `Edit view` of the report, right click on the `Agent Name` and click on `Create Enhanced Field`
15. Change the `Name` to `LOB_{YourNameInitial}`, Type `Default` in `Default Group` 
16. In `Group` configure `Group Name` as `Sales` and select your `agent` in `Provide Value`  and `Save` it
17. Now move the newly created `Enhanced field` above `Agent Name` by click and drag in the segment section.
18. Now this `Enhanced field` can be saved to use globally in other reports by `right click` on the field and click `SAVE`  and `SAVE`.
18. `Save` the report and `Preview`: You will see `Enhanced Field` in first column : `Default` and `Sales` with your agent assigned under `Sales` and rest of the agents under `Default`.
19. Lets see how we can create `Custom formula`: In this case we would like to get a field which give us `total number of calls handled by the agent including inbound and outbound`.
20. Go to the `report edit view` and right Click on `Inbound Call`--> `click New Formula`
21. Name the formula as `Total Agent Call_{YourNameInitial}`
22. In Arithmetic Expression Use `Inbound Call + Outdial Calls` (Click the down arrow to see the field) and `Save`
23. This Formula can be saved for global use in other reports, to do so `right click` on the newly created formula variable and click `save` and then `OK`
23. `Save` the report and `Preview`, this will add new column providing you `Total number of calls`
