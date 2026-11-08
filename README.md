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

## The full journey: one doctoral candidate, five users
Follow Thabo Nkosi from ethics clearance to examination. Every step is a real screen from the running system, and each hand-off appears as the *next task* for the right person.

**1. Administrator verifies ethics clearance.** A proposal can't be submitted until ethics is verified.

![Admin verifies ethics](screenshots/5-process/01-admin-verifies-ethics-before.png)

**2. Student: the proposal step unlocks and a proposal is submitted with a PDF.**

| Dashboard after ethics | Proposal form | Submitted |
|---|---|---|
| ![](screenshots/5-process/03-student-ethics-cleared-dashboard.png) | ![](screenshots/5-process/04-student-proposal-form.png) | ![](screenshots/5-process/05-student-proposal-submitted.png) |

**3. Supervisor is prompted to assign evaluators.** The system lists only eligible staff and excludes the student's own supervisors automatically.

| Proposal arrives | Panel assigned |
|---|---|
| ![](screenshots/5-process/06-supervisor-sees-proposal.png) | ![](screenshots/5-process/09-supervisor-panel-assigned.png) |

**4. Evaluator records Accept, Rework or Reject, with comments.**

| Assignment appears | Evaluation | Queue cleared |
|---|---|---|
| ![](screenshots/5-process/10-evaluator-sees-assignment.png) | ![](screenshots/5-process/11-evaluator-reviews-a-dlamini.png) | ![](screenshots/5-process/12-evaluator-after-a-dlamini.png) |

**5. Administrator approves the evaluated proposal** in the committee queue.

| Awaiting approval | Approved |
|---|---|
| ![](screenshots/5-process/13-admin-proposal-awaiting-approval.png) | ![](screenshots/5-process/14-admin-proposal-approved.png) |

**6. Student: the thesis step unlocks, and the thesis is lodged for examination.**

| Proposal approved | Thesis unlocked | Thesis form | Lodged |
|---|---|---|---|
| ![](screenshots/5-process/15-student-proposal-approved-dashboard.png) | ![](screenshots/5-process/16-student-thesis-unlocked.png) | ![](screenshots/5-process/17-student-thesis-form.png) | ![](screenshots/5-process/18-student-thesis-lodged.png) |

**7. Supervisor nominates a three-examiner panel** (doctoral candidates need three, at least one external). The nomination is hidden from the candidate.

| Thesis lodged | Nominating | Full panel |
|---|---|---|
| ![](screenshots/5-process/19-supervisor-thesis-lodged.png) | ![](screenshots/5-process/21-supervisor-nominating-examiner.png) | ![](screenshots/5-process/22-supervisor-examiners-nominated.png) |

**8. Supervisor writes a progress report and downloads it as a PDF.**

| Report form | Report created |
|---|---|
| ![](screenshots/5-process/23-supervisor-progress-report-filled.png) | ![](screenshots/5-process/24-supervisor-progress-report-created.png) |

**9. Administrator sees the updated picture across all candidates.**

![Admin oversight after the journey](screenshots/5-process/25-admin-oversight-after-journey.png)

## My contribution
I contributed to the application's development and designed the workflow concepts around role-specific shortcuts and progress indicators, which help students identify their next steps and let supervisors and evaluators track multiple students at once.

## Stack
ASP.NET MVC (C#), Microsoft SQL Server, Visual Studio 2026.

## Team
A group of four third-year Software Development students at Nelson Mandela University.

## About this repository
This is a **showcase repository**. It contains a description only, not the source code. The code is a shared academic project with my teammates and remains private. © the HexaCore project team. All rights reserved. See [LICENSE](LICENSE).

Showcased by [Craig Chadley Johnson](https://github.com/craig-builds) — johnsoncraig.dev@gmail.com
