**MICROSOFT 365 COPILOT COWORK \| LAB GUIDE**

# Lab 5: Building a Personal Work Dashboard with Microsoft Copilot Cowork (Read Only)

| EST. DURATION | TASKS | STEPS |
| --- | --- | --- |
| 30 min | 5 | 32 |

## Overview

Modern knowledge workers spend a significant amount of time switching between Outlook, Teams, Calendar, and OneDrive to identify priorities and track ongoing work. Microsoft Copilot Cowork enables users to automate these repetitive activities by orchestrating Microsoft Graph data, generating personalized outputs, and scheduling recurring tasks that continuously refresh with the latest information.

In this lab, you will use Microsoft Copilot Cowork to build a personalized HTML work dashboard that consolidates important information from Microsoft 365 services into a single, interactive view. You will configure Cowork to gather data from Outlook, Teams, Calendar, OneDrive, and Microsoft Search, generate a visually rich dashboard with actionable insights, schedule automatic refreshes, and customize the dashboard to suit your preferences. By the end of the lab, you will have an automated work dashboard that provides a centralized view of your daily priorities while demonstrating how Copilot Cowork can streamline personal productivity workflows.

> **Note:** This is a read-only lab intended to introduce the key concepts and capabilities of building automated dashboards in Microsoft 365 Copilot Cowork. No hands-on activities are performed in this exercise, in order to manage credit consumption for the workshop. Participants will gain the foundational knowledge needed to understand how dashboards are built, customized, and scheduled to refresh.

## Objectives

In this lab, you will perform the following:

- **Task 1:** Sign In and Navigate to Copilot Cowork

- **Task 2:** Build a Dashboard Using Cowork

- **Task 3:** Schedule the Hourly Refresh

- **Task 4:** Explore and Customize the Dashboard

- **Task 5:** Manage Scheduled Tasks

## Task 1 - Sign In and Navigate to Copilot Cowork

In this task, you will sign in to Microsoft 365 Copilot and navigate to the Cowork experience, ensuring your environment is ready to build and automate AI-powered productivity workflows.

1.  Open your browser and navigate to **Microsoft 365 Copilot** using the URL

    ```
    https://m365.cloud.microsoft
    ```

2.  On the **Microsoft 365 Copilot** page, click **Sign in**.

    ![](./media/image1.png)

3.  You'll see the **Sign into Microsoft 365 Copilot** tab. Here, enter your **credentials (1)** and select **Next (2)**:

- **Email/Username**

    ![](./media/image2.png)

4.  Next, provide **Temporary Access pass**, and select **Sign In (2)**:

- Enter **Temporary Access Pass**

    ![](./media/image3.png)

5.  If **Action required** pop-up window appears, click on **Ask later**.

6.  If prompted to **stay signed in**, you can click **No**.

    ![](./media/image4.png)

7.  Confirm you land on the Microsoft 365 home page.

    ![](./media/image5.png)

8.  Click on the **Cowork** tab in the left navigation menu , to switch to Cowork

    ![](./media/image6.png)

## Task 2 - Building Dashboard using Cowork

In this task, you will use Microsoft Copilot Cowork to generate a personalized HTML work dashboard by gathering information from Outlook, Teams, Calendar, OneDrive, and Microsoft Search. The dashboard will provide a centralized view of your meetings, emails, projects, and other important work items.

