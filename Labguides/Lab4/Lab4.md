# Lab 4 – Executive Meeting Coordinator

| Estimated Time | 20 minutes |
|----|----|
| Objective | Automate the full meeting lifecycle: AI-generated preparation, cross-app content collection, and post-meeting follow-up — all grounded in real M365 data. |
| Skills & Plugins Active | Word (docx skill), Calendar Management, Scheduling, OneDrive/SharePoint connector, Microsoft Graph API, Teams connector, Transcript connector |

## Exercise 1: AI-Generated Meeting Preparation

Goal: Build a cross-app meeting prep brief as a Word document saved to
OneDrive Lab Files. Data gathered from Calendar, Email,
OneDrive/SharePoint, and Teams in parallel.

1.  Go to the Cowork tab (not Chat).

<img src="./18e84db2ace698b5322d1e215a10753eb497bf2a.png"
style="width:7in;height:4.63542in" />

2.  In the prompt bar, type the Exercise 1 prompt and press Enter:

"Prepare me for my next meeting. Build a one-page prep brief containing:
attendee list with my last interaction with each, the stated purpose,
related email threads and files, open action items from previous related
meetings, and 3 questions I should ask. Save it as a Word document in my
'Lab Files' folder named 'Prep –june 19, 2026 –project planning
workshop'."​

**Screenshot 1 — Prompt submitted — Cowork begins processing**

<img src="./media/image1.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork received the prompt and auto-named the session
“Meeting Preparation Brief for…” in the left sidebar. The status
“Narrowing down the approach” confirms it is processing before opening
the Workspace panel.

**Screenshot 2 — Workspace opens — Step 1 of 2 complete, calendar
accessed**

<img src="./media/image2.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork read Outlook Calendar and found “Project Planning
Workshop today at 8:00 AM–12:00 PM UTC.” Step 1 is complete (✓); the
plan is still expanding as Cowork decides what additional data to
gather.

**Screenshot 3 — Workspace expands to 5 steps — parallel lookups begin**

<img src="./media/image3.png" style="width:5.9375in;height:3.4375in" />

**What We Did** The Workspace plan expanded from 2 to 5 steps. Steps 2–4
(attendee profile, emails/files, transcripts) run in parallel; Step 5
(document build) waits for all data to complete.

**Screenshot 4 — Data gathering complete — transitioning to document
build**

<img src="./media/image4.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Data gathering is complete. Cowork transitions to deeper
email extraction and notes that the “Lab Files” folder doesn’t exist —
it will create it rather than fail.

3.  A “Create folder?” card has appeared. Click the dark “Create” button
    to approve. ⚠ Do NOT type in the message bar while the card is open
    — it will cancel the action.

**Screenshot 5 — Approval card — “Create folder?” for Lab Files in
OneDrive**

<img src="./media/image5.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork requests approval before writing to OneDrive. The
card confirms the exact folder name from your prompt. This
approve-before-write pattern ensures Cowork never modifies storage
silently.

4.  Click “Create” to proceed.

**Screenshot 6 — Cursor on “Create” button — about to approve**

<img src="./media/image6.png" style="width:5.9375in;height:3.4375in" />

**What We Did** The cursor is on the “Create” button. One click approves
folder creation — Cowork has been waiting patiently.

**Screenshot 7 — Folder created — Word plugin activates**

<img src="./media/image7.png" style="width:5.9375in;height:3.4375in" />

**What We Did** “Approved 1 action” confirms the Lab Files folder was
created. The Word plugin activates immediately in the Skills & Plugins
panel — required to generate the .docx file.

**Screenshot 8 — Word document build starts — agent narrates its plan**

<img src="./media/image8.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Document build starts. Cowork uses a two-phase approach:
writes a content plan, then executes it to produce the .docx. The Output
panel begins showing the document filename.

**Screenshot 9 — Folder confirmed — Word build in progress**

<img src="./media/image9.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Folder creation confirmed (blue circle). Cowork
transitions cleanly from infrastructure (folder) to content (document
build) — the Word plugin is active.

**Screenshot 10 — Four parallel sub-tasks enumerated — Output panel
shows document**

<img src="./media/image10.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork lists four parallel lookups (attendee,
emails/files, transcripts, Teams chats) and confirms it is the meeting
organiser. The Output panel shows the prep brief filename being built.

**Screenshot 11 — First parallel batch complete — deeper email search
begins**

<img src="./media/image11.png" style="width:5.9375in;height:3.4375in" />

**What We Did** First parallel batch complete. Three M365 connectors ran
simultaneously: Directory (attendee profile), Email + Files (related
docs), Outlook (calendar). Cowork now reads full email bodies.

