# Instructions for Generating Data
Use these instructions to generate data into your tenant.  This should take no more than about 10 minutes and will only generate a little data for you to use during the course of the lab.

## Use the sections below to 
- Make voice calls into the system
- Access Facebook and create a chat request
- Email the system for an agent
- Create a chat bubble and create a chat request
- Send an SMS to connect with an agent

## All Interactions Require Agent Desktop Logged in and **Available**


### Inbound Voice
**Dial +1 508-433-7864**
* If international calling please use the US code

 1. `Voice calls` hit a common Entry Point and answers with a Flow enabled for Google CCAI.
 2. Tell the auto attendant you want to speak to an agent  _(Sample:Say "Agent")_
 3. Enter your Student Number.  The number matches the number in your login ID. _(Sample: 10#)_
 4. Calls will route to your own queue so ensure your agent is logged in and your agent will get the call
  * Want to Try Callback and check reports?
	* Make your agent not avaliable and let call go to queue
	* After few seconds wait you will get an option to press 1 for Callback and 2 to stay in Queue
	* Press 1, call will disconnect
	* Make your agent Avaliable, you will see a callback!!
5. Make a few more test calls just to generate some data
  
### Omnichannel Contacts
All `Omnichannel` contacts will all route to a common queue
* Help your classmates out by responding to their emails, texts, facebook and SMS queries.

### Facebook Chats
1. Use the following Link: <a href="https://www.facebook.com/Wxcc-Demo-Page-107841834739318" target="_blank">Facebook</a>
2. Request a chat and wait for a response
3. As long as your agent is ready, you or another attendee will get the contact request

### Email Assistance
1. Use your email client and send to:  `wxccanalyzer@gmail.com`
2. Give it a Subject and a short message and send
3. Agent will see the request and respond

### Chat using WxCC Chat Widget  
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
5. Enter your Name, Email and Reason and start the Chat
6. When BOT responds, you can use "Agent" as the key word to escalate the call to the agent
7. Respond to chats to help your classmates out

### Inbound SMS
1. Text to `+1 202-982-4690`
2. If any agents are available, the SMS will get routed.
3. If no agents are available, you will not get a response

# Once Section Complete


## Back to Main Page
* [Main Page](/CiscoLiveLabLibrary2108.md)

[Back to top](#instructions-for-generating-data)

