# Lab 6 – Building Custom Cowork Skills

| Item | Details |
|------|---------|
| **Estimated Time** | 20 minutes |
| **Objective** | Build two custom skills using Copilot Cowork's conversational AI Skill Builder, then publish the skill output to a Microsoft Teams channel. |

# Before You Start: What Is a Custom Skill?

A Custom Skill is a saved workflow Cowork follows whenever you call it
by name. You describe what you want once, Cowork builds and saves it,
and from then on one sentence triggers the full workflow automatically.

> [!NOTE]
> The **Skill Builder** is fully conversational. Instead of filling out forms or writing code, simply describe the skill you want to create. Copilot Cowork asks follow-up questions, gathers the required information, and generates the skill automatically.

# Exercise 1: Design Your Skill on Paper First

Before touching any tool, spend 5 minutes planning. A clear spec leads
to a much better skill. Rushing straight to the builder is the most
common reason skills turn out vague and unreliable.

## Step 1 — Open your browser and navigate to Cowork

1.  Open your browser.

2.  Click the address bar at the very top of the window and type:
    m365.cloud.microsoft — then press Enter.

3.  Click the first autocomplete result — m365.cloud.microsoft — and
    sign in with your lab account credentials.

4.  After signing in, you land on the Microsoft 365 Copilot interface.
    Click the Cowork tab at the top of the left panel.

***What you should see:***

- The Cowork home screen is loaded with the Cowork tab selected.

- LEFT PANEL: New task (blue), Search, Scheduled, Customize, and recent
  task history.

- MAIN AREA: ‘What can I do for you?’ heading, task bar, Up next tasks,
  and Try these next tiles.

> **Action:** Your Cowork home screen is confirmed. Do not click
> anything yet — proceed to Step 2.

## Step 2 — Open Notepad alongside the browser

5.  Press the Windows key on your keyboard and type: Notepad — then
    click the app when it appears.

![](./media/image1.png)

***What you should see:***

- The Windows Start menu search overlay appears.

- Under Best match: Notepad is highlighted in blue, cursor pointing at
  it.

> **Action:** Click Notepad to open it. Drag / resize it to sit side by
> side with your browser.

6.  Notepad is now open. Type the five planning questions shown below,
    one per line, into the blank Notepad document.

***What you should see:***

- Notepad shows five planning questions:

- What should this skill DO? | What does it need to READ? | Does it
  WRITE or change anything? | What should the output LOOK LIKE? | Is
  there a VARIABLE that might change?

> **Action:** Answer each question in plain English on the next line.
> These answers guide your selections in Exercise 2.

## Step 3 — Fill in your Skill Spec below the questions

7.  Below your five answers, type out the complete Skill Spec template.
    Fill in each field for the Leadership Update skill you are about to
    build.

***What you should see:***

- Notepad shows both sections: the five planning questions and the
  completed Skill Spec below.

- Skill Spec includes: Skill Name, Trigger Phrase, Parameters, Apps It
  May Read, Apps It May Write, Output Format.

> **Action:** Keep Notepad open alongside your browser. Refer to this
> spec when Cowork asks questions. Do NOT paste it into Cowork.

# Exercise 2: Build the Leadership Update Skill

> [!IMPORTANT]
> Earlier versions of this lab described a manual form with fields such as **Name**, **Description**, and **Scope**. The current **Copilot Cowork Skill Builder** no longer uses this form. Instead, the entire skill creation experience is **fully conversational**—Copilot Cowork asks a series of questions, gathers the required information, and generates the skill automatically, as demonstrated in the screenshots throughout this lab.

## Step 1 — Open the Customize area via the + menu

1.  Click the + button at the left side of the task bar on the Cowork
    home screen.

![](./media/image2.png)

***What you should see:***

- A context menu from the + button shows four options:

- \(1\) Add work context (2) Upload images and files (3) Attach cloud
  files (4) Customize — highlighted, sub-text ‘Manage skills & plugins’.

> **Action:** Click Customize (option 4) to navigate to the Customize
> page.

2.  You are now on the Customize page. Click the Skills tab to switch
    from Plugins to Skills.

***What you should see:***

- The Customize page has loaded.

- Two tabs: Plugins (currently active) and Skills (not yet selected).

- Six plugin tiles displayed in a 2×3 grid under Discover.