**Screenshot 12 — Deepest data layer — email bodies, Teams chats, and
transcripts**

<img src="./media/image12.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Deepest data extraction: four simultaneous calls — full
email body, all messages, Teams chat history, and meeting transcripts.
Empty transcript results are expected in a sandbox.

**Screenshot 13 — Build error detected and self-corrected — spacing
optimised**

<img src="./media/image13.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork self-corrected a syntax error at line 371, then
detected a 2-page spill and began iterative spacing reduction to meet
the one-page requirement.

**Screenshot 14 — Second round of spacing reduction — document close to
one page**

<img src="./media/image14.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Still 2 pages after the first pass. Cowork identifies
the exact overflow elements (alert box and questions table) and targets
only those for margin reduction.

**Screenshot 15 — Final fixes — smart quotes, trailing spacer, upload
preparation**

<img src="./media/image15.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Three final quality fixes: questions shortened, smart
quotes converted to ASCII, trailing blank spacer removed. File is then
located and encoded for upload.

5.  A “Use Microsoft Graph?” card has appeared. Click “Approve” to
    upload the document to OneDrive. ⚠ Do NOT type in the message bar
    while the card is open.

**Screenshot 16 — Upload approval card — “Use Microsoft Graph?” to save
to Lab Files**

<img src="./media/image16.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Every file write to OneDrive requires this approval
step. The card confirms the filename and destination folder. “Always
allow” is available to pre-approve future Graph calls this session.

**Screenshot 17 — Upload failed — document accessible via link card**

<img src="./media/image17.png" style="width:5.9375in;height:3.4375in" />

**What We Did** The upload failed due to sandbox permissions. The
document is still accessible via the link card in the chat — Cowork
reports the failure transparently rather than pretending it succeeded.

6.  Click the document link card to open the prep brief in Word Online
    and verify all sections.

**Screenshot 18 — Word Online — completed prep brief document open**

<img src="./media/image18.png" style="width:5.9375in;height:3.4375in" />

**What We Did** The completed prep brief opens in Word Online with a
professional dark blue header. All five sections are populated with real
M365 data: Meeting Details, Attendees, Emails, Files, and 3 Questions.

**Screenshot 19 — Side-by-side — Cowork shows 3 questions and ⚠ heads-up
alert**

<img src="./media/image19.png" style="width:5.9375in;height:3.4375in" />

**What We Did** The three strategic questions are grounded in the
meeting’s stated purpose. The ⚠ Heads-up alert proactively flags the
invite bounce to Amit M — a risk Cowork surfaced from email data without
being asked.

**Screenshot 20 — Word document — lower sections including Heads-up and
Q table**

<img src="./media/image20.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Lower sections confirmed: Attendees table shows Amit M’s
last interaction, Related Emails shows the invitation and bounce notice,
Related Files honestly reports “No related files found”, and the
Q1/Q2/Q3 table is present.

7.  Send the refinement prompt: “Add a Risks section listing anything in
    the email threads that sounds like a blocker.”

**Screenshot 21 — Refinement prompt — “Add a Risks section” typed and
ready to send**

<img src="./media/image21.png" style="width:5.9375in;height:3.4375in" />

**What We Did** The refinement tests whether Cowork updates the existing
document or creates a duplicate. No Risks section exists yet — the right
panel shows the current document state.

**Screenshot 22 — Refinement submitted — Cowork re-analyses email
threads**

<img src="./media/image22.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Refinement sent. Cowork re-analyses email threads
already gathered — no new API calls needed. The document stays unchanged
while the update is being prepared.

**Screenshot 23 — Word Online — view document in context before Risks
section added**

<img src="./media/image23.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Document before the update: ends with 3 QUESTIONS TO
ASK, Page 1 of 1. Useful as a before/after comparison point.

**Screenshot 24 — Risks section added — grounded content confirmed**

<img src="./media/image24.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Risks/Blockers section added with one grounded finding:
the invite bounce. Cowork confirms exactly one blocker found and that
the document still fits on one page. Updated in place — not duplicated.
✓

8.  Send: “move updated word file to lab files folder”

**Screenshot 25 — “move updated word file to lab files folder” — typed
and sent**

<img src="./media/image25.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork must interpret “updated word file” as a specific
OneDrive file ID, verify it contains the Risks section, then present an
approval card for the move.

**Screenshot 26 — “move updated word file” sent — Cowork searching
OneDrive**

<img src="./media/image26.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork gets the OneDrive root path and searches by
filename to locate the correct version. “Thinking…” indicates it is
selecting the updated file over the original.

9.  A “Use Microsoft Graph?” card for the file move has appeared. Click
    “Approve”.

**Screenshot 27 — File verified — “Use Microsoft Graph?” card for move
operation**

<img src="./media/image27.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork confirmed the file contains the Risks section
before requesting the move. The card describes the action clearly:
“Moving the prep brief into the Lab Files folder.”

**Screenshot 28 — Move blocked twice — Cowork pivots to copy operation**

<img src="./media/image28.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Move API blocked twice by sandbox restrictions. Cowork
transparently reports both failures and autonomously pivots to a copy
operation as a fallback — no user input needed.

**Screenshot 29 — Copy succeeds — file verified in Lab Files folder**

<img src="./media/image29.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Copy succeeded (“Approved 1 action”). Cowork
automatically verifies the file appears in Lab Files by listing folder
contents before confirming success.

**Screenshot 30 — Final confirmation — housekeeping note about two
copies**

<img src="./media/image30.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Updated prep brief confirmed in Lab Files. Cowork
discloses that a second copy remains in the working folder and honestly
acknowledges it cannot delete it from here.

**Screenshot 31 — Document thumbnail hover card — v2 file confirmed in
Output panel**

<img src="./media/image31.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Thumbnail preview confirms professional formatting. The
Workspace Output panel shows two files: v2 (with Risks) and the
original. Use the v2 link to open the final document.

10. Open OneDrive → My files. Verify the Lab Files folder exists with 1
    item.

**Screenshot 32 — OneDrive web view — Lab Files folder visible with 1
item**

<img src="./media/image32.png" style="width:5.9375in;height:3.4375in" />

**What We Did** OneDrive confirms the Lab Files folder was created and
contains 1 item — external verification that the Cowork workflow
produced a real, accessible OneDrive folder.

**Screenshot 33 — Two-file status table — v2 is correct, original is
outdated**

<img src="./media/image33.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork provides a clear ✅/❌ status table: v2 (updated
with Risks) is the correct file; the original is outdated. Click the v2
link. Exercise 1 complete.

**Screenshot 34 — Word Online — RISKS / BLOCKERS section visible in
final document**

<img src="./media/image34.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Final v2 document: RISKS / BLOCKERS section appears in
orange/red with Blocker, Source (actual email subject), and Recommended
Action. Page 1 of 1 — one-page constraint maintained. ✓

## Exercise 2: Collect Documents, Emails, and Action Items

Goal: Gather all content related to the Project Sync meeting and
organise it into a “Meeting Pack” folder in OneDrive with a hyperlinked
index document.

11. Send the Exercise 2 prompt: "For the Project Sync meeting, gather
    everything related: files in OneDrive/SharePoint, email threads,
    Teams messages, and any open tasks. Organise them into a single
    'Meeting Pack' folder in OneDrive and give me an index document
    linking to each item with a one-line description."

**Screenshot 35 — Exercise 2 prompt — typed and ready to send**

<img src="./media/image35.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Exercise 2 gathers content from four M365 sources and
produces a hyperlinked index document. The two Exercise 1 output files
carry over in the Workspace panel.

**Screenshot 36 — New workspace with 4 steps — parallel search
launched**

<img src="./media/image36.png" style="width:5.9375in;height:3.4375in" />

**What We Did** New 4-step Workspace plan opens. Cowork launches
parallel searches: Outlook for the Project Sync event, and Files +
Email + Teams for related content. Graph API permissions from Exercise 1
carry over.

**Screenshot 37 — Project Sync identified — false positives detected,
deeper search initiated**

<img src="./media/image37.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Project Sync identified (June 23, 9:00–9:45 AM UTC).
Initial search returned mostly loose keyword matches. Cowork proactively
flags the quality issue and deepens the search rather than filling the
pack with irrelevant results.

12. A “Pack scope” card has appeared. Select option 1 “Project planning
    work”, then click Submit.

**Screenshot 38 — Scope disambiguation card — three options for Meeting
Pack content**

<img src="./media/image38.png" style="width:5.9375in;height:3.4375in" />

**What We Did** “Project Sync” is too generic — Cowork found two content
clusters and presents options rather than guessing. It also honestly
reports that open tasks couldn’t be retrieved due to a permission gap.

13. Confirm option 1 is selected (filled badge), then click Submit.

**Screenshot 39 — Option 1 selected — “Project planning work” scoped**

<img src="./media/image39.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Option 1 selected: prep doc with Risks, invitation +
bounce emails, and Teams chat with Amit M. Active sales deal threads are
correctly excluded as unrelated.

14. A “Create folder?” card has appeared. Click “Create” to approve the
    Meeting Pack folder.

**Screenshot 40 — “Create folder?” card — Meeting Pack – Project Sync**

<img src="./media/image40.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Same folder-creation pattern as Exercise 1. Workspace
shows 2/4 steps — search phase complete, build phase beginning. Both
Graph API permissions from Exercise 1 remain active.

