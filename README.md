# Ai-automation-lead-qualification
# AI Automation Lead Evaluation System

## Overview
An automated lead-evaluation and follow-up system designed to classify and manage real estate leads based on engagement and intent.

## System Functionality
- Leads are classified as:
  - Cold
  - Medium
  - Hot
  - Red flag
  -  unsubscribed
- Classification is based on response behaviour and predefined criteria
- Automated actions are triggered based on lead status:
  - Monthly follow-ups for cold leads
  - Weekly check-ins for medium leads
  - Immediate notifications and call scheduling for hot leads / very hot leads
  - Automatic exclusion of unqualified leads.
  - Note that the whole system is made up of 4 different system in one . 

## Tools Used
- Zapier (workflow automation)

- Slack & Whatapp (notifications and internal alerts)
- google Email automation tools
- Google Sheets / CRM-style data storage
- Google Calandar
- Chat gbt
- SMS
- zapier Form
- zapier update table
- zapier Formate
- zapier Schedule
- zapier find record
- zapier create loops 

## Logic Design
- Continuous re-evaluation based on response timing and engagement
- Status updates occur automatically after each interaction
- System prevents unnecessary follow-ups to disengaged leads

## Skills Demonstrated
- Workflow automation
- Logical system design
-  Process optimisation
- Real-world application of AI-assisted decision-making

## IN depth explanation of whole system 

Main system explanation 

The main system start of with the lead filling in a form that gives uses data about them and what they are looking for and there current finical state ,
that information is then transfered to chat gbt where , it will evaulate the lead based on the data and information and give them a lead type : 
these include hot lead , very hot lead , cold , medium , red flage . once there lead type has been give they will go down the four different path ways based on there lead type. 
Path A is that chat gbt says they are very hot / hot , Path B is for medium lead , path C is cold lead , path D is for red flags .
if they are hot lead they will go through Path A where it will up date the table with there lead type then notify the agent team by useing slack . 
This notifcation will inform them about a hot lead / very hot lead that they must go after , and that they must set up a call with them .
It then sends a message to the specific agent that will handle the call through whatapp. then after that it sends a message to lead through sms 
message informaing them that we have recieved there form submission and that we would like to set a day to talk , which then they are provided with a calander to book a day based on what day the agent and lead are avaliable. lastly it will then send a email to them just informatiing what will happend after . 

For the medium lead path way and cold lead path way they both update the table(data base where the lead informaton is stored ) lead type  and put the rest of the information in there as well , and then sends a email to the lead telling them that we have recieved the submission , and that we will email to check when there ready .

Red flag nothing happends 

Main system image:
<img width="925" height="641" alt="image" src="https://github.com/user-attachments/assets/19a2da43-10df-4d5a-abe9-60f1a130e981" />






<img width="965" height="642" alt="image" src="https://github.com/user-attachments/assets/c8a22074-3c31-4b46-93ef-3e2356df665a" />








## second system explanation  (cold lead email weekly):
this system start of with schedule activation every week day . when activated it will find all cold leads that have been inactive . it then loops through all of the cold leads and sends them  emails . this email ask how they are if they are ready to by a property , but it also updates them about  the propertys avaliable , and what has been happening with the agency . it then updates all leads that where loop through last follow up date in the data bases . 


second system image:


<img width="568" height="584" alt="image" src="https://github.com/user-attachments/assets/8f0267e9-4fce-47ae-bf88-bb197bb3ed8a" />





## third system explanation(medium lead email weekly):
this system start of with schedule activation every week day . when activated it will find all medium leads that have been inactive . it then loops through all of the medium leads and sends them  emails . this email ask how they are if they are ready to by a property , but it also updates them about  the propertys avaliable , and what has been happening with the agency . it then updates all leads that where loop through last follow up date in the data bases . 


third system image:


<img width="589" height="550" alt="image" src="https://github.com/user-attachments/assets/27f2d8a7-411a-43d2-afe3-9b07688297f1" />



## Four system explanation(medium lead email weekly):
this system starts of by getting all email replies , then after getting all email replies it filters all email that contain the caption re in it email showing that it a reply from the previous one , and it also filters emails contain a body plain exist . one it found all email that contain those conduction we then search for all there email name in the data bases and retrieve them . once after that we get all the content in each email make chat gbt analysize the email content to categorises them into 4 four differnt categories: interested , neutral , not interested , subscribed .  if you are  put into the not interested , then you go down path C which involves getting the current date , and update lead lead type in the data bases to cold , and also update follow up date . this is the same for path D but there lead type is updated to subscired meaning the agency will not contact them again. if you are neutral you stay the same , however if you are interested you go up one lead and go down the path A where there are 3 different path for each lead type there currently are   .  for each one they first get the current date , then update the lead type by one up . so medium to hot , cold to medium ,hot to very hot . in addiotn it also up date the follow up date . however for medium lead since they got prompoted to hot a slack message is sent to agency team saying how somone has been prompoted to hot lead , and that they must go after them . the system then sends a messsage to the lead asking them to arrange a time for them to talk with one of the agents . they can do this be setting a date on the calander 


Fourth system image:

<img width="914" height="662" alt="image" src="https://github.com/user-attachments/assets/a2fb4c28-c155-47a3-8d96-163aed181c81" />

<img width="978" height="652" alt="image" src="https://github.com/user-attachments/assets/160f6645-70a3-441a-9562-9d3583f0d113" />