> **Action:** Click the Skills tab to switch to the skills management
> view.

3.  The Skills tab is now selected. Read both sections before clicking
    anything.

![](./media/image3.png)

***What you should see:***

- The Skills tab is now selected.

- SECTION 1 — Your skills: ‘You haven’t added any skills yet.’

- SECTION 2 — Built-in: three tiles — PDF, Word, Excel.

- Add button with dropdown arrow at the top right.

> **Action:** Click the Add button at the top right to open the
> dropdown.

## Step 2 — Click Add, then Create new to launch the builder

4.  Click the Add button at the top right of the Skills page to open the
    dropdown.

***What you should see:***

- The Add dropdown shows two options: (1) + Create new (highlighted) (2)
  Upload skill.

- Left panel: ‘Creating Personal Skill Definition’ appears at the top of
  the task history.

> **Action:** Click ‘+ Create new’ to launch the conversational skill
> builder.

## Step 3 — Cowork opens the skill builder conversation

5.  After clicking Create new, Cowork opens a new task. Wait for the
    task to fully load before doing anything.
  **Enter the following prompt:**
```
I want to create a new personal skill. Guide me through defining the skill name, description, category, and instructions. Help me write a SKILL.md file and save it to my OneDrive skills folder.
```
![](./media/image4.png)

***What you should see:***

- A new Cowork task has opened with the skill creation prompt in a
  right-aligned bubble.

- Cowork is processing — ‘Working through your request’ spinner is
  visible.

- Workspace panel (right): Skills & Plugins \> Skill Management.

> **Action:** Do not type anything. Wait for the Skill purpose panel to
> appear within a few seconds.

## Step 4 — Choose your Skill purpose

6.  Cowork has responded and a Skill purpose panel has appeared. Read
    all four options before selecting.

***What you should see:***

- Cowork responds: ‘I’d love to help you build this. The one thing I
  need first is the core purpose…’

- Skill purpose panel shows four options: (1) Draft a recurring
  document (2) Format/transform content (3) Communication template (4)
  Data/analysis routine.

> **Action:** Click option 3 — ‘Communication template’. A Submit button
> will appear.

7.  Option 3 Communication template is now selected. Click Submit to
    confirm.

![](./media/image5.png)

***What you should see:***

- Option 3 ‘Communication template’ is now selected — filled dark circle
  on number 3.

- Submit button has appeared at the bottom right.

> **Action:** Click Submit to confirm Communication template as your
> skill purpose.

## Step 5 — Choose the Message type

8.  Cowork has confirmed your choice and is asking a follow-up question.
    Read all four message types before selecting.

![](./media/image6.png)

***What you should see:***

- Message type panel shows four options: (1) Leadership / exec
  update (2) Team announcement (3) Customer / client reply (4) Project
  status email.

> **Action:** Click option 1 — ‘Leadership / exec update’. The Submit
> button will appear.

9.  Read the full description of option 1 Leadership / exec update
    before clicking it.

![](./media/image7.png)

***What you should see:***

- Message type panel shows all four options. Cursor is on option 1 but
  it has NOT been clicked yet — no filled circle, no Submit button
  visible.

> **Action:** Click option 1 ‘Leadership / exec update’ once to select
> it. The Submit button will then appear.

10. Option 1 is selected. Click Submit to start the skill build.

![](./media/image8.png)

***What you should see:***

- Option 1 ‘Leadership / exec update’ is now selected — filled dark
  circle on number 1.

- Submit button has appeared at the bottom right.

> **Action:** Click Submit. Watch the Workspace panel on the right to
> follow the three build steps.

## Step 6 — Watch the Workspace panel as Cowork builds your skill

11. After clicking Submit, watch the Workspace panel on the right side.
    Do NOT click anything.

![](./media/image9.png)

***What you should see:***

- Workspace panel shows Steps 0/3: (1) Validating skill name and
  capacity — open circle (2) Write SKILL.md and save to OneDrive —
  greyed out (3) Validate, score, and report quality — greyed out.

- Chat confirms both your selections were received.

> **Action:** Wait and watch — do not click. The panel advances
> automatically: 0/3 → 1/3 → 2/3 → 3/3.

12. Step 1 of the build is now active. The Workspace panel shows 0/3
    with step 1 spinning.