1.  In the task input box, enter the following prompt (1) and then click the **Submit (2)** icon.

    ```
    Build me a personal work dashboard as a single HTML file at output/dashboard.html.

    Gather fresh data in parallel from across my Microsoft Graph:

    1. Calendar — today's remaining events and the next 7 days, including response status, organizer, and online-meeting status

    2. Inbox — unread, flagged, and high-importance messages from the last few days

    3. Teams — unread chats with last-message previews

    4. OneDrive — recently modified folders in my personal drive

    5. Search M365 for any action-required emails (access renewals, expense reminders, training notices)

    Infer my top 5–8 active projects by clustering recurring meetings, email threads, and customer names. Surface a "Next" action for each.

    Render a single-page HTML dashboard with this layout:

    - Header: greeting with today's date, last-refresh timestamp (Pacific time), "Click any item to open it" hint

    - KPI strip (6 tiles): overdue actions, unread emails, meetings tomorrow, Teams unread, active projects, OOF this week. Color the urgent ones red, warnings amber, healthy ones green.

    - Urgent banner (red-bordered): items that need attention today

    - Tomorrow's Schedule card: every event with time chip, title, response badge, organizer, conflict markers

    - Prep Notes card: short crib sheets for meetings that need prep

    - Top Projects card: inferred projects with a "Next" line each

    - Week Calendar Load: pure CSS bar chart of meeting counts per day for the upcoming week (flex-aligned `<div>` bars with `linear-gradient` fills and inline `style="height: NN%"`)

    - Time Allocation: pure CSS doughnut chart splitting the week by category (`<div>` with `conic-gradient` background and a `::after` hole, paired with a static legend)

    - Emails Needing a Reply card: the few messages that actually want a response — filter out newsletters, alerts, external pitches

    - Long-Term Action Items card: overdue tasks, weekly deadlines, upcoming milestones

    - Training & Learning card: upcoming training sessions

    - OOF Radar card: teammates out this week & next, with a heads-up if any organize a meeting I'm attending

    - People to Follow Up With card: name + one-line context

    - Unread Teams Chats card: top chats with one-line previews

    - Recent Files in Flight card: most recently modified OneDrive folders

    - Footer: refresh schedule note

    Visual style: soft blue gradient background (#f5f7fa to #e8edf3), rounded white cards with subtle shadow, 'Segoe UI' font, Microsoft accent #0078d4, color-coded badges (green #dcfce7/166534 = accepted, amber #fef3c7/92400e = tentative, red #fee2e2/991b1b = no response or overdue, purple #ede9fe/5b21b6 = organizer). Use a 2-column grid for the main sections, 3-column for the smaller cards, collapsing to single column under 1024px.

    PORTABILITY REQUIREMENT — the file must render correctly with zero external network requests and zero JavaScript executing. No `<script src="...">` to any CDN. No Chart.js, D3, or other charting libraries. No external fonts (use the system 'Segoe UI' stack). All charts must be built from HTML + CSS only: bar chart = flex-aligned gradient `<div>` bars; doughnut = `conic-gradient` background with a `::after` pseudo-element hole. All KPI tiles must render their final value directly in the HTML — never start at `0` and rely on JS to fill in the number. Any animation or interactivity (slide-up entry, pulse dot, dark mode toggle) is allowed but must be additive: CSS-driven where possible, and any inline script must gracefully no-op if blocked (e.g. wrap `localStorage` access in `try/catch`). The dashboard will be opened in sandboxed previews, email-attachment viewers, and locked-down browsers where scripts and CDNs frequently do not run.

    Premium touches to include (all must work without JavaScript or external requests):

    - Dark mode toggle in the header (pill button with sun/moon icon, CSS-variable theming). Persist preference via `localStorage` wrapped in `try/catch` so it gracefully no-ops where storage is blocked. The page must render correctly in light mode by default even if the toggle script never runs.

    - KPI tiles render their final value directly in the HTML (e.g. `<div class="kpi-value">22</div>`). Optional polish: a CSS-only entry animation (e.g. `@keyframes` opacity/translate). Do not start the tile text at `0` and rely on JS to count it up — that breaks in any context where scripts don't execute.

    - Slide-up entrance animation on KPI tiles and cards via pure CSS `@keyframes`.

    - 3-color header gradient (#0078d4 → #00bcf2 → #5e60ce) with radial-gradient overlay highlights.

    - Pulse dot animation on the "Last refreshed" timestamp via pure CSS `@keyframes`.

    - CSS bar chart for Week Calendar Load — `<div>` columns whose heights are inline `style="height: NN%"` percentages. Fill classes: `.heavy` (red `linear-gradient` when count ≥ 7), `.light` (gray when = 2), `.normal` (blue otherwise). Number labels sit at the top of each bar in white text.

    - CSS doughnut for Time Allocation — `<div class="donut">` with `conic-gradient(...)` background, segment angles computed at build time from the percentages, and a `::after` pseudo-element using the card background color to punch out the center hole. Render the legend as static HTML next to it.

    - Project health dots next to each project name — red (hot), green (active), amber (watch), with a soft box-shadow glow.

    - Avatar initials circles on the People card (avatar-1 through avatar-5 with gradient backgrounds).

    - Decorative ⚠ watermark in the urgent banner using a `::before` pseudo-element.

    CRITICAL — every item must be clickable. Wrap every event, email, chat, file, project card, training item, action item, and person in an <a href="..." target="_blank"> anchor tag:

    - Calendar events → fetch via QueryGraph on /me/calendarView with $select including webLink; use the event's webLink

    - Emails → fetch via QueryGraph on /me/messages with $select including webLink; use the message's webLink

    - Teams chats → fetch via QueryGraph on /me/chats with $select including webUrl; use the chat's webUrl

    - OneDrive folders → use the item's webUrl

    - People → mailto:<email> for email follow-ups, or the 1:1 chat webUrl for Teams follow-ups

    - Project cards / training items without a canonical link → use an Outlook inbox search URL like https://outlook.office.com/mail/inbox?searchquery=<keyword>

    Style anchors with class names so they look like regular cards (color: inherit; text-decoration: none; display: block or flex; subtle hover background).

    Save to output/dashboard.html. After writing, confirm the file exists in output/.
    ```

    ![](./media/image7.png)

