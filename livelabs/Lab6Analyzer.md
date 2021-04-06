<p align="center">
  <img src="https://ayankovs-ccp-s3.s3.eu-west-3.amazonaws.com/CiscoLiveLogo.jpg">
</p>

# Cisco Live HOLCCT-2108 Webex Contact Center Reporting - Analyzer Deep Dive
## Final Exercise 6 Bonus Lab


# Table of Contents
1. [Exercise 6.1 Personal Agent Statistics](#exercise-41-using-formulas-and-filters)
2. [Exercise 6.2 Threshold Alerting](#exercise-42-enhanced-field-compound-visualization-and-drill-down)
3. [Exercise 6.3 Scheduler](#exercise-42-enhanced-field-compound-visualization-and-drill-down)

**Quick Links**

* <a href="https://portal.wxcc-us1.cisco.com/portal" target="_blank">Portal</a>
* <a href="https://analyzer.wxcc-us1.cisco.com/analyzer/home" target="_blank">Analyzer</a>
* <a href="https://desktop.wxcc-us1.cisco.com" target="_blank">Agent Desktop</a>


## Lab Objective

This lab is designed to introduce you to the Agent Personal Statistics in Agent Desktop as well as setting Threshold Alerts and Scheduling Reports. 
**This lab was created as a single video with all listed elements.  Section videos will jump to the video position for the section**

### Pre-requisite

1. All previous labs completed is advisable but not required
2. Admin or supervisor credential with Analytics access in user profile
3. Make sure to make few test calls and answered by the agent the day you attempting this lab (to ensure we have some data to analyze)

# Exercise 6.1 Personal Agent Statistics

<iframe width="1024" height="576" src="https://youtube.com/embed/NBwnjKByJB4?rel=0" title="Exercise 6.1 Agent Personal Statistics" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Section Information
- `Agent Personal Statistics (APS)` are available on the Agent Desktop
- This section will show various features available with the APS on Agent Desktop

1. If not logged in to the Agent Desktop, open a new window and login to look at the current Agent Performance Statistics (APS)
2. Navigate through the available APS reports available in the Agent Desktop
3. See what options are available within the stock reports (shown in video)
4. Change the views by `filtering` or changing report `interval` periods
5. This exercise is designed to familiarize you with these options 

# Exercise 6.2 Threshold Alerting

<iframe width="1024" height="576" src="https://youtube.com/embed/NBwnjKByJB4?start=172" title="Exercise 6.2 Threshold Alerts" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Section Information
- `Threshold` Alerting can be set for various values in reports

1. Navigate to the Admin Portal and under the `hamburger` menu go to Threshold Rules
2. Create a new Threshold Rule
3. Threshold rules can be set according to Agent or Contact records.  Set the threshold as shown in the video for calls to your Team queue
4. Set the thresholds for this new rule to `number of calls in queue` and for simplicity set the threshold to 1 with interval at 120
5. Set your email address for the alert
6. Give the rule a name and save it
7. Test the new threshold with a call into the queue 
8. Check your email to see that you got the alert
9. In Analyzer check your threshold alerts and notice what options are available


# Exercise 6.3 Scheduler

<iframe width="1024" height="576" src="https://youtube.com/embed/NBwnjKByJB4?start=318" title="Exercise 6.3 Scheduler" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Section Information
- Setting up the Scheduler to run reports automatically

1. In Analyzer, look at the reports you created during this lab.  Choose a report you want to schedule.
2. In the video, report 3.3_CSR_ContactVolume report is chosen, however, which report you choose is up to you
3. Fill in the schedule information for the scheduled report
  - Note the options available at the top of this form
  - `Reoccurence` will allow you to set this job to run more than once
  - `Delete`, of course, allows you to delete a current job
5. Set the trigger to run a few minutes ahead so the report results can be seen
6. Once saved, check the details about the report you have scheduled by using the elipsis menu on that report `card`
7. If everything was setup correctly, check your email for the report
8. If your job was only set to run once, once it runs, that job is delted from the jobs list



# Congratulations - Cisco Live HOLCCT-2108 Lab Complete!

<p align="center">
<a href="https://user-images.githubusercontent.com/75790934/113780553-fe71f580-96f4-11eb-85c3-0fa7064794b5.gif" target="_blank">I Finished The Analyzer Lab!</a>
</p>