![](./media/image10.png)

***What you should see:***

- Workspace panel: Steps 0/3 but step 1 now has an active spinning
  circle.

- Steps 2 and 3 are still greyed out. Chat shows ‘Creating your skill’
  spinner.

> **Action:** Continue waiting. Step 1 checks the skill name and will
> complete in a few seconds.

13. Step 1 is now complete. Watch step 2 begin in the Workspace panel.

![](./media/image11.png)

***What you should see:***

- Workspace panel: Steps 1/3. Step 1 has a green checkmark.

- Step 2 ‘Write SKILL.md and save to OneDrive’ is now actively spinning.
  Step 3 still greyed out.

> **Action:** Continue waiting. Cowork is writing the skill file. Watch
> for step 2 to get a checkmark.

14. All three steps are now complete (3/3). Read the output carefully.

![](./media/image12.png)

***What you should see:***

- Workspace panel: Steps 3/3 — all three steps have green checkmarks.

- Output section shows two file links: leadership-upd…SKILL.md and
  skill-quality-report.html.

- Note: a red FAILED badge may appear in chat — this is normal. Cowork
  automatically retried and succeeded.

> **Action:** Do not worry about the red FAILED message. Wait for the
> final completion summary to appear.

15. Cowork has finished. Read the completion summary and note the three
    trigger phrases.

![](./media/image13.png)

***What you should see:***

- Workspace panel: 3/3 all checkmarks. Both output files visible.

- Completion message shows three trigger phrases to use the skill.

- Two output tiles at the bottom: leadership-update (Skill) and
  skill-quality-report.html.

> **Action:** Write down the three trigger phrases — you will use them
> in Exercise 3. Read the full completion message.

16. Hover over the skill-quality-report.html file in the Workspace
    Output section to preview it.

![](./media/image14.png)

***What you should see:***

- Cursor hovers over ‘skill-quality-report.html’ in the Workspace Output
  section.

- A thumbnail pop-up preview of the HTML quality report appears.

> **Action:** Optional: click skill-quality-report.html to read the full
> quality report. Otherwise click elsewhere and proceed to Step 7.

17. Click the three-dot … menu on the leadership-update Skill tile at
    the bottom of the conversation.

![](./media/image15.png)

***What you should see:***

- Workspace panel shows Skills & Plugins expanded with the Skill
  Management button.

- Cursor is clicking the Skill Management button.

> **Action:** Click Skill Management in the Workspace panel, or click
> Customize in the left navigation.

18. Click the X / Close button on the Workspace panel to collapse it.

![](./media/image16.png)

***What you should see:***

- Workspace panel with Close (X) button at the top right.

- Steps 3/3 complete. Output section lists both files.

> **Action:** Click the Close (X) button to collapse the Workspace
> panel.

## Step 7 — Verify the skill appears under Customize \> Skills

19. Click Customize in the left navigation, then click the Skills tab to
    confirm the skill saved correctly.

![](./media/image17.png)

***What you should see:***

- Customize \> Skills page — Skills tab is selected.

- Under ‘Your skills’: the ‘leadership-update’ skill tile is now
  visible.

- Under ‘Built-in’: PDF, Word, Excel unchanged.

> **Action:** Confirm the leadership-update tile is present. Click
> elsewhere to close the Add dropdown, then click the tile to open its
> detail page.

## Step 8 — Read the skill detail and guardrails

20. Click the leadership-update skill tile to open its detail page.

![](./media/image18.png)

***What you should see:***

- The skill detail page for ‘leadership-update-1’ is open.

- Instructions box: Overview, When to Use (3 bullets), When NOT to Use
  (4 bullets — announcements, external messages, formatted file reports,
  scheduling).

> **Action:** Read all four When NOT to Use items — these are the skill
> guardrails. Then click Show more in the description.

21. Click Show more in the description to expand the full text.

![](./media/image19.png)

***What you should see:***

- Full description is now expanded (‘Show less’ replaced ‘Show more’).

- Includes trigger phrases and Do NOT use rules: team announcements →
  stakeholder-comms; full reports → docx.

> **Action:** Read the full description including the Do NOT use rules.
> Then click the back arrow (top left) to return to the Skills list.

# Exercise 3: Test the Leadership Update Skill

