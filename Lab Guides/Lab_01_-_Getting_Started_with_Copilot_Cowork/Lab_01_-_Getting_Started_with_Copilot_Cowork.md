**MICROSOFT 365 COPILOT COWORK \| LAB GUIDE**

# Lab 1: Getting Started with Copilot Cowork

| EST. DURATION | TASKS | STEPS |
| --- | --- | --- |
| 30 min | 5 | 70 |

## Overview

In this hands-on lab, you will get oriented to Copilot Cowork, the agentic workspace inside Microsoft 365 Copilot. Unlike traditional Copilot Chat, where you ask a single question and receive a single answer, Cowork can plan and carry out multi-step tasks on your behalf - reading your emails, checking your calendar, working with files, and delivering a finished result, all in one go. You will sign in to Microsoft 365, tour the Cowork home screen, explore how starter tiles pre-fill ready-to-run prompts, and review the Customize area where Cowork's capabilities can be extended with plugins and skills. You will then generate sample emails and calendar events in Outlook, upload sample files to OneDrive, and create a team in Microsoft Teams - before returning to Cowork to explore work context, task history, and scheduled tasks against that data.

> **Note:** Tasks 2, 3, and 4 are prerequisite setup steps rather than part of the core walkthrough. Copilot Cowork works by acting on real data in your mailbox, calendar, files, and Teams, so before you can meaningfully explore what it can do, your environment needs sample emails, calendar events, OneDrive files, and a Teams channel in place. These three tasks create that data for use throughout this lab and every lab that follows - complete them in order before moving on to Task 5.

## Objectives

In this lab, you will perform the following:

- **Task 1:** Sign In and Explore the Cowork Interface

- **Task 2:** Generate Sample Emails in Outlook

- **Task 3:** Generate Sample Calendar Events in Outlook

- **Task 4:** Upload Sample Files to OneDrive and Create a Team in Microsoft Teams

- **Task 5:** Explore Work Context, Task History, and Scheduled Tasks

## Task 1: Sign In and Explore the Cowork Interface

In this task, you will sign in to Microsoft 365, review how Copilot Cowork differs from Copilot Chat, explore the layout of the Cowork home screen, see how starter tiles pre-fill ready-to-run prompts, and review the Customize area where Cowork's capabilities can be extended with plugins and skills.

1.  Review how Copilot Cowork compares to Copilot Chat.

| **Copilot Chat**         | **Copilot Cowork**                         |
|--------------------------|--------------------------------------------|
| One question, one answer | Multi-step tasks from a single instruction |
| You guide each step      | Cowork plans and executes the steps itself |
| Great for quick lookups  | Great for complex, repeatable workflows    |
| No task history          | All tasks are saved and searchable         |

2.  Open the Edge browser and navigate to the Microsoft 365 portal with the below link and click on **Sign in**:

    ```
    www.office.com
    ```

    ![](./media/image1.png)

3.  On the sign-in page, enter the provided email address and click **Next (2)**.

- **Email/Username**

    ![](./media/image2.png)

4.  Enter the provided Temporary Access Pass and click **Sign in (2)**.

- **Temporary Access Pass**

    ![](./media/image3.png)

5.  When prompted, select **No** on the Stay signed in? dialog.

    ![](./media/image4.png)

6.  Click the **Auto** dropdown at the top and review the models available.

    ![](./media/image5.png)

    > **Note:** Leave the model set to Auto for this entire lab. Auto automatically selects the best available model for each task, so you do not need to choose one manually.

7.  At the top of the left panel, click on the **Cowork** tab.

    ![](./media/image6.png)

8.  Click the **"..." (1)** icon at the top-right corner, select **Keyboard shortcuts (2)**, and review the list. Close the page.

    ![](./media/image7.png)

    ![](./media/image8.png)

9.  Select **New task (1)** and click on **Prep for a meeting (2)**. If Prep for a meeting is not visible, click on **See more**.

    ![](./media/image9.png)

10. Click on **Use this task.**

    ![](./media/image10.png)

11. Review the **prompt (1)** that Cowork has pre-filled in the task bar - notice how it already describes gathering attendee, agenda, and file context in one instruction. Then clear the task bar **without sending it**.

    ![](./media/image11.png)

12. Click on **Customize** in the left panel.

    ![](./media/image12.png)

13. Click the **filter (1)** icon beside **Discover** and select **Collaboration (2)**.

    ![](./media/image13.png)

14. Review the plugins visible in the Discover gallery.

    ![](./media/image14.png)

    > **Note:** Each plugin tile shows a logo, name, and one-line description. Plugins connect Cowork to services outside Microsoft 365.

15. Click the **Add** dropdown to create or upload a new skill.

    ![](./media/image15.png)

## Task 2: Generate Sample Emails in Outlook

In this task, you will use Cowork to generate and send 5 sample training emails to your own Outlook inbox for use in later labs.

1.  Navigate back to the **+ New task** from the left panel. In the Cowork pane, enter the below prompt **(1)** and click the **send (2)** button:

    ```
    I need you to seed my Outlook inbox with 5 sample training emails for a Copilot Cowork demo environment (Contoso Electronics / Project Orion ERP modernization scenario). Send each individually to my own email address so it lands as a received message in my Inbox. You have my approval to send all 5 without pausing for individual confirmation - send them one after another, then give me a final summary list (subject + time sent).

    For every email: proper business email (greeting, 2–3 short paragraphs or bullets, professional sign-off with sender name/title/company). Prefix the Subject line with the source tag in brackets. Do not literally attach files - mention any referenced attachment in the body text only.

    Send these 5, in order:

    1. [Northwind Retail] Subject: "Final Contract Review - Payment Milestone Clarification." From: Priya Desai, Procurement Lead, Northwind Retail. Reviewing the ERP contract, needs clarification on the payment milestone schedule before signing. Polite, slightly urgent - wants this resolved this week.

    2. [Fabrikam Industries] Subject: "Feature Request - Barcode Scanning & Warehouse Integration." From: Marcus Webb, IT Director, Fabrikam Industries. Requests barcode scanning and warehouse-management integration be added to the ERP build; needed for their distribution centers. Leave this request open/unresolved in tone.

    3. [Tailspin Toys] Subject: "URGENT: Production Issue Affecting Order Processing." From: David Chen, IT Support Lead, Tailspin Toys. Urgent tone - a production issue is blocking order processing right now, needs immediate attention, asks for a callback ASAP. Leave this issue open/unresolved in tone.

    4. [PMO] Subject: "Invitation – Steering Committee Meeting." Short agenda (3–4 bullet points covering Project Orion milestones, budget status, go/no-go checkpoints), a list of expected attendees (by role, not real people — e.g., Steering Committee members, Project Sponsor, PMO), a placeholder Teams link, and a note that a deck is attached.

    5. [PMO – Risk Management] Subject: "Risk Review Meeting – Follow-Up Notes." Summarizes 3 decisions made in a recent risk review, each with an owner name and a due date.

    Once all 5 are sent, reply with only the word "Done."
    ```

    ![](./media/image16.png)

2.  After submitting the prompt, you can see that Cowork has started **processing** the request with the steps visible in the workspace on the right.

    ![](./media/image17.png)

    > **Note:** Cowork may send all 5 emails automatically without showing individual **Send** approval cards, as the prompt grants upfront approval. If no approval cards appear and Cowork replies **Done**, this is expected - skip to step 6 and continue.

    ![](./media/image18.png)

3.  Review the email generated by Cowork and click on **Send** to approve it.

    ![](./media/image19.png)

4.  Review the second email generated by Cowork and click on **Send** to approve it.

    ![](./media/image20.png)

    > **Note:** Repeat the same steps and approve all the remaining 3 emails generated by Cowork.

5.  Review the output generated with all 5 email details listed.

    ![](./media/image21.png)

6.  To verify the emails were generated, click on the **Microsoft 365 app launcher (1)** and select **Outlook (2)**.

    ![](./media/image22.png)

7.  If the **Your privacy matters** popup appears, click on **Continue**.

    ![](./media/image23.png)

8.  Go to **Inbox (1)** and confirm that all the **sample emails (2)** are present.

    ![](./media/image24.png)

## Task 3: Generate Sample Calendar Events in Outlook

In this task, you will use Cowork to create 3 sample calendar events in Outlook to build out a realistic project calendar.