2.  Observe that **Copilot Cowork** is processing the request, gathering data across your **calendar**, **inbox**, **Teams**, and **OneDrive** in parallel, as shown under the **Steps** panel on the right.

    ![](./media/image8.png)

    > **Note:** Cowork can take upto 5-10 minutes to complete the task

3.  Verify that all steps are completed under **Workspace**, and that the **dashboard.html** file is generated under **Output**, then click on the **dashboard** file to view the result.

    ![](./media/image9.png)

4.  Verify that the **dashboard.html** file opens successfully, displaying a personalized dashboard with KPI cards for **Overdue Actions**, **Unread Emails**, **Meetings Tomorrow**, **Teams Unread**, **Active Projects**, and **OOF This Week**, along with a **Needs your attention today** section.

    ![](./media/image10.png)

5.  Under **Output**, click the **more options (1)** icon next to **dashboard.html**, and review the available options: **Download**, **Open in OneDrive**, **Open location**, and **Copy link**.

    ![](./media/image11.png)

## Task 3 - Schedule the Hourly Refresh

In this task, you will configure a recurring Cowork task to automatically refresh your work dashboard throughout the day. You will also verify that the scheduled task executes successfully and updates the dashboard with the latest information.

1.  In the task input box, enter the following prompt (1) and then click the **Submit (2)** icon.

    ![](./media/image12.png)

    ```
    Set up a scheduled task that refreshes output/dashboard.html every weekday at :55 past the hour, from 6:55 AM through 5:55 PM Pacific time - auto-detect this from the device/browser's local timezone rather than the account's configured IST setting, and don't ask me to confirm it. If the device timezone can't be detected, default to America/Los_Angeles and proceed without asking.
    Use the same data-gathering and rendering instructions from the dashboard we just built - capture webLink/webUrl for every item so links stay clickable on every refresh.
    At the 9 AM Pacific run only (and no other hour), also send me an email:

    To: odl_user_2439755@sandboxailabs1012.onmicrosoft.com
    Subject: "Your Daily Work Dashboard - [today's date in M/D format]"
    Body: brief greeting noting the dashboard is attached, every item is clickable, and the in-session version refreshes hourly
    Attachment: output/dashboard.html

    For all other hours, refresh the file silently - no email.
    Handle daylight saving automatically by re-deriving the Pacific offset at each run rather than hardcoding it, so the :55 anchor never drifts.
    Name the task "Refresh work dashboard (hourly at 9 AM, email at 9 AM)"
    ```

2.  On the **Create recurring task?** prompt, review the **Name**, **Repeat**, **Run in**, and **Description** details, ensure **Run once now** is checked, then click **Next** and then **schedule**.

    ![](./media/image13.png)

    ![](./media/image14.png)

3.  Confirm that the message **"Done — your scheduled task is now active"** is displayed, verifying that the **Refresh work dashboard** task has been scheduled successfully.

    ![](./media/image15.png)