A skill is only useful if it runs when you call it. This exercise tests
the skill with a sample input and confirms the Workspace panel activates
correctly.

## Step 1 — Return to the home screen

1.  Click New task in the left navigation panel to return to the Cowork
    home screen.

![](./media/image20.png)

***What you should see:***

- Cowork home screen: ‘What can I do for you?’

- Up next: three recent skill-creation tasks. Try these next tiles at
  the bottom.

> **Action:** Click inside the task bar (‘Start a task…’) and type the
> prompt shown in the next step.

2.  Type the full test prompt into the task bar exactly as shown, then
    press Enter or click the blue send arrow.

![](./media/image21.png)

***What you should see:***

- Task bar shows the multi-line test prompt — starting with ‘Use
  leadership-update-1’, followed by the instruction and sample
  paragraph.

- Blue send arrow is active (filled) at the top right.

> **Action:** Click the blue send arrow or press Enter to submit the
> prompt.

## Step 2 — Read the structured output

3.  Wait for Cowork to generate the output. Read it carefully when it
    appears.

![](./media/image22.png)

***What you should see:***

- Leadership update generated in four sections: HEADLINE — one
  paragraph. PROGRESS — three bullets. RISKS & BLOCKERS — two bullets.
  ASKS / NEXT STEPS — two bullets.

- Workspace panel: Skills & Plugins shows ‘leadership-update’ — confirms
  the skill was activated.

> **Action:** Confirm the output has exactly four sections: Headline,
> Progress, Risks & Blockers, Asks / Next Steps. The skill is working
> correctly.

## Step 3 — Check Customize \> Skills to confirm the skill is still registered

4.  Click Customize in the left navigation, then click the Skills tab.

![](./media/image23.png)

***What you should see:***

- Customize \> Skills page. Skills tab selected.

- Under ‘Your skills’: leadership-update tile listed.

- Left panel: ‘Leadership Update Executive S…’ at top of task history.

> **Action:** Confirm leadership-update is still in Your skills. Click
> New task in the left panel and proceed to Exercise 4.

# Exercise 4: Build the Store Daily Snapshot Skill

Now apply the exact same conversational pattern to a retail operations
scenario. The process is identical to Exercise 2 — only your answers to
Cowork’s questions change.

## Step 1 — Start a new skill build

1.  Click Customize in the left nav, then Skills, then click Add and
    select + Create new.

![](./media/image24.png)

***What you should see:***

- Customize \> Skills page with the Add dropdown open.

- ‘+ Create new’ highlighted at top. ‘Upload skill’ below.

- Your skills shows the leadership-update tile.

> **Action:** Click ‘+ Create new’ to start building the second skill.

## Step 2 — Submit your Store Daily Snapshot spec

2.  A new Cowork task has opened. Wait for the Skill purpose panel to
    appear.

![](./media/image25.png)

***What you should see:***

- New Cowork task is open. Left panel: ‘Create Personal Skill with Doc…’
  highlighted.

- Cowork is processing with a spinner. Workspace panel: Skills & Plugins
  \> Skill Management.

> **Action:** Wait for the Skill purpose panel to appear. Then type your
> Store Daily Snapshot spec into the ‘Describe another option’ field.

3.  The Skill purpose panel has appeared. Type your spec into the
    Describe another option field at the bottom.

![](./media/image26.png)

***What you should see:***

- Skill purpose panel shows four options: (1) Draft recurring
  writing (2) Format/transform content (3) Research & summarize (4)
  Workflow automation.

- ‘Describe another option’ field is PRE-FILLED with: ‘name: Store Daily
  Snapshot, Description: Generates a morning operations brief…’

> **Action:** Type your spec into the Describe another option field, OR
> click option 4 ‘Workflow automation’. Then click Submit.

4.  Your spec has been submitted. Cowork is processing it and narrowing
    down the approach.

![](./media/image27.png)

***What you should see:***

- Skill purpose panel is dismissed.

- A second bubble confirms the spec was received.

- ‘Narrowing down the approach’ spinner is visible.

> **Action:** Wait. Cowork is narrowing down the approach. Watch for the
> Workspace Steps counter to appear.

## Step 3 — Watch all three build steps complete

5.  The Workspace Steps counter has appeared. Watch step 1 start.

![](./media/image28.png)

***What you should see:***

