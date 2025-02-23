# Submissions Page (Submit Files, Emails, Teams Messages, URLs)

This feature allows you to submit files, emails, Teams messages, and URLs to Microsoft Defender.

## Submitting Files

1. Go to the [Microsoft Defender portal](https://security.microsoft.com).
2. Select **Actions & Submissions** on the left-hand panel.
3. Select **Submissions**. You will see tabs for Emails, Teams Messages, Email Attachments, URLs, Files, and User Reported.
4. User Reported shows all user-reported submissions, while the rest are for admin submissions.
5. Submissions help Microsoft to improve their detection policies.
![Submissions page](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2047.png)

### To Submit a File:
1. Select **Files** or **File Hash** depending on your preference.
2. You can also decide to upload a file. The maximum file size is 500 MB.
3. Upload a test file you created on your desktop.
4. The file should be categorized. You can select **Malware**, **Unwanted Software**, or **Clean**.
   - I will select **Clean** because after my analysis, I believe the file is clean.
5. Choose the priority:
   - **Low** for bulk file or file hash submissions.
   - **Medium** for standard submissions.
   - **High** for immediate attention (3 allowed per organization per day).
6. In **Notes for Microsoft**, type "Don't analyze, it's a test".
7. Check the **Share feedback and relevant content with Microsoft** checkbox.
8. Click on **Submit**. You will receive a pop-up asking if you are sure you want to submit. Click **OK**.
9. You will get a pop-up saying your submission has been submitted to Microsoft for analysis. They will get back to you with the result as soon as your submission has been analyzed.
10. Click on **Done**.
11. Refresh the page. You will see the submission name, submission ID, submitted by, date submitted, and reason for submitting.
12. When you click on the submission, you can add this file as an indicator or go hunt.
![Submissions File](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2048.png)

## Submitting Emails

1. Under **Select the submission type**, you can select **Email**, **URL**, and **Email Attachment**.
2. Add the email Network Message ID or upload the email file.
   - **Network Message ID (NMID)** is a unique identifier assigned to emails processed through Microsoft Defender for Office 365. The NMID can be used to trace and investigate specific email messages within the Defender portal.
   - To find the Network Message ID:
     - Open the email message in Outlook.
     - View the message header: In Outlook, go to **File > Properties**. The Internet headers box will contain the NMID.
     - Search the Defender Portal: Use the NMID to search for the specific email in the Microsoft Defender for Office 365 portal. Go to **Threat Explorer** or **Advanced Hunting** and enter the NMID to locate and investigate the email.
     - It is available as this value: **X-MS-Exchange-Organization-Network-Message-Id**.
     - If you're looking at a quarantined message, it will be **X-MS-Office365-Filtering-Correlation-Id**.
3. Choose at least one recipient who had an issue. It is recommended to add one user.
4. Specify why you are submitting this message to Microsoft:
   - **I've confirmed it's clean**.
   - **It appears clean**.
   - **It appears suspicious**.
   - **I've confirmed it's a threat** (you will have to select whether it's spam, phish, or malware).
5. Click on **Next** and **Submit**.
![Submissions email](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2049.png) 

## Submitting Teams Messages

1. You can only submit user-reported Teams messages.
2. A user-reported Teams message will come under **User Reported**.
3. Select the user-reported message and click on **Submit to Microsoft for analysis**.
4. From there, you can report it as phishing or malware.
![Submissions teams message](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2050.png)

## Submitting Email Attachments

The submission form is similar to email submissions.
![Submissions email attachments](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2051.png) 
## Submitting URLs

1. Click on the **URL** tab.
2. Click on **Submit to Microsoft for analysis**.
3. Select the submission type:
   - **URL**
   - **Email**
   - **Email Attachment**
4. Since you want to submit a URL, choose **URL**.
5. Type in the URL.
6. Specify why you're submitting this URL to Microsoft:
   - **I've confirmed it's clean**.
   - **It appears clean**.
   - **It appears suspicious**.
   - **I've confirmed it's a threat** (you will have to specify whether it's phish or malware).
![Submissions URL](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2052.png)
![Submissions URL](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2053.png)
![Submissions URL](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2054.png)
 
## User Reported

You can configure this so that users can use the phishing button in Outlook to submit suspicious emails to the Defender portal. The admin will select the submitted user report and click on **Submit to Microsoft for analysis**.

![Submissions User Reported](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2050.png)

## Submitting Files from Alert

1. Select **Alerts** in the Defender portal.
2. Select the alert. When the pop-up showing the alert appears on the right, click on the three dots and select **Submit items to Microsoft for review**.
3. Choose the submission type: **File** or **File Hash**.
4. Upload the file.
5. Categorize this submission as **Malware**, **Unwanted Software**, or **Clean**.
6. Choose the priority: **Low**, **Medium**, or **High**.
7. Include the alert story. This will attach a JSON file that will help Microsoft experts further investigate your submission.
![Submissions Files from Alert](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2055.png)

## Submitting from Email & Collaboration

1. Select **Review**.
2. Select **Quarantined**.
![Submissions from Email & collaboration](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2056.png)

## Submitting a File for Malware Analysis

You can also submit a file for malware analysis through the following URL: [Microsoft File Submission](https://www.microsoft.com/en-us/wdsi/filesubmission)

![Submissions from the Microsoft link](https://github.com/StephenOwusuB/Implementing-Microsoft-Defender-for-Enterprise-Security/blob/main/images/Submissions/MDE%20onboard%2057.png)
---

This should provide clear instructions for submitting various items in Microsoft Defender. If you need further adjustments, let me know! 😊
