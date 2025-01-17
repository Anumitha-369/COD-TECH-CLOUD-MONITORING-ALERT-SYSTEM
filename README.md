# COD-TECH-CLOUD-MONITORING-ALERT-SYSTEM
CLOUD ALERT MONITORING SYSTEM IN AWS S3

**COMPANY** : CODTECH IT SOLUTIONS 
**NAME** : ANUMITHA J 
**INTERN ID** : CT6WGUL 
**DOMAIN** : " CLOUD COMPUTING " 
**BATCH DURATION** : January 5th 2025 to February 20th 2025.
**MENTOR NAME** : SANTHOSH NEELA

TASK DESCRIPTION :

SET UP MONITORING FOR A CLOUDBASED APPLICATION USING AWS CLOUDWATCH, GOOGLE CLOUD MONITORING, OR AZURE MONITOR. 

CLOUD MONITORING AND ALERTS :

DELIVERABLE: CONFIGURED ALERTS
AND A DASHBOARD SHOWCASING
METRICS.

Here are the steps to configure alerts and a dashboard showcasing the metrics :

AWS CLOUDWATCH :

AWS CloudWatch helps you keep an eye on your applications by tracking metrics, monitoring log files, and setting up alarms.
It gives you useful data and insights to ensure your applications run smoothly, helps you spot and fix issues, and makes sure you're using resources efficiently.

STEP 1 : Open the Cloud Watch Console 
STEP 2 : Select cloud watch or search for cloud watch .
STEP 3 : Create an alarm in alarn sections , select " ALL ALARMS " and click on " CREATE ALARM " .
STEP 4 : Select a metric: 
         Choose the metric you want to monitor (e.g., CPU utilization, memory usage).
STEP 5 : Set conditions: 
         # Define the conditions for the alarm (e.g., threshold value, period).
STEP 6 : Configure actions: 
          Set up actions to be taken when the alarm is triggered (e.g., send an email notification).
         # ACTIVE AN SNS SUBSCRIPTION TO GET NOTIFIED IN EMAIL. 
STEP 7 : Save the alarm: 
         # Save your alarm configuration.
STEP 8 : Create a dashboard to monitor the application's performance .

Detailed Steps to Set Up Monitoring with AWS CloudWatch

1. Open CloudWatch Console

First, log in to your AWS Management Console. In the menu, find and click on "CloudWatch" .

2. Create an Alarm

Once you're in the CloudWatch console, look for the "Alarms" option on the left side and click it. Then, click on "Create Alarm" to start the process. 
Alarms help you monitor specific data points and notify you or take action when something unusual happens. ( when the data points reaches threshold limit , alert will be notified )

3. Select a Metric

Now, you need to choose a metric to monitor. Metrics are like pieces of data collected from various AWS resources (like servers or databases). 
Here , I have used metrics :

---- Namespace
---- AWS/Lambda

---- Metric name
---- Errors

---- FunctionName
---- nodejs_custom_error ( Function has been created on new for setting the alarm alert )

4. Set Conditions

After choosing a metric, set the conditions for the alarm. This means you define when the alarm should go off.

I preferred using the threashold limit and time period for about 3 outof 5 and for 5minutes.

---- THRESHOLD : 3 OUTOF 5
---- TIME PERIOD : 5 MINUTES 

5. Configure Actions

Next, decide what should happen when the alarm goes off. You can set it to send you an email, trigger an AWS Lambda function, or create a notification in an SNS topic. You can even set it to automatically restart a server if it has issues.
I preferred to  
---- " SNS notifications " via email . 

6. Save the Alarm

Finally,  Make sure everything is correct. Then, click "Create Alarm" to save it. Your new alarm will start monitoring the metric you selected and will notify you or take action based on the conditions you set.

# Creating a Dashboard
Dashboards in CloudWatch help you visualize and monitor your application's metrics and alarms in real time.

1. Create a Dashboard

In the CloudWatch console, click on "Dashboards" in the left menu, then click "Create Dashboard." Give your dashboard a name.

2. Add Widgets

To make your dashboard useful, add widgets like charts or text boxes. Click "Add widget" and choose the type you want. Then, select the metrics you want to display in each widget.

3. Configure Widgets

Set up each widget by choosing how you want the data to be displayed. You can select the time range and type of graph (like line graph or stacked area). 

4. Save the Dashboard

After configuring all the widgets, click "Save Dashboard." Your dashboard will now show real-time data for the selected metrics, making it easy to monitor your application's performance

OUTPUT :

CLOUD WATCH ALARM : SHOWING THE " OK " STATE .




