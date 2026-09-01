# Activity-audit

# EXPERIMENT 5

# AUDITING CLOUD ACTIVITY USING AWS CLOUDTRAIL

## Objective

To audit and monitor cloud activity in AWS using AWS CloudTrail by viewing and analyzing recorded AWS events and identifying important audit information such as user identity, event name, event time, AWS service, region, and operation status.

## 1. Requirements

  -> AWS Account 
  
  -> Web Browser 

  -> Internet Connection 

  -> Amazon S3 access 
  
  -> AWS CloudTrail 

## PART A — ACCESS AWS CLOUDTRAIL
## Step 1: Login to AWS

1.Open the AWS Management Console. 

2.Sign in using your AWS account. 

3.In the AWS search bar, type CloudTrail. 

4.Select AWS CloudTrail. 

Output:<img width="1918" height="903" alt="image" src="https://github.com/user-attachments/assets/7c604820-1edb-4be6-93f5-787c76deeab2" />

## Step 2: Open Event History

1.In the CloudTrail navigation menu, select Event history. 

2.CloudTrail displays recent AWS activity. 

3.Review the available events. 

The Event History page may display information such as:
  -> Event time 

  -> Username 

  -> Event name 

  -> Event source 
  
  -> Resource type 

  -> Resource name 

Output:<img width="1919" height="907" alt="image" src="https://github.com/user-attachments/assets/f8829658-e4f0-4e50-b6ff-4711684a577c" />

## PART B — ANALYZE A CLOUDTRAIL EVENT

## Step 3: Select an Event

1.From the Event History list, select an S3-related event. 

2.Click the event to open its details. 

3.Examine the event information and the event record/JSON. 

For this experiment, a CreateBucket event can be used.

## Step 4: Analyze the CreateBucket Event

  -> The CreateBucket event indicates that an Amazon S3 bucket creation operation occurred.

Record the following information:

Parameter	     Observation

Event Time    	__________

User Name	      __________

Event Name	   CreateBucket

Event Source	s3.amazonaws.com

AWS Region	   __________

Read-only	     __________

Error Code	    __________

Activity	S3 bucket creation

Meaning of Important Fields


Event Time - Time at which the activity occurred

User Name -	User/identity associated with the activity

Event Name -	AWS operation that was performed

Event Source -	AWS service that generated the event

AWS Region -	Region where the activity occurred

Read-only -	Indicates whether the event was only a read operation or involved a change

Error Code -	Indicates whether an error occurred

Output:<img width="1839" height="514" alt="image" src="https://github.com/user-attachments/assets/daebfb64-7541-4026-81f3-13a1249fb9b0" />

## PART C — IDENTIFY ANOTHER CLOUDTRAIL EVENT
## Step 5: Select Another Event

1.Return to CloudTrail → Event history. 

2.Select another event. 

3.Open its details. 

4.Record the important fields. 

For example, an event such as:
AutomatedDefaultVpcCreationn may be present.

This event is associated with Amazon EC2.

## Step 6: Analyze the Second Event

## Record:

Parameter	  Observation

Event Time	 __________

User Name   	__________

Event Name	 AutomatedDefaultVpcCreation

Event Source	 ec2.amazonaws.com

AWS Region	  __________

Read-only	    __________

Error Code	    __________

Activity	Automated default VPC creation

Output:<img width="1911" height="592" alt="image" src="https://github.com/user-attachments/assets/b72587f2-af01-4062-9f95-f5a990db8b6c" />

## PART D — COMPARE THE EVENTS

## Step 7: Prepare the Audit Comparison

Compare the two CloudTrail events.

Parameter	Event 1	Event 2

Event Time	__________	__________

User Name	__________	__________

Event Name	CreateBucket	AutomatedDefaultVpcCreation

Event Source	s3.amazonaws.com	ec2.amazonaws.com

AWS Region	__________	__________

Read-only	__________	__________

Error Code	__________	__________

Activity	S3 bucket creation	Automated VPC creation

PART E — SECURITY AUDIT ANALYSIS
Step 8: Identify Who, What, When and Where
For each event, identify:
WHO?
Who or which identity performed/generated the activity?
WHAT?
What AWS operation was performed?
WHEN?
At what date and time did the activity occur?
WHERE?
In which AWS Region did the activity occur?
RESULT?
Was the operation successful or did it generate an error?

Output:<img width="1840" height="516" alt="image" src="https://github.com/user-attachments/assets/0285ea87-5069-4b92-a19f-eb82b923c2bf" />
<img width="1833" height="366" alt="image" src="https://github.com/user-attachments/assets/ade8bf6c-bc6b-4f1d-8e4e-51b1d6314851" />



RESULT
The cloud activities in AWS were successfully audited using AWS CloudTrail Event History. Different AWS events were examined based on event time, user identity, event name, event source, AWS Region, read-only status, and error status. The experiment demonstrated how AWS CloudTrail provides an audit trail for monitoring, accountability, and investigation of cloud activities.
