# GroupPilot v2 — University Group Project Planner

[**Try the live interactive demo**](https://yuzonglinsam.github.io/grouppilot/index.html)

A reusable workspace for university group coursework: presentations, research reports, case studies and software prototypes.

## Problem

Teams often coordinate through group chats and fragmented documents; ownership, milestones, blockers and delivery risks are hard to track. GroupPilot provides a shared project structure with a visual execution workflow.

## Demo workflow (90 seconds)

1. Open a sample workspace and review completion, upcoming milestones and owner workload.
2. Drag a task between Kanban columns.
3. Add a prerequisite to another task. GroupPilot surfaces the block and prevents premature completion.
4. Complete the prerequisite; finish the dependent task.
5. Review the local activity log and export a printable status report.
6. Create a new project with a template, members and deadline.

## Features

- Multiple projects and four course templates; automatic starter tasks and milestones.
- Kanban task CRUD, drag-and-drop, priority/owner filters.
- Member responsibilities, workload distribution and completion rates.
- Date-based project risks: overdue, due soon, unassigned and blocked.
- Prerequisite tasks and circular-dependency validation.
- Local activity log for project/task/milestone changes.
- JSON export/import and HTML report export; browser-local persistence.
- Responsive mobile and desktop UI.

## Stack

A dependency-free, self-contained web app built in vanilla **HTML, CSS and JavaScript**, deployable as GitHub Pages static content. The complete code lives in [index.html](./index.html).

Data model: `projects[]`, `tasks[]`, `activity[]`, active workspace and UI view, serialized in browser `localStorage`.

**Project boundary:** This is a single-user local-data prototype. The activity history is device-local, not an authenticated contribution log. Each sample project and member is synthetic. No backend, AI API, multi-device sync, account system or live collaboration has shipped yet.

## Next releases

1. Validate the workflow with real HKU course teams and document feedback.
2. Add accounts, invites, Postgres persistence and authorization.
3. Introduce authenticated team edits, realtime updates and audit history.
4. Optional evidence/rubric-aware planning assistant with verified due dates.

Author: Sam Yu · November 2026.
