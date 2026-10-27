**MICROSOFT 365 COPILOT COWORK \| LAB GUIDE**

# Lab 2: AI-Powered Calendar Optimization and Executive Meeting Coordinator

| EST. DURATION | TASKS | STEPS |
| --- | --- | --- |
| 30 min | 3 | 21 |

## Overview

In this hands-on lab, you will use Copilot Cowork, the agentic layer of Microsoft 365 Copilot, as an AI-powered executive assistant that optimizes your calendar and coordinates your meetings across Outlook Calendar, Outlook mail, Microsoft Teams, and OneDrive. Rather than manually protecting focus time, finding meeting slots, or checking which commitments clash with your plans, you will instruct Cowork in plain language and let it handle the work. You will apply executive-style standing rules across an entire week, schedule new meetings and generate a one-page prep brief for an executive meeting, and then run a discovery pass that detects conflicts with your upcoming time away and resolves them through an approved handoff. Throughout the lab, watch the Workspace panel on the right, which tracks the steps of Cowork’s plan and the plugins it uses, and the approval cards that appear in the conversation. Cowork waits for you to approve each card before it makes any calendar or email change, a human-in-the-loop design that matters most for bulk edits.

## Objectives

In this lab, you will perform the following:

- **Task 1:** Executive Calendar Management

- **Task 2:** Intelligent Meeting Scheduling

- **Task 3:** Conflict Detection and Resolution

## Task 1: Executive Calendar Management

In this task, you will set standing rules for Cowork to apply across next week: protecting focus time, declining meetings that have no agenda, and keeping Friday afternoon free. Cowork proposes every change as one batch for your review before anything is added to your calendar.

1.  In Microsoft 365 Copilot, make sure the **Cowork** tab is selected, click **New task**, enter the prompt below in the message box, and click the **Send** button:

    ```
    Act as my executive assistant. Apply these standing rules to next week: block two 90-minute focus blocks before noon; decline meetings with no agenda after asking the organizer for one; keep Friday afternoons free; and summarize every change you make for my approval before applying it.
    ```

    ![](./media/image1.png)

2.  Review the proposed changes. Cowork checks your calendar for next week, confirms your mailbox time zone and working hours, and lists each proposed change in a numbered table with its date, time, and **Shows as** status. Notice that Cowork states that nothing has been applied yet.

    ![](./media/image2.png)

    > **Note:** Cowork may respond a little differently from the screenshots. For example, it may first ask a few clarifying questions, or it may show the **Create calendar event?** approval cards straight away. If this happens, answer the questions based on your preference (or select the recommended option) and click **Send** or **Next**. If the approval cards appear directly, skip Step 3 and continue with Step 4.

3.  Scroll down to review the rest of the proposal, including the Friday afternoon **Keep free – no meetings** hold and the **How I read your rules** notes. Then type **Approve all** in the **Message Cowork** box and click the **Send** button.

    ![](./media/image3.png)

4.  Cowork displays a **Create calendar event?** approval card for each item: the **Focus Block 1** and **Focus Block 2** series that repeat Monday to Friday, and the Friday afternoon hold. On each card, review the date, time, repeat pattern, and title, and then click **Save**. Repeat until you have saved every card.

    ![](./media/image4.png)

5.  Review the confirmation summary. Cowork shows **Approved 3 actions** and a day-by-day table for next week with both focus blocks on every weekday and the **Keep Free – No Meetings** hold on Friday afternoon, each shown as Busy.

    ![](./media/image5.png)

## Task 2: Intelligent Meeting Scheduling

In this task, you will ask Cowork to add two meetings to your calendar for next week and confirm their final times. You will then have it prepare you for your upcoming Steering Committee Review by building a one-page prep brief as a Word document, using data it gathers from your calendar, email, and OneDrive, and saving the brief to OneDrive.

### Schedule New Meetings

1.  Stay in the **Executive Assistant Calendar Rules** task from Task 1. In the **Message Cowork** box, enter the prompt below and click the **Send** button:

    ```
    Add these 2 meetings to my Outlook calendar, covering next Monday and Thursday. I am the only attendee/organizer on both — do not invite anyone else, use only my own email if an attendee field is required. Add a Teams meeting link to each.

    - Monday: "Client Status Call – Northwind Account" — 10:00–10:30 AM
    - Thursday: "Budget Review – Phase 3 Sign-off" — 2:00–2:30 PM

    Confirm each one's final date/time in a summary table.
    ```

    ![](./media/image6.png)

2.  Cowork displays a **Create calendar event?** approval card for each meeting. Review the date, time, and title on both cards, and click **Save** on each one to approve it.

    ![](./media/image7.png)

3.  Review the summary table. Cowork confirms that both meetings were added with you as the only attendee and a Teams meeting link: **Client Status Call – Northwind Account** on Monday from 10:00 to 10:30 AM, and **Budget Review – Phase 3 Sign-off** on Thursday from 2:00 to 2:30 PM.

    ![](./media/image8.png)

    > **Note:** Because you scheduled these meetings in the same task, Cowork checks them against the focus blocks you created in Task 1. It flags that the Monday call falls inside **Focus Block 2** (10:00–11:30) and offers to move or shorten that block. Cowork only proposes this change and does not move anything unless you approve it, so you can continue with the lab without replying.

### Generate an Executive Meeting Prep Brief