1.  Go back to Microsoft 365 Copilot portal and in the Cowork pane, enter the below prompt **(1)** and click the **send (2)** button:

    ```
    I need you to create 3 sample calendar events on my Outlook calendar for a Copilot Cowork demo environment (Contoso Electronics / Project Orion ERP modernization scenario). Create all 3 without pausing for individual confirmation, then give me a summary table at the end (event title, date, time) once done.

    ## Rules for every event

    - I am the only attendee/organizer — do NOT invite or add any other person's email address, even if a name or company is mentioned. Any names/companies mentioned should appear as plain text in the description only.
    - Add a Microsoft Teams meeting link to each event.
    - Schedule them on the next 3 consecutive business days starting tomorrow (skip weekends), one per business day, in the order below.
    - If any time conflicts with something already on my calendar, shift only that one event by 30 minutes and note it in your summary.

    ## The 3 events

    Business day 1 — 2:00–3:00 PM
    Title: Steering Committee Review
    Description: Agenda: review of Project Orion milestones, budget status, and go/no-go checkpoints.
    Attendees (for reference only, do not invite): Steering Committee members, Project Sponsor, PMO.

    Business day 2 — 10:00–11:00 AM
    Title: Security Assessment Meeting
    Description: Agenda: review of vulnerability assessment findings (high-risk and medium findings) and required remediation plan.
    Attendees (reference only): Security Team, Compliance Officer, IT Director.

    Business day 3 — 10:00–11:30 AM
    Title: Go-Live Readiness Review
    Description: Agenda: walkthrough of the deployment readiness checklist (servers, backup, disaster recovery, monitoring), outstanding approval items, and the go-live decision.
    Attendees (reference only): Executive Sponsor, Infrastructure Lead, PMO, QA Lead.

    Once all 3 are created, reply with only the word "Done."
    ```

    ![](./media/image25.png)

2.  After submitting the prompt, you can see that Cowork has started **processing** the request.

    ![](./media/image26.png)

    > **Note:** Cowork may create all 3 events automatically without showing individual **Save** approval cards. If no approval cards appear and Cowork replies **Done**, this is expected - skip to the step 5 and continue.

3.  Review the event generated by Cowork and click on **Send** to approve it.

    ![](./media/image27.png)

    > **Note:** Repeat the same steps and approve the remaining 2 events generated by Cowork.

4.  Review the output generated with all 3 event details listed.

    ![](./media/image28.png)

5.  Navigate back to Outlook and select the **Calendar icon (1)** from the left. Go to **Month (2)** at the top and review all **three events (3)** listed.

    ![](./media/image29.png)

    ![](./media/image30.png)

## Task 4: Upload Sample Files to OneDrive and Create a Team in Microsoft Teams

In this task, you will upload sample folders and files to OneDrive, then create a team and channel in Microsoft Teams for use in later labs.

1.  On the Microsoft 365 Copilot portal, open the **Microsoft 365 app launcher (1)** and select **OneDrive (2)**.

    ![](./media/image31.png)

2.  If the **Work smarter with Copilot** popup appears, click on **Not now** and continue.

    ![](./media/image32.png)

3.  On OneDrive, navigate to **My files**.

    ![](./media/image33.png)

4.  Click on **Create or upload (1)** and select **Folder (2)** to create a new folder.

    ![](./media/image34.png)

5.  Name the folder Lab Files **(1)** and click on **Create (2)**.

    ![](./media/image35.png)

6.  Verify that the **Lab Files** folder is created and click on it to navigate inside.

    ![](./media/image36.png)

7.  In **Lab Files**, click on **Create or upload (1)** and select **Folder upload (2)**.

    ![](./media/image37.png)

8.  Navigate to the path C:\LabFiles\lab file **(1)**, select **ArchiveCandidates (2)**, and click **Upload (3)** to complete the upload.

    ![](./media/image38.png)

9.  If you see a popup asking for permission to upload the files then click on **Upload**.

    ![](./media/image39.png)

    > **Note:** Repeat this process and upload all the remaining folders into Lab Files except the **Project Orion Files** folder.

10. Once done uploading, verify that all four folders are visible, then click on **Create or upload (1)** and select **Files upload (2)**.

    ![](./media/image40.png)

11. Navigate to the path C:\LabFiles\lab file **(1)**, select **all four files (2)**, and click **Open (3)** to complete the upload.

    ![](./media/image41.png)

