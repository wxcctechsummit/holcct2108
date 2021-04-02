
<p align="center">
  <img src="https://ayankovs-ccp-s3.s3.eu-west-3.amazonaws.com/CiscoLiveLogo.jpg">
</p>

# Cisco Live HOLCCT-2108 Webex Contact Center Reporting - Analyzer Deep Dive <br>
## Exercises 1.1 to 1.3

# Table of Contents
1. Exercise 1.1: Dashboard reports
2. Exercise 1.2: Analyzer User Interface
3. Exercise 1.3: Access Control

**Quick Links**

* <a href="https://portal.wxcc-us1.cisco.com/portal" target="_blank">Portal</a>
* <a href="https://analyzer.wxcc-us1.cisco.com/analyzer/home" target="_blank">Analyzer</a>

## Lab Objective

This lab is designed to give you basic understanding of Analyzer, user interface features , how execute stock reports and use them to create custom reports per your need. In these videos the `lab goal` is familiarization of the product and terminology. 

We will also be creating two new reports (one for Call and one for agent) to capture relevent information and then will use these reports in a dashboard, while doing this we will learns about capabilities and features you can use to capture the required insights.

## Pre-requisite

1. All previous labs completed
2. Admin or supervisor credential with Analytics access in user profile
3. Make sure to make few test calls and answered by the agent the day you attempting this lab (to ensure we have some data to analyze)


# Exercise 1.1. Login into Analyzer and review dashboard reports

<iframe width="560" height="315" src="https://youtube.com/embed/Q4kf8dHN8x8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 
<br>
<br>
**Lab Section Information & Guide**
1. `Login to the WxCC portal` using the Portal link above.
2. Login using your provided student email and password.  Emails for this lab are always **cladmXuser@mailinator.com** where **X** is your student number.
3. The initial dashboard includes several `Realtime & Historical` reports showing current contact information in the system.
4. Navigate (shown in the video) through the various dashboard reports and the dropdown allowing you to see current information to familiarize yourself with these stock reports.
- Video Checkpoints
> * <a href="https://www.youtube.com/embed/Q4kf8dHN8x8?start=63" target="_blank">Entry Point Site Level Dashboard </a>
> * <a href="https://www.youtube.com/embed/Q4kf8dHN8x8?start=68" target="_blank">Contact Center Overview - Realtime Dashboard </a>
> * <a href="https://www.youtube.com/embed/Q4kf8dHN8x8?start=75" target="_blank">Contact Center Overview - Historical Dashboard </a>
> * <a href="https://www.youtube.com/embed/Q4kf8dHN8x8?start=85" target="_blank">Agent State Data - Realtime Dashboard </a>

5. `Navigate back to the Entry Point Site Level Dashboard` and complete some navigation exercises shown in the video
6. `Cross-Launch` from dashboard to a specific dashboard **Entry Point Historical Dashboard**
7. From the Cross-Launched dashboard - `Cross-Launch into Analyzer` to the specific table **Incomming, Short Contacts Entry Point** anf follow the instructions to set filters as desired.
> * <a href="https://www.youtube.com/embed/Q4kf8dHN8x8?start=3:12" target="_blank">Analyzer Incomming, Short Contacts Entry Point </a> <br>
8. This exercise completed

# Exercise 1.2 Analyzer User Interface
<iframe width="560" height="315" src="https://www.youtube.com/embed/xKoAPtAtXzo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  

**Lab Section Information & Guide**
1. `Login to the WxCC Analyzer` using the Analyzer link above
2. If already in Analyzer click on the `Home` icon to head back to the start screen of Analyzer
3. `Navigate` around the home screen learning the different features available on this screen
4. Select the `Visualization` icon to navigate to the Visualization repository
> * <a href="https://www.youtube.com/embed/E4Ch2gUSRi4?start=1:12" target="_blank">Visualization</a>
5. Use the `Search` box to find specific or groups of reports
6. Report information on card 2:46
7. Set preferred view characteristics 3:40
8. 

# Exercise 1.3 Access Control

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
