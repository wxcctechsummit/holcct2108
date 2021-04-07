<p align="center">
  <img src="https://ayankovs-ccp-s3.s3.eu-west-3.amazonaws.com/CiscoLiveLogo.jpg">
</p>

# Cisco Live HOLCCT-2108 Webex Contact Center Reporting - Analyzer Deep Dive
## Exercises 5.1 and 5.2


# Table of Contents
1. [Exercise 5.1: Stock Dashboards](#exercise-51-stock-dashboards)
2. [Exercise 5.2: Custom Dashboards](#exercise-52-custom-dashboards)

**Quick Links**

* <a href="https://portal.wxcc-us1.cisco.com/portal" target="_blank">Portal</a>
* <a href="https://analyzer.wxcc-us1.cisco.com/analyzer/home" target="_blank">Analyzer</a>
* <a href="https://desktop.wxcc-us1.cisco.com" target="_blank">Agent Desktop</a>


## Lab Objective

This lab is designed to introduce you to the dashboards available in Analyzer.  Dashboards are available for Historical, Realtime and Business Metrics.  

### Pre-requisite

1. All previous labs completed is advisable but not required
2. Admin or supervisor credential with Analytics access in user profile
3. Make sure to make few test calls and answered by the agent the day you attempting this lab (to ensure we have some data to analyze)

# Exercise 5.1 Stock Dashboards
![Banner](https://user-images.githubusercontent.com/81705459/113801810-2f672000-971f-11eb-9f4d-cfa9bc9c72cb.jpg)

<iframe width="1024" height="576" src="https://youtube.com/embed/quuS5xrsmgI?rel=0" title="Exercise 5.1 Stock Dashboards" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Section Information
- Navigate some stock dashboards
- Create a dashboard from a stock dashboard

1. Navigate the Analyzer directory structure and discover the `Dashboards` directory
2. Dashboards are catagorized under the following types.  Historical, Realtime and Business Metrics.

![dashboards](https://user-images.githubusercontent.com/75790934/113645373-60c2eb80-964c-11eb-939f-fbbcbcb71608.png)

3. Under Business Metrics, run the `Abandoned Contacts` dashboard.  This dashboard is able to be a mash-up dashboard using data from other systems like UCCE and UCCX.
4. Under this dashboard there are several different types of data reports.  Take some time to familiarize yourself with them.
5. Expand the `Customer Journey` dashboard and familiarize yourself with how this report makes use of mouse overs to track the different abandoned contacts
6. Navigate back to the main dashboard directory and open a dashboard named `Contact Volume Historical Dashboard` under the Multimedia directory.
> * <a href="https://youtube.com/embed/quuS5xrsmgI?start=201" target="_blank">Start at timestamp</a>
7. Create a copy of this dashboard and edit to make some changes
8. Remove the `Contact Volume` dashboard component
9. Find the report created in Lab 4.2 called `4.2.1_CSR_QueueStatus` and drag that into the dashboard
10. Save this report as `5.1_Contact_Volume_Queue_Dashboard` and run it
11. This concludes this section.  Onto the next.

# Exercise 5.2 Custom Dashboards
![Banner](https://user-images.githubusercontent.com/81705459/113801857-4574e080-971f-11eb-990c-80a1c89ef2ef.jpg)

<iframe width="1024" height="576" src="https://youtube.com/embed/MokwdERAlgc?rel=0" title="Exercise 5.2 Custom Dashboards" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Section Information
- Create a custom dashboard called 5.2.1_NewReportDashboard
- Create a custom dashboard using previous lab reports and call it 5.2.2_CL21HOLCCT2108Dashboard

1. Navigate to the Dashboards section of Analyzer and `Create New` Dashboard
2. Drag dashboards according to the video instruction to the work canvas and position to your liking
3. When dashboard components have been arranged, you should have somthing similar to this

![custom dashboard](https://user-images.githubusercontent.com/75790934/113778075-92da5900-96f1-11eb-9b05-3a5f86d24920.png)

4. Save this report as `5.2.1_NewReportDashboard` under your team folder
5. Run the report and notice that you can make changes to widget sizes but this will not save to the template
6. Edit the new dashboard and make any sizing changes and save to see those changes every time
7. Create a `new dashboard` for the next exercise
> * <a href="https://youtube.com/embed/MokwdERAlgc?start=179" target="_blank">Start at timestamp</a>
8. In this new dashboard you will be using several of the reports created earlier in this lab
  - 4.2.1_CSR_QueueStatus
  - 3.2_AAR_AgentState
  - 3.3_CSR_ContactVolume
  - 3.1_CSR_Contacts

![5-2customdashboard](https://user-images.githubusercontent.com/75790934/113779194-f3b66100-96f2-11eb-8a22-21c1bf94b1a5.png)

9. Save this report as `5.2.2_CL21HOLCCT2108Dashboard`
10. Explore some options to edit and personalize this new dashboard like changing background colors
11. This lab is complete, however, if you have time feel free to move to the Bonus Lab.

## Next Lab is Lab 6: Bonus Lab
> * [Analyzer Lab 6 Link](https://wxcctechsummit.github.io/holcct2108/livelabs/Lab6Analyzer.html)

[Back to top](#cisco-live-holcct-2108-webex-contact-center-reporting---analyzer-deep-dive)

## No Time for Bonus Lab?
> * [Primary Labs Complete Back to Main](https://wxcctechsummit.github.io/holcct2108/finishedholcct2108.html)