12. Verify that all the folders and files are visible, then navigate back to **My files**.

    ![](./media/image42.png)

13. Click on **Create or upload (1)** and select **Folder upload (2)**.

    ![](./media/image43.png)

14. Navigate to the path C:\LabFiles\lab file **(1)**, select **Project Orion Files (2)**, and click **Upload (3)**.

    ![](./media/image44.png)

15. If you see a popup asking for permission to upload the files then click on **Upload**.

    ![](./media/image45.png)

16. Verify that the **Project Orion Files** folder appears in the list.

    ![](./media/image46.png)

17. Go back to the Microsoft 365 Copilot portal, open the **Microsoft 365 app launcher (1)**, and select **Teams (2)**.

    ![](./media/image47.png)

18. On the **Get to know Teams** pop up click on **Get Started**.

    ![](./media/image48.png)

19. Click **X** and close the tab with QR code.

    ![](./media/image49.png)

20. In the Teams browser, click on **See all your teams (1)** and select **Create team (2)**.

    ![](./media/image50.png)

    ![](./media/image51.png)

21. Add the team name as **Retail (1)**, the first channel name as **General (2)**, and click on **Create (3)**.

    ![](./media/image52.png)

22. Click on **Skip** on the **Add members to Retail** page.

    ![](./media/image53.png)

23. Verify that the team **Retail** and channel **General** have been created on the left.

    ![](./media/image54.png)

## Task 5: Explore Work Context, Task History, and Scheduled Tasks

In this task, you will explore how Cowork surfaces your seeded data as work context, search your task history, schedule a recurring task, and browse suggested task ideas.

1.  Navigate back to Copilot. Click on the **New task** from the left.

2.  Click the **"+" (1)** icon, review the options present, and select **Add work context (2)**.

    ![](./media/image55.png)

3.  Navigate through each tab and review what it shows.

    ![](./media/image56.png)

4.  Click on **My tasks (1)** from the left and type **email (2)** in the search bar. The list filters in real time to tasks containing that word.

    ![](./media/image57.png)

5.  Click the **"..." (1)** icon on any task row to review the options available to rename or delete the task.

    ![](./media/image58.png)

6.  Select **Automations (1)** in the left panel and click on **Add (2) \> Create with Cowork (3)**.    

    ![](./media/image59.png)

7.  After clicking on Create, you can see that Cowork has started **processing** the request. Click on **Send**.

    ![](./media/image60.png)

8.  Review the recommendations provided by Cowork, select the **option (1)** that best aligns with your interest, and click **Next (2)**.

    ![](./media/image61.png)

    ![](./media/image62.png)

9.  Schedule the **time (1)** as per your need and click **Next (2)**.

    ![](./media/image63.png)

10. Click on **Email to me (1)** under How should you get the results? and click on **Submit (2)**.

    ![](./media/image64.png)

11. Click on **Schedule** to approve the request for creating a scheduled task.

    ![](./media/image65.png)

12. On Send Email pop up, click on **Always allow**

    ![](./media/image66.png)

13. Verify that Cowork has processed the request and generated the output.

14. Click on **Automations (1)** and, under **All**, verify that the **Weekday Morning Prep Briefing (2)** task is scheduled.

15. Click on **New task (1)** and select **Show more (2)** next to the "Try these next" section.

    ![](./media/image67.png)

16. Review all the topics presented one by one.

    ![](./media/image68.png)

17. Search and select **Meeting briefing (2)**.

    ![](./media/image69.png)

18. Click on **Use this task**.

    ![](./media/image70.png)

19. Read the prompt, then press Escape twice or clear the task bar without running it.

    ![](./media/image71.png)

## Review

In this lab, you completed the following:

- Signed in to Microsoft 365, explored the Copilot Cowork home screen, and reviewed how starter tiles pre-fill ready-to-run prompts

- Explored the Customize area to review available plugins and built-in skills

- Generated sample emails and calendar events in Outlook using Cowork

- Uploaded sample files to OneDrive and created a team and channel in Microsoft Teams

- Explored the + menu and reviewed the work-context sources available to a task

- Searched task history, created a recurring scheduled task, and browsed suggested task ideas

**You have successfully completed the Lab!**

Now, click on **Next \>\>** from the lower right corner to move on to the next page.

    ![](./media/image72.png)