**Screenshot 41 — Meeting Pack folder created — prep brief being copied
in**

<img src="./media/image41.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Meeting Pack – Project Sync folder created. Cowork
correctly selects the v2 prep brief (with Risks) to copy in,
demonstrating cross-exercise memory.

**Screenshot 42 — Step 3 complete — index document creation starts**

<img src="./media/image42.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Step 3 complete. Step 4 (index document) starts. Cowork
waits for OneDrive sync confirmation before generating hyperlinks to
ensure all links point to verified locations.

**Screenshot 43 — All 4 steps complete — 5-item index confirmed with
caveats**

<img src="./media/image43.png" style="width:5.9375in;height:3.4375in" />

**What We Did** All 4/4 steps complete. Index links to 5 items with
honest caveats (task permission gap, scope limit). Cowork also flags two
action items: the bounced invite and missing Project Sync attendees.

15. Click the Meeting Pack index document link to open it in Word
    Online. Verify the first 3 rows and test the hyperlinks.

**Screenshot 44 — Word Online — Meeting Pack index document, first 3
items**

<img src="./media/image44.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Index document open in Word Online. Header shows
“MEETING PACK — INDEX” with meeting details. Items 1–3 (calendar event,
prep brief, invitation email) have hyperlinks and source type labels.

**Screenshot 45 — Word Online — complete index with all 5 items and
Notes & Coverage**

<img src="./media/image45.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Complete index: all 5 items with hyperlinks, source
labels, and one-line descriptions. NOTES & COVERAGE section documents
the task permission gap, scope limit, and action about the bounced
invite. Page 1 of 1. ✓ Exercise 2 complete.

## Exercise 3: Post-Meeting Follow-Up Automation

Goal: Generate a meeting summary, action items, follow-up email, and
tasks from a transcript. Demonstrates AI grounding — refusing to
fabricate content without source material.

16. Send the Exercise 3 prompt: "From this meeting's
    transcript/notes: (1) write a crisp summary with decisions made, (2)
    extract action items with owner and due date, (3) draft a follow-up
    email to all attendees, and (4) create tasks for the items assigned
    to me. Show me everything for review before creating or sending
    anything."

**Screenshot 46 — Exercise 3 prompt — typed and ready to send**

<img src="./media/image46.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Four post-meeting deliverables requested. The “Show me
everything for review” safeguard tests whether Cowork defers all actions
pending approval. Cowork will first search for a transcript.

**Screenshot 47 — Grounding enforced — “I won’t invent meeting
content”**

<img src="./media/image47.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Cowork immediately enforces grounding: “Before I write
anything, I need the actual transcript or notes — I won’t invent meeting
content.” It searches for transcripts, finds none, then widens the
search to notes files.

**Screenshot 48 — Complete refusal with three constructive forward
paths**

<img src="./media/image48.png" style="width:5.9375in;height:3.4375in" />

**What We Did** After an exhaustive search, Cowork confirms no source
material exists: “I can’t produce them without fabricating what was
said, which I won’t do.” Three constructive alternatives are offered:
paste notes into chat, run after the meeting with transcription on, or
point to a different meeting with an existing transcript.

**Screenshot 49 — Correction pre-registered — honest state disclosure**

<img src="./media/image49.png" style="width:5.9375in;height:3.4375in" />

**What We Did** Correction test result: Cowork acknowledges “website
task → Priya, not you” and honestly discloses no action items have been
generated yet — so there is nothing to correct. The correction is
pre-registered for when notes are provided. ✓ Exercise 3 complete. All
validation checkpoints confirmed.

# Validation Checkpoint

Before completing the lab, confirm every item below against your actual
Cowork session:

- ✔ Exercise 1 — A prep brief exists as a Word file in the OneDrive Lab
  Files folder, combining calendar, email, and file context. The
  Risks/Blockers section is present and grounded in a real email thread.

- ✔ Exercise 1 — The document was updated (not duplicated) when the
  Risks section was added. Only one new section was inserted.

- ✔ Exercise 2 — A Meeting Pack folder with a working index document
  exists in OneDrive. The index links to 5 items with source labels and
  one-line descriptions.

- ✔ Exercise 2 — The Notes & Coverage section of the index honestly
  documents what was omitted and why (task permissions gap, scope
  limitation).

- ✔ Exercise 3 — Cowork refused to fabricate meeting content and
  explicitly stated it would not invent meeting decisions. Three
  constructive alternatives were offered.

- ✔ Exercise 3 — The action item correction (“website task was assigned
  to Priya”) was acknowledged and pre-registered for future use —
  without creating phantom corrected outputs.