- Workspace panel: Steps 0/3. Step 1 ‘Checking skill name and capacity’
  has an active spinning circle.

- Steps 2 and 3 are greyed out. Chat: ‘Got it — Store Daily Snapshot…
  Let me set up and generate.’

> **Action:** Wait. Step 1 checks that ‘store-daily-snapshot’ is not
> already taken.

6.  Step 1 is complete. Step 2 is now in progress. Watch the Workspace
    panel.

![](./media/image29.png)

***What you should see:***

- Workspace panel: Steps 1/3. Step 1 has green checkmark. Step 2
  ‘Writing and saving the skill’ is actively spinning. Step 3 greyed
  out.

- Chat: ‘Name’s valid… Writing the skill now.’

> **Action:** Wait. Step 2 is writing and saving the SKILL.md — this is
> the longest step.

7.  Step 2 is complete. Step 3 is now validating and scoring the skill.

![](./media/image30.png)

***What you should see:***

- Workspace panel: Steps 2/3. Steps 1 and 2 have green checkmarks. Step
  3 ‘Validate, score, and report’ is now actively spinning.

- Output section shows: store-daily-snapshot-SKILL.md and
  skill-quality-report.html.

> **Action:** Wait. Step 3 is validating the skill structure and
> calculating the quality score.

8.  Step 3 is still running. The validation and quality scoring are in
    progress.

![](./media/image31.png)

***What you should see:***

- Workspace panel: 2/3 advancing to 3/3. Step 3 still spinning.

- Chat: ‘Strong result — let me generate the quality report…’

> **Action:** Wait for the completion summary and Next step dialog.

9.  All steps are complete. The completion summary and Next step dialog
    are loading.

![](./media/image32.png)

***What you should see:***

- Workspace panel: Steps 3/3 — all three steps have green checkmarks.

- Three output tiles at the bottom of the conversation.

> **Action:** Wait a moment longer. The completion message and Next step
> dialog (1 of 2) are about to appear.

## Step 4 — Review the quality score and choose your polish preference

10. The Next step dialog has appeared. Read both options carefully
    before choosing.

![](./media/image33.png)

***What you should see:***

- Next step dialog (1 of 2) shows two options:

- \(1\) ‘Yes, polish it’ — tighten scope and robustness (current score:
  83/100).

- \(2\) ‘Leave it as-is’ — keep 83/100, already clears the publish bar.

> **Action:** Click option 2 ‘Leave it as-is’, then click the Next
> button at the bottom right.

11. Option 2 Leave it as-is is selected. Click Next to advance to the
    Auto-run dialog.

![](./media/image34.png)

***What you should see:***

- Next step dialog (1 of 2): option 2 ‘Leave it as-is’ is now selected —
  filled dark circle on number 2.

- Next button visible at the bottom right. Workspace panel highlighted
  showing all three steps checked.

> **Action:** Click Next to advance to the Auto-run schedule dialog (2
> of 2).

*Before moving to Auto-run, open the quality report to see the score
details:*

12. Click the skill-quality-report.html link to open the quality report
    in a side panel.

![](./media/image35.png)

***What you should see:***

- skill-quality-report.html open in a side panel.

- Score: 83 out of 100.

- Badges: green ‘Meets the bar to publish’, orange ‘Risk: medium’, green
  ‘Grounding: PASS’.

- Checkmarks: ‘It switches on at the right time.’ and ‘It knows what to
  do.’

> **Action:** Read: 83/100 is Good and ready to publish. Risk: medium
> means scope could be tightened. Close this panel and click Next.

## Step 5 — Set the Auto-run schedule

13. The Auto-run dialog has appeared (step 2 of 2). Read all three
    options.

![](./media/image36.png)

***What you should see:***

- Auto-run dialog (2 of 2) shows three options: (1) ‘No, I’ll run it
  manually’ (2) ‘Yes, every weekday morning’ (3) ‘Yes, every day’.

> **Action:** Click option 2 ‘Yes, every weekday morning’, then click
> Submit to register the Monday–Friday schedule.

14. Option 1 is selected in this screenshot — for the lab, select option
    2 instead. Click Submit.

![](./media/image37.png)

***What you should see:***

- Auto-run dialog shows option 1 ‘No, I’ll run it manually’ selected
  (filled circle on 1).

- NOTE: This screenshot shows option 1 — for this lab, select option 2
  ‘Yes, every weekday morning’ instead.

> **Action:** Select option 2 ‘Yes, every weekday morning’ (not option 1
> as shown), then click Submit.

15. Submit is done. Read the final completion message — it confirms the
    skill is ready.

![](./media/image38.png)

***What you should see:***

- Final completion message: ‘Your Store Daily Snapshot skill is ready.’

- Three trigger phrases: ‘give me the store daily snapshot’ | ‘morning
  operations brief’ | ‘prep me for opening’.

- Workspace panel: Steps 3/3 complete with both output files.

> **Action:** Write down the three trigger phrases — you will use these
> in Exercise 5.

## Optional — View the SKILL.md file Cowork created

16. Click the store-daily-snapshot-SKILL.md link in the Workspace Output
    section to view the raw skill file.

![](./media/image39.png)

***What you should see:***

- store-daily-snapshot-SKILL.md open in a side panel.

- Content shows: name, description, trigger phrases, Do NOT use
  guardrails, and M365 data sources.

> **Action:** Read the SKILL.md to see the trigger phrases, guardrails,
> and data sources Cowork created. Close this panel when done.

## Step 6 — Confirm both skills in Customize \> Skills

17. Click Customize in the left nav and then click the Skills tab.

![](./media/image40.png)

***What you should see:***

- Customize \> Skills page now shows TWO skills under ‘Your skills’: (1)
  leadership-update (2) store-daily-snapshot.

- Built-in section unchanged. Both use the same circular arrow icon.

> **Action:** Both skills are confirmed. Both exercises completed
> successfully.

18. Click the Add button to see the dropdown, then click elsewhere to
    close it.

![](./media/image41.png)

***What you should see:***

- Customize \> Skills page with Add dropdown open. ‘Upload skill’
  highlighted.

- NOTE: ‘Upload skill’ installs a pre-written SKILL.md file — used in
  Exercise 6.

> **Action:** Click elsewhere to close the Add dropdown. Proceed to
> Exercise 5.

# Exercise 5: Run the Store Snapshot and Post to a Teams Channel

Skills become most powerful when their output goes somewhere useful
automatically. In this exercise you run the Store Daily Snapshot and
then direct Cowork to post the result to a Teams channel — all from one
natural-language instruction.

## Step 1 — Upload the SKILL.md file via the Upload skill path (optional reference step)

1.  Go to Customize \> Skills, click Add, then click Upload skill. The
    file browser will open.

![](./media/image42.png)

***What you should see:***

- Windows file browser Open dialog has appeared.

- Downloads folder: store-daily-snapshot-SKILL (selected),
  leadership-update-SKILL, cowork-output.

- Open button at the bottom right.

> **Action:** This step is optional — it shows how to upload a
> pre-written SKILL.md file. If not needed, click Cancel and proceed to
> Step 2.

## Step 2 — Invoke the Store Daily Snapshot skill from the task bar

2.  Click New task in the left nav to go to the home screen. Then click
    the task bar and type the trigger phrase.

![](./media/image43.png)

***What you should see:***

- Cowork home screen shows ‘What’s first today?’

- Task bar shows ‘give me the store daily snapshot’ typed in, with the
  blue send arrow active.

> **Action:** Press Enter or click the blue send arrow to submit the
> trigger phrase.

3.  Watch the left panel — a new Store Daily Snapshot Report task will
    appear.

![](./media/image44.png)

***What you should see:***

- Left panel: ‘Store Daily Snapshot Report’ highlighted in bold at the
  top of the task history.

- Main chat: right-aligned bubble ‘give me the store daily snapshot’.
  ‘Plugging away at this’ spinner visible.

> **Action:** Wait. Cowork is recognising the trigger phrase and loading
> the store-daily-snapshot skill.

4.  Watch the Workspace panel on the right — it confirms the
    store-daily-snapshot skill was activated.

![](./media/image45.png)

***What you should see:***

- Workspace panel confirms the skill activated: Skills & Plugins shows
  ‘store-daily-snapshot’.

- Chat: ‘I’ll pull together your store morning brief. Let me gather
  everything in parallel.’

- Three parallel searches running: Files, Email, Teams (store data) +
  Teams list chats.

> **Action:** Continue waiting. Cowork is searching across Files, Email,
> and Teams simultaneously.

