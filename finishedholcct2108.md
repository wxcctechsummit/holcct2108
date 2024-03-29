---
title: "Cisco Live HOLCCT-2108 Lab Guide Library"
---
<script>

window.onload=function(){window.location ="https://webexcc.github.io/"}

</script>

# Labs Have Been Completed!  Congratulations!
### Please be sure to complete the <a href="https://reg.rainfocus.com/flow/cisco/ciscolive2021/adashsurvey/page/surveydash" target="_blank">Cisco Live Lab Survey</a>

<p align="center">
  <img src="https://user-images.githubusercontent.com/75790934/113780553-fe71f580-96f4-11eb-85c3-0fa7064794b5.gif">
</p>

![Banner](images/wxccbanner.jpg)

### Welcome to Cisco Live 2021 HOLCCT-2108 New Webex Contact Center Analyzer - Data and Analytics Deep Dive  

# Table of Contents
1. [Webex Contact Center Quick Links](#quick-links)
2. [Analyzer Lab Configuration Diagram](#analyzer-lab-configuration)
3. [Connecting Instructions](#connecting-instructions)
	* [Inbound Voice](#inbound-voice)
	* [Facebook Chats](#facebook-chats)
	* [Email Assistance](#email-assistance)
	* [Chat using WxCC Chat Widget](#chat-using-wxcc-chat-widget)
	* [Inbound SMS](#inbound-sms)
4. [Lab Schedule](#lab-schedule)
5. [Lab Video Links](#lab-video-links)

## Purpose and Scope
This intermediate level lab session is intended for Contact Center engineers and Business Managers/Supervisors with prior Contact Center experience. No previous exposure to the product is required. Get all knowledge to…... This lab covers all aspects of, Cisco's native-cloud Webex Contact Center Reporting from basic UI to Advanced Visualization and Data capabilities

## Pre-requisite

1. Recommended to review BRKCCT-1004 before this lab but not required
2. Ensure that you have received your tenant login credentials and directions to make some test calls before starting the Lab

## Quick Links 
*Note: We've done our best to ensure links open in a new tab, but if it does not, just right click and select the open in new tab option*

* <a href="https://portal.wxcc-us1.cisco.com/portal" target="_blank">Portal</a>
* <a href="https://analyzer.wxcc-us1.cisco.com/analyzer/home" target="_blank">Analyzer</a>
* <a href="https://desktop.wxcc-us1.cisco.com" target="_blank">Agent Desktop</a>

## Analyzer Lab Configuration
- Voice calls will guide you through the flow to enter your student ID and land in your team queue
- Multimedia will be shared with all queues

![Banner](images/analyzerlabsetup.jpg)

# Connecting Instructions
## Inbound Voice
**Dial +15084337864**
* If international calling please use the US code

 1. `Voice calls` hit a common Entry Point and answers with a Flow enabled for Google CCAI.
	* Tell the auto attendant you want to speak to an agent
	* Enter your Student Number.  The number matches the number in your login ID.
	* Calls will route to your own queue so ensure your agent is logged in and your agent will get the call
2. `Omnichannel` contacts will all route to a common queue
	* Help your classmates out by responding to their emails, texts, facebook and SMS queries.

## Facebook Chats
1. Use the following Link: <a href="https://www.facebook.com/Wxcc-Demo-Page-107841834739318" target="_blank">Facebook</a>

## Email Assistance
1. Use your email client and send to:  `wxccanalyzer@gmail.com`

## Chat using WxCC Chat Widget  
1. Navigate to a Java Script editor like <a href="https://js.do/" target="_blank">JS.DO</a>
2. Insert the following code block into the Java Editor, on the left side
```
<script>
    //Name of the Customer Support Template: CL2108lab_Chat
    //Name of the Organisation: CL_HOLCCT2108
      (function(document, script) {
      var bubbleScript = document.createElement(script);
      e = document.getElementsByTagName(script)[0];
      bubbleScript.async = true;
      bubbleScript.CiscoAppId =  'cisco-chat-bubble-app';
      bubbleScript.appPrefix = '';
      bubbleScript.DC = 'produs1.ciscoccservice.com';
      bubbleScript.orgId = '85d74f70-1fd5-4744-91f2-042ea361ca03';
      bubbleScript.templateId = '424807d0-91bf-11eb-96d7-e33c5a6b0997';
      bubbleScript.src = 'https://bubble.produs1.ciscoccservice.com/bubble.js';
      bubbleScript.type = 'text/javascript';
      bubbleScript.setAttribute('charset', 'utf-8');
      e.parentNode.insertBefore(bubbleScript, e);
      })(document, 'script');
    </script>
```
3. Once this is pasted, click the `Run Code` button at the top
4. Look on the **Lower Right Side** for the `Chat Bubble` and click that to start a Chat session

## Inbound SMS
1. Text to `+12029824690`
2. If any agents are available, the SMS will get routed.
3. If no agents are available, you will not get a response


## Lab Schedule

| Duration | Session | Corresponding `Lab Guide` |
| ---- | ------- | ----------------- |
| 20 min | Admin Portal Dashboards and Analyzer User Interface |  [Lab 1: Admin Portal Dashboards and Analyzer User Interface](livelabs/Lab1Analyzer.md) |
| 20 min | Stock Reports | [Lab 2: Stock Reports](livelabs/Lab2Analyzer.md) |
| 30 min | Custom Visualizations| [Lab 3: Custom Visualizations](livelabs/Lab3Analyzer.md) |
| 40 min |Advanced Insight Functionalities| [Lab 4: Advanced Insight Functionalities](livelabs/Lab4Analyzer.md) |
| 20 min | Dashboards | [Lab 5: Dashboards](livelabs/Lab5Analyzer.md) |
| 30 min | Data Capabilities | [Lab 6: Data Capabilities](livelabs/Lab6Analyzer.md) |

## Lab Video Links
**Full video links used in the lab instructions.  Video links are also available in the lab exercises.**

### Lab 1: Admin Portal Dashboards and Analyzer User Interface Videos
- <a href="https://youtube.com/embed/Q4kf8dHN8x8" target="_blank">Lab Exercise 1.1 Dashboard Reports</a>
- <a href="https://youtube.com/embed/4pGNHkd87Zs" target="_blank">Lab Exercise 1.2 Analyzer User Interface</a>
- <a href="https://youtube.com/embed/MdKzqrZ-EGA" target="_blank">Lab Exercise 1.3 Access Control</a>
### Lab 2: Stock Reports Videos
- <a href="https://youtube.com/embed/aCGxNPmWvPw" target="_blank">Lab Exercise 2.1 Execute Stock Reports</a>
- <a href="https://youtube.com/embed/f-vsOu32tD4" target="_blank">Lab Exercise 2.2 : Create Custom Report using Stock Report</a>
### Lab 3: Custom Visualizations : Contact and Agent Videos
- <a href="https://youtube.com/embed/n4qAwwhuTmg" target="_blank">Exercise 3.1 - Create Realtime Contact Report</a>
- <a href="https://youtube.com/embed/IiA0RYmgoIE" target="_blank">Exercise 3.2 - Create Realtime Agent Report</a>
- <a href="https://youtube.com/embed/t_Ub0xGfG0s" target="_blank">Exercise 3.3 - Create Chat Reports with Interval</a>
### Lab 4: Advanced Insights Videos
- <a href="https://youtube.com/embed/mIaUgAEjRHs" target="_blank">Exercise 4.1 - Using Formula and Filter</a>
- <a href="https://youtube.com/embed/Poc7WdDdbEM" target="_blank">Exercise 4.2 - Enhanced Field Compound Visualizations</a>
### Lab 5: Dashboards Videos
- <a href="https://youtube.com/embed/quuS5xrsmgI" target="_blank">Exercise 5.1 Stock Dashboards</a>
- <a href="https://youtube.com/embed/MokwdERAlgc" target="_blank">Exercise 5.2 Creating Custom Dashboards</a>
### Lab 6: Data Capabilities Video
- <a href="https://youtube.com/embed/NBwnjKByJB4" target="_blank">Lab 6 Data Capabilities</a>


# Lab Info Per User
* [LabInfo](livelabs/labinfo.md)

[Back to top](#welcome-to-cisco-live-2021-holcct-2108-new-webex-contact-center-analyzer---data-and-analytics-deep-dive)

