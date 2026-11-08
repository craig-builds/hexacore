# HexaCore — postgraduate student record-keeping system

A web system that helps universities track postgraduate students from enrolment to completion. **Third-year group project at Nelson Mandela University, built by a team of four.**

## The problem
Postgraduate supervision involves many people and many stages: students, supervisors and evaluators, each needing a different view of the same information. Records scattered across emails and spreadsheets make it hard for a student to know their next step, and for a supervisor to see which of their students are on track or stuck.

## What it does
- **One record per student**, kept in a central database, covering their progress through each stage.
- **Role-based experience for every level of user**, from first-time students (novices) to experienced supervisors and evaluators (professionals). Each sees only the shortcuts and information relevant to their role.
- **Progress indicators** that show students exactly where they are and what comes next.
- **A tracking view for supervisors and evaluators** to follow several students at different stages at once.
- **Simplified tasks:** common actions are reduced to a few clicks, so the system supports the work rather than adding to it.

## How it works, role by role
Screenshots from the running system, using fictional demo data. Each section starts from the user's signed-in home screen.

### Student (novice) — one clear next step
The dashboard leads with a single "next task" and a progress bar, then shows deadlines, status and supervisor details at a glance.

![Student dashboard](screenshots/1-student/01-student.png)

| My supervisor | Ethics clearance | Proposal | Thesis |
|---|---|---|---|
| ![](screenshots/1-student/02-student-supervisor.png) | ![](screenshots/1-student/03-student-ethics.png) | ![](screenshots/1-student/04-proposal.png) | ![](screenshots/1-student/05-thesis.png) |

Steps unlock in order, so a student cannot submit a proposal before ethics clearance is verified. The same dashboard for a different student, at a different stage:

![Second student dashboard](screenshots/1-student-b/01-student.png)

### Supervisor — track every candidate
Counts of candidates, overdue proposals and at-risk students sit above a table showing each student's status and the action needed. Progress reports are written in a few fields and exported as a PDF.

![Supervisor: My students](screenshots/2-supervisor/01-supervisor.png)

| Progress reports | New progress report |
|---|---|
| ![](screenshots/2-supervisor/02-progress.png) | ![](screenshots/2-supervisor/03-progress-create-studentid-4.png) |

### Evaluator — a focused queue
Evaluators see only the proposals assigned to them, with counts of what is outstanding, completed and stalled.

![Evaluator dashboard](screenshots/3-evaluator/01-evaluator.png)

### Administrator (professional) — whole-institution oversight
A full view of every candidate, supervisor, evaluator and examiner, with whatever each is holding up. Rows waiting on someone are highlighted.

![Admin oversight](screenshots/4-admin/01-admin.png)

| Supervision register | Assign a supervisor | Committee decision queue | Progress reports |
|---|---|---|---|
| ![](screenshots/4-admin/02-supervision.png) | ![](screenshots/4-admin/03-supervision-assign-studentid-1.png) | ![](screenshots/4-admin/05-spgsc.png) | ![](screenshots/4-admin/06-progress.png) |

## My contribution
I contributed to the application's development and designed the workflow concepts around role-specific shortcuts and progress indicators, which help students identify their next steps and let supervisors and evaluators track multiple students at once.

## Stack
ASP.NET MVC (C#), Microsoft SQL Server, Visual Studio 2026.

## Team
A group of four third-year Software Development students at Nelson Mandela University.

## About this repository
This is a **showcase repository**. It contains a description only, not the source code. The code is a shared academic project with my teammates and remains private. © the HexaCore project team. All rights reserved. See [LICENSE](LICENSE).

Showcased by [Craig Chadley Johnson](https://github.com/craig-builds) — johnsoncraig.dev@gmail.com