4.  In the left pane, click **New task**, enter the prompt below, and click the **Send** button:

    ```
    Prepare me for my Steering Committee Review meeting for Project Orion.

    Gather from these three sources only:
    - My calendar: that meeting's details and attendees
    - My email: Project Orion messages from the last 7 days
    - My OneDrive "Project Orion Files" folder

    Produce a one-page prep brief as a Word document containing: attendee list with my last interaction with each, the stated agenda and purpose, related email threads and files, open action items, and the decisions needed. Save it to my OneDrive "Lab Files" folder.

    Keep your final confirmation to one line.
    ```

    ![](./media/image9.png)

5.  Monitor Cowork as it works. It names the task **Steering Committee Prep Brief for Orion**, and the **Working on it** section shows each action as it runs, such as listing the contents of the **Project Orion Files** folder. In the **Workspace** panel, **Steps** tracks the plan (finding the meeting, reviewing Project Orion emails and files, writing the prep brief, and saving it to your Lab Files folder), and **Plugins** shows the sources in use: Calendar, SharePoint, and Outlook.

    ![](./media/image10.png)

6.  When Cowork is ready to save the brief, it displays an **Approve action?** card. Confirm that the **Parent path** is **Lab Files**, review the **File name**, and click **Approve**.

    ![](./media/image11.png)

7.  Review Cowork’s confirmation that the prep brief is saved in your OneDrive **Lab Files** folder, and then click the Word document card to open the brief.

    ![](./media/image12.png)

8.  Review the prep brief. Verify that it includes the meeting purpose and agenda, the attendee list with your last interaction with each attendee, the related email threads and files, the open action items, and the decisions needed.

    ![](./media/image13.png)

## Task 3: Conflict Detection and Resolution

In this task, you will prepare for a vacation next Monday through Friday. You will ask Cowork to scan your email, calendar, To Do tasks, and Teams, detect the meetings and commitments that conflict with your time away, and show what is at risk along with a proposed action for each item. After you approve the plan, Cowork resolves the conflicts by carrying out the handoff.

1.  In the left pane, click **New task**, enter the prompt below, and click the **Send** button:

    ```
    I'm on vacation next Monday through Friday and returning to work the Monday after. Before I leave, scan the following and flag anything at risk while I'm away:

    - Email: unanswered threads and unsent drafts that need action before I leave
    - Calendar: meetings during my vacation week that conflict with my time away
    - To Do tasks: anything due during my time away or right after I return
    - Teams: unanswered questions directed at me

    Sort findings into 🔴 Must Handle, 🟡 Needs Delegation, and 🟢 Can Wait, with a proposed action for each item.

    Take no action yet - just show me the plan.
    ```

    ![](./media/image14.png)

2.  Wait for Cowork to finish scanning your sources, and then review its response. Cowork first lists any coverage gaps, such as sources it could not access, so you know what to check manually. It then sorts its findings into **Must Handle**, **Needs Delegation**, and **Can Wait**, with a proposed action for each item. Scroll through all three sections.

    ![](./media/image15.png)

    ![](./media/image16.png)

    ![](./media/image17.png)

3.  In the **Message Cowork** box, enter the follow-up prompt below and click the **Send** button:

    ```
    That looks right. Go ahead and handle everything. Show me anything before it goes out, and get my approval before sending or posting anything.
    ```

    ![](./media/image18.png)

4.  Cowork asks a few questions to plan the handoff, such as who should cover for you, how to handle the meetings you organize during your time away, and what to do with unsent drafts. For each question, select the option that suits you and click **Next**. On the last question, click **Submit**.

    ![](./media/image19.png)

    ![](./media/image20.png)

    ![](./media/image21.png)

    > **Note:** Because Cowork uses AI to generate responses, the number and type of questions may differ from the screenshots.
    
    > **Note:** Cowork may show an approval request directly after you answer its questions. If this happens, select the recommended option, click **Next**, and skip Step 6.

5.  Review the plan Cowork builds from your answers, such as a meeting reschedule plan that moves each meeting to your return week and a list of items held until you return. Notice that Cowork has not sent, moved, or cancelled anything yet.

    ![](./media/image22.png)

    ![](./media/image23.png)

6.  Enter the follow-up prompt below and click the **Send** button:

    ```
    Confirm the proposed actions and execute them.
    ```

    ![](./media/image24.png)

7.  Cowork displays an approval card for each action. Review each card and approve it: click **Update** for meeting changes, **Send cancellation** for meetings to cancel, and **Reply** for email replies. When several cards are queued, use the arrows at the top of the card to move between them.

    ![](./media/image25.png)

    ![](./media/image26.png)

    ![](./media/image27.png)

8.  Review Cowork’s completion summary, which confirms that every approved action was carried out, including the new time for each rescheduled meeting.

    ![](./media/image28.png)

## Review

In this lab, you completed the following:

- Applied executive-style standing rules across an entire week and reviewed every proposed change before it was applied

- Scheduled new meetings with Cowork and confirmed their final dates and times in a summary table

- Built an AI-generated executive meeting prep brief as a Word document, combining calendar, email, and file data gathered in parallel by Cowork

- Ran a full discovery pass across email, calendar, tasks, and Teams to detect conflicts with your time away, then approved Cowork's proposed resolution and handoff actions

### You have successfully completed the Lab!

Now, click on **Next \>\>** from the lower right corner to move on to the next page.

![](./media/image29.png)