## Step 3 — Read the Store Daily Snapshot output carefully

5.  The Store Daily Snapshot output has appeared. Read every section
    carefully.

![](./media/image46.png)

***What you should see:***

- Full Store Daily Snapshot output is displayed:

- RED DOT ‘Needs attention before open’ — Nothing flagged.

- YELLOW DOT ‘Today’s schedule & watch items’ — Deliveries,
  Shifts/staffing, Meetings: all None/clear.

- GREEN DOT ‘Overnight FYI’ — No overnight email. Zava Retail sales item
  surfaced from Teams and flagged proactively.

- Workspace panel: ‘store-daily-snapshot’ in Skills & Plugins.

> **Action:** Read the three coloured sections. The Zava Retail mention
> shows the skill surfaced relevant context proactively. Proceed to post
> to Teams.

6.  Scroll down in the main conversation to read the rest of the output,
    including Latest numbers.

![](./media/image47.png)

***What you should see:***

- Output continues: LATEST NUMBERS — ‘No sales or inventory report found
  in your files.’

- BOTTOM LINE — explains account may not be connected to a store
  mailbox, offers to search a specific location.

> **Action:** Cowork reports no store data rather than inventing numbers
> — this is graceful failure. Proceed to post the output to Teams.

## Step 4 — Post the snapshot to the Retail Teams channel

7.  Click the task bar at the bottom and type the Teams posting
    instruction, then press Enter.

![](./media/image48.png)

***What you should see:***

- Full snapshot output visible. Task bar shows: ‘send the updates to
  Retail temas channel’ typed in (typo ‘temas’ — Cowork understands it).

- Blue send arrow is active.

> **Action:** Press Enter or click the blue send arrow to submit the
> Teams posting instruction.

8.  Watch the conversation as Cowork locates the Retail Teams channel.

![](./media/image49.png)

***What you should see:***

- New bubble: ‘send the updates to Retail temas channel’.

- Cowork: ‘I’ll find the Retail channel and post the snapshot there.’

- ‘List teams’ action with Teams badge is visible.

> **Action:** Wait. Cowork is querying your Teams environment. A ‘Post
> to channel?’ dialog will appear shortly.

9.  A Post to channel? confirmation dialog has appeared. Review the
    details, then click Send.

![](./media/image50.png)

***What you should see:***

- ‘Post to channel?’ dialog appears.

- Channel: Retail \> \#General. Subject: ‘Store Daily Snapshot — Sunday,
  June 21, 2026’.

- Message preview shows the formatted snapshot with all three coloured
  sections.

- Cancel and Send buttons at the bottom right.

> **Action:** Confirm the channel shows ‘Retail \> \#General’ and
> subject is correct. Then click Send.

10. After clicking Send, watch Cowork confirm the post and open Teams in
    a new browser tab.

![](./media/image51.png)

***What you should see:***

- Browser address bar: m365.cloud.microsoft — still on Cowork.

- Chat: ‘Found the Retail team. I’ll post the snapshot to its channel.’

- ‘Approved 1 action’ banner confirms Cowork received permission to
  post.

> **Action:** Wait. The final posting confirmation will appear shortly.

11. Read the final confirmation message from Cowork.

![](./media/image52.png)

***What you should see:***

- Full confirmation flow in chat: team found, two ‘Approved 1 action’
  entries, then final message.

- Final: ‘Done — I posted the snapshot to the General channel of the
  Retail team.’

> **Action:** Cowork confirmed the post. Open Microsoft Teams to verify
> the message in Retail \> General.

## Step 5 — Verify the post appeared in Microsoft Teams

12. Switch to the Microsoft Teams browser tab (it opened automatically)
    or type teams.cloud.microsoft in a new tab.

![](./media/image53.png)

***What you should see:***