4.  Under **Workspace**, verify that the **Refresh work dashboard** task is listed under **Scheduled task**, running **Every week**, and click on it to open the task.

    ![](./media/image16.png)

5.  On the **Refresh work dashboard** blade, verify that the task status is **Active**.

    ![](./media/image17.png)

6.  Click **Run now** to trigger the scheduled task immediately.

    ![](./media/image18.png)

7.  Verify that the task ran successfully, confirming a **silent refresh, no email** since it ran outside the **9:55 AM Pacific** window, with the **dashboard.html** file updated with the latest **Last refreshed** timestamp.

    ![](./media/image19.png)

8.  Under **Output**, click on the **dashboard.html** file to view the refreshed dashboard.

    ![](./media/image20.png)

9.  Verify that the **dashboard.html** file displays the updated **Last refreshed (1)** timestamp, confirming the dashboard has been refreshed successfully.

    ![](./media/image21.png)

## Task 4 - Explore and Customize the Dashboard

In this task, you will review the generated dashboard, explore its interactive sections, customize its appearance and content, and save your preferred layout for future dashboard generations.

1.  Go through the **dashboard.html** file and review all the sections available, including **Overview**, **Needs your attention today**, **Tomorrow's Schedule**, **Prep Notes**.**Week Calendar Load** and **Time Allocation**.

    ![](./media/image22.png)

    ![](./media/image23.png)

2.  On the **dashboard.html** file, click on **Theme (Light/Dark button)** to toggle between light and dark mode.

    ![](./media/image24.png)

3.  Verify that the **dashboard.html** file switches to **dark mode**.

    ![](./media/image25.png)

4.  Navigate back to the **Cowork** chat, then in the message box, enter **"Lock this dashboard format in for all future ones" (1)** and click **Submit (2)**.

    ![](./media/image26.png)

5.  Allow the **Always allow Copy artifact** pop-up. Then click **Approve** again.

    ![](./media/image27.png)

    ![](./media/image28.png)

6.  Verify that the message **"Locked in"** is displayed, confirming that the dashboard format has been saved as the standing house style for future requests.

    ![](./media/image29.png)

7.  In the message box, enter **"Remove the training and learning card" (1)** and click **Submit (2)**. Then **approve** the edit schedule task.

    ![](./media/image30.png)

    ![](./media/image31.png)

8.  Verify that the message confirms the **Training & Learning card** has been removed from both the live dashboard and the locked-in standard.

    ![](./media/image32.png)

9.  Click **dashboard.html** in the Output section to open and review the changes.

    ![](./media/image33.png)

## Task 5 - Manage Scheduled tasks

In this task, you will review the scheduled dashboard automation, explore the available management options, and verify how recurring Cowork tasks can be monitored and maintained.

1.  Click the **Cowork (1)** tab and then select **Automations** **Scheduled**.

2.  Confirm the schedule is now active, click the ellipsis icon to review the **Edit**, **Run now**, **Pause**, and **Delete** options.

    ![](./media/image34.png)

## Review

In this lab, you used Microsoft Copilot Cowork to create a personalized HTML work dashboard that consolidated information from Outlook, Teams, Calendar, OneDrive, and Microsoft Search into a single interactive view. You verified that the generated dashboard displayed key productivity insights, including upcoming meetings, unread emails, active projects, Teams activity, recent files, and priority actions.

You then automated the dashboard by creating a recurring scheduled task that refreshes the dashboard throughout the workday and delivers a daily email containing the updated dashboard at the designated time. After validating the scheduled task and confirming the dashboard refreshed successfully, you explored the generated dashboard, customized its appearance and content, and saved your preferred layout for future dashboards. Finally, you reviewed and managed the scheduled automation task, gaining experience with maintaining recurring Copilot Cowork workflows.

You have successfully built, automated, customized, and managed a personal productivity dashboard using Microsoft Copilot Cowork, demonstrating how AI-powered workflows can simplify daily work management and provide timely, actionable insights across Microsoft 365.

### You have successfully completed the Lab!

Now, click on **Next \>\>** from the lower right corner to move on to the next page.

![](./media/image35.png)
