# CODTECH Internship - Task 2

##  Task Name: Cloud Monitoring and Alerts (AWS CloudWatch)
*Intern Name**: Prachi Gupta  
> **Task**: 2 - Cloud Monitoring and Alerts  
> **Internship Provider**: CODTECH    
> **Status**: Completed


This task demonstrates how to configure AWS CloudWatch to monitor an EC2 instance’s CPU utilization and send an alert via Amazon SNS when usage crosses a threshold.

---

##  Objective

To set up an alarm that notifies via email when the **CPU Utilization** of an EC2 instance exceeds a certain limit — in this case, **70%**.

---

## EC2 Instance Details

- **Instance ID**: `i-04dd4e487e2b28646`
- **Region**: Asia Pacific (Mumbai) `ap-south-1`
- **Metric Monitored**: `CPUUtilization`
- **Alarm Trigger Condition**: 
  - `CPUUtilization >= 70` for `1 datapoint` within `5 minutes`
- **Statistic Used**: Average

---

##  SNS Alert Configuration

- **SNS Topic Name**: `HighCPUAlert`
- **Subscribed Email**: `prachigupta2624@gmail.com`
- **Notification Trigger**: Alarm state enters `In alarm`
- **Subscription Status**: Confirmed ✅

---

##  Steps Followed

### Step 1: Specify metric and conditions  
Selected the EC2 instance metric `CPUUtilization`, set the threshold to `>= 70`, and period to 5 minutes.

### Step 2: Configure actions  
Selected the existing SNS topic `HighCPUAlert`, and linked my email for notifications.

### Step 3: Add alarm details  
Added a description to identify the alarm easily.

### Step 4: Review and create  
Reviewed the configuration and successfully created the alarm.

---

##  Screenshots

Below are the screenshots of my Task 2 setup:
- Metric and threshold configuration
- SNS Topic setup and subscription
- Alarm details and state
- Successful alarm creation

_All images are included in this repository._

---

## ✅Services Used

- **Amazon EC2**
- **Amazon CloudWatch**
- **Amazon SNS**

---

## Status

- [x] Alarm created successfully
- [x] Email notification configured and confirmed
- [x] Alarm visible in CloudWatch console
- [x] Task 2 complete

---

> 