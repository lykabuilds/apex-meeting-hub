# Apex Meeting Hub

**Live demo:** https://lykabuilds.github.io/apex-meeting-hub/

A prototype of a one-stop department hub. It turns meeting transcripts into tracked action items, and project requests into approved, measurable projects.

> All data is fictional. Apex Motorsport, its people, sponsors and suppliers were created as sample data for this demo.

## The problem

Teams lose track of what was decided in meetings and who owes what. Project requests arrive by email or chat, files sit in separate team folders, and progress lives in personal task lists. Results are rarely measured, so it's hard to show whether a project actually worked.

## What it does

### Meeting briefs
- AI-style summaries of each meeting: TL;DR, summary, decisions, open items and risks
- Full transcript, collapsible, under each brief
- Editable tags for meeting type, company, department and people
- Comments at the end of each brief
- Filters by type, company, department and person

### Deliverables
- Every action item from every meeting in one board
- Editable status (Not started, In progress, Blocked, Done) and owner
- Remarks on each deliverable
- Group by date and meeting, owner, or status, with collapsible groups
- Flags for overdue items, items due soon, missing dates and unassigned owners

### Team summary
- A roster of "our team", separate from other meeting participants
- One card per teammate with open, done, overdue and no-date counts
- Unassigned deliverables and other teams' workload shown separately

### Projects
- **Request form:** captures the problem, success criteria, and a baseline and target for measurement
- **Automatic Project ID** in a readable format (e.g. `202609-APR-FRT`) plus a random access code
- **Approval queue:** approve, ask for more information, or decline. Approval is blocked without a baseline or a written reason
- **Project register** with stage, owner, due date and KPI progress
- **Project page** with baseline vs target vs actual, linked meetings, files and an activity log
- **Closure rule:** a project can't close until its actual result is logged
- **Requester view:** enter the Project ID and access code to see status and finished files only

### Department KPIs
- % of projects with a baseline
- % of closed projects with a measured result
- % of closed projects that hit target
- Deliverables closed, overdue, and with both an owner and a due date

## Try it

1. Open a meeting brief and change a deliverable's status or owner.
2. Go to **Deliverables** and group by owner.
3. Go to **Projects → New request**, submit a request, then approve it in the **Approval queue**.
4. In **Requester view**, use the demo button to look up a project as a requester would.

Changes save in your own browser only, so every visitor starts from the same demo data. Use **Reset demo** in the footer to start over.

## How the real version works

This prototype shows the interface and workflow. In a production build:

| Prototype | Production |
|---|---|
| Meeting briefs | Meeting recordings (Wispr Flow, Fathom) summarized by AI |
| Request form | Microsoft Forms or Jotform |
| Project ID, access code, folder creation | Power Automate or Make |
| Project register | SharePoint list, Airtable or Google Sheets |
| KPI dashboard | Power BI |

## Built with

Plain HTML, CSS and JavaScript in a single file. No frameworks, no build step, no backend.

## Author

**Lyka Ganotisi**, digital transformation and process automation
Lean Six Sigma Yellow Belt · Power Automate · Make · SharePoint · Google Apps Script