- A Microsoft Teams browser tab has opened
  (https://teams.cloud.microsoft).

- Teams tab shows a (1) notification badge. Teams loading splash screen
  is visible.

> **Action:** Wait for Teams to finish loading. Retail \> General will
> appear in the left navigation.

13. Teams has loaded. Navigate to Retail \> General in the left panel to
    find the posted message.

![](./media/image54.png)

***What you should see:***

- Microsoft Teams is fully loaded. LEFT PANEL: General, Healthcare,
  Retail (red icon — collapsed), Zava retail.

- Workflows shown in bold with a blue dot (new unread message).

> **Action:** Click ‘Retail’ in the Teams and channels section to expand
> it, then click ‘General’ under Retail.

14. Click Retail \> General in the left panel. The Store Daily Snapshot
    post will be visible.

![](./media/image55.png)

***What you should see:***

- Retail \> General channel is now open.

- Posted message from ODL_User 2270231 at 8:35 AM: ‘Store Daily Snapshot
  — Sunday, June 21, 2026’.

- Full snapshot body: RED DOT (nothing flagged), YELLOW DOT (three
  bullets all None/clear), GREEN DOT (two overnight bullets).

> **Action:** Confirm the Store Daily Snapshot message is visible in
> Retail \> General. End-to-end flow verified.

# Exercise 6: Inspect, Edit, Download, and Delete Skills

The final exercise shows you how to review a skill’s full instructions,
manage it, and understand the Download and Delete management options.

## Step 1 — Return to Cowork and navigate to the skill detail

1.  Switch back to the Cowork browser tab. Note the post confirmation in
    the conversation, then click Customize in the left nav.

![](./media/image56.png)

***What you should see:***

- Back in the Cowork browser tab. Final posting confirmation visible.

- Left panel: ‘Store Daily Snapshot Report’ at top of task history.

- Workspace panel: Skills & Plugins \> store-daily-snapshot.

> **Action:** Click Customize in the left navigation, then click the
> Skills tab.

## Step 2 — Open the store-daily-snapshot skill detail page

2.  Click the store-daily-snapshot tile in the Your skills section to
    open its detail page.

![](./media/image57.png)

***What you should see:***

- Skill detail page for ‘store-daily-snapshot’ is open.

- TOP RIGHT: Download button (downward arrow) and red Delete button (bin
  icon).

- Instructions box: Overview, When to Use (3 bullets), When NOT to Use
  (3 bullets — routes to daily-briefing, leadership-update,
  stakeholder-comms).

> **Action:** Read all three When NOT to Use entries — they route
> requests to more appropriate skills.

3.  Look at the top-right corner of the skill detail page to see the
    Download and Delete buttons.

![](./media/image58.png)

***What you should see:***

- Skill detail page: Download and red Delete buttons clearly visible at
  top right.

- Cursor is on the Delete button. Edit instructions pencil icon is
  visible.

> **Action:** DO NOT click Delete unless you want to permanently remove
> the skill. Download saves the SKILL.md for sharing. To edit
> instructions, click the pencil icon.

# Validation Checkpoint

Verify that you have successfully completed all exercises in this lab before proceeding.

- [ ] You built the **leadership-update** skill using the conversational Skill Builder and observed all three **Workspace** steps (**0/3**, **1/3**, and **3/3**) complete successfully with checkmarks.
- [ ] You reviewed the **leadership-update** skill guardrails, including all four **When NOT to Use** scenarios, and understand when requests should be routed to a different skill.
- [ ] You tested the **leadership-update** skill with sample input and confirmed the output included the following four sections:
  - **Headline**
  - **Progress**
  - **Risks & Blockers**
  - **Asks / Next Steps**
- [ ] You built the **store-daily-snapshot** skill using the same conversational workflow and confirmed the quality assessment reported **83/100 – Good, Meets the bar to publish**.
- [ ] You completed both the **Next step** dialog (**Leave it as-is**) and the **Auto-run** dialog after creating the **store-daily-snapshot** skill.
- [ ] You invoked the **store-daily-snapshot** skill and verified that Copilot Cowork searched across **Files**, **Email**, and **Teams**, then accurately reported that no store data was available instead of generating fabricated results.
- [ ] You instructed Copilot Cowork to post the generated snapshot to the **Retail > General** Microsoft Teams channel and verified that the message appeared in Teams at **8:35 AM**.
- [ ] You opened the **store-daily-snapshot** skill details page and located the **Download** and **Delete** actions in the upper-right corner.

> [!SUCCESS]
> **Congratulations!** You have successfully completed **Lab 6 – Building Custom Cowork Skills**. You learned how to create AI skills through the conversational Skill Builder, validate skill quality, test skill execution, apply guardrails, and publish AI-generated output to Microsoft Teams.
