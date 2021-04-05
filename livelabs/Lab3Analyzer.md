<p align="center">
  <img src="https://ayankovs-ccp-s3.s3.eu-west-3.amazonaws.com/CiscoLiveLogo.jpg">
</p>

# Cisco Live HOLCCT-2108 Webex Contact Center Reporting - Analyzer Deep Dive
## Exercises 3.1, 3.2 and 3.3

# Table of Contents
1. [Exercise 3.1 - Create Realtime Contact Report](#exercise-31---create-realtime-contact-report)
2. [Exercise 3.2 - Create Realtime Agent Report](#exercise-32---create-realtime-agent-report)
3. [Exercise 3.3 - Create Chat Reports with Interval](#exercise-33---create-chat-reports-with-interval)

**Quick Links**

* <a href="https://portal.wxcc-us1.cisco.com/portal" target="_blank">Portal</a>
* <a href="https://analyzer.wxcc-us1.cisco.com/analyzer/home" target="_blank">Analyzer</a>
* <a href="https://desktop.wxcc-us1.cisco.com" target="_blank">Agent Desktop</a>

## Lab Objective

This lab is designed to dig deeper into Analyzer and rather than copying and editing stock reports, the attendee will create new and custom reports.  These reports will be used in subsequent labs to build upon as well so it is important to finish this lab prior to moving on to the next lab.

## Pre-requisite

1. All previous labs completed is advisable
2. Admin or supervisor credential with Analytics access in user profile
3. Make sure to make few test calls and answered by the agent the day you attempting this lab (to ensure we have some data to analyze)


# Exercise 3.1 - Create Realtime Contact Report  
<iframe width="1024" height="576" src="https://youtube.com/embed/n4qAwwhuTmg?rel=0" title="Exercise 2.1 Execute Stock Reports" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


**Section Information**
- Set User Profile back to All Entry Points
- Create a new visualization for Realtime Contacts

1. Prior to starting the lab exercise, navitate to the user profile and return your user access for Entry Points to `All`
2. Navigate to Analyzer and `Create` a new report visualization that will be saved in your personal directory.
> * [Create New Visualization](https://www.youtube.com/embed/n4qAwwhuTmg?start=101)
3. This will be a Realtime report so select the appropriate value under `Compute` on the left side of the screen
4. Follow the video instructions to add the `14` values to the report
5. `Save` The new report to your directory as `3.1_CSR_Contacts`
6. This completes your first custom report

# Exercise 3.2 - Create Realtime Agent Report

<iframe width="1024" height="576" src="https://youtube.com/embed/IiA0RYmgoIE?rel=0" title="Exercise 2.1 Execute Stock Reports" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


**Section Information**
- Create a new AAR Agent Activity Realtime Report

1. Create a new visualization in Analyzer as an `Agent Activity Record`
2. Set this report as a Realtime Report with a Snapshot refresh rate of 3 seconds
3. Follow the video guide to add the reporting element columns 
> * [Add New Column Data](https://www.youtube.com/embed/IiA0RYmgoIE?start=88)
4. Once done, `Save` the new report as `3.2_AAR_AgentState`
5. `Review` the report by doing a preview and if all is good, this exercise is complete
6. Move to the next and last exercise


# Exercise 3.3 - Create Chat Reports with Interval
<iframe width="1024" height="576" src="https://youtube.com/embed/t_Ub0xGfG0s?rel=0" title="Exercise 2.1 Execute Stock Reports" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


**Section Information**
- Create a new `Chart View` historical report for Total Calls and Abandoned Calls

1. Create a new visualization using CSR report data. `CSR is Customer Session Record`
2. Set this as a `Monthly` report
3. Follow the instructions in the video to complete the fields.  `This will be a Line Chart`
4. When done, save this chart as `3.3_CSR_ContactVolume`
5. This section is done.  When complete, move to Lab 4.

## Next Lab is Lab 4: Advanced Insights
> * [Analyzer Lab 4 Link](https://wxcctechsummit.github.io/holcct2108/livelabs/Lab4Analyzer.html)

[Back to top](#cisco-live-holcct-2108-webex-contact-center-reporting---analyzer-deep-dive)
