# Training Progress & Proof – Renuka Jadhav

Every finished task gets a proof: a commit, a link, or a screenshot saved in `proof/`.
Plan: [training-plan.md](training-plan.md) for Days 1–5 · "Renuka's Learning Path" (PDF from my manager, 19 Oct) for Days 6–20

## Summary

| Day | Status | Main proof |
|---|---|---|
| 1 | Done | [notes.md on GitHub](https://github.com/renukajadhav-spec/training/blob/main/Day%2001/notes.md) |
| 2 | Done | [commit history](https://github.com/renukajadhav-spec/training/commits/main) |
| 3 | Done | [Live profile page](https://renukajadhav-spec.github.io/training/) |
| 4 | Done | [vendors.csv](Day%2004/vendors.csv) · [Day 4 notes](Day%2001/notes.md) |
| 5 | Done | [vendor-page repo](https://github.com/renukajadhav-spec/vendor-page) · [overdue in red](proof/day5-overdue-red.png) |
| 6 | To do | |
| 7 | To do | |
| 8 | To do | |
| 9 | To do | |
| 10 | To do | |
| 11 | To do | |
| 12 | To do | |
| 13 | To do | |
| 14 | To do | |
| 15 | To do | |
| 16 | To do | |
| 17 | To do | |
| 18 | To do | |
| 19 | To do | |
| 20 | To do | |

## Day 1 – Set up laptop, meet VS Code (12 Oct 2026)

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Install VS Code and Git | Done | `git version 2.56.0.windows.2` shown in VS Code's Git Bash terminal |
| 2 | Claude Code extension + company login | Done | Extension installed and working; signed in as renukajadhav334@gmail.com — manager confirmed (14 Oct) this login is OK to use instead of a company login |
| 3 | Folder `training`, opened in VS Code | Done | `Desktop\Training` open as the VS Code workspace |
| 4 | `notes.md` with heading, list, bold | Done | [notes.md](https://github.com/renukajadhav-spec/training/blob/main/Day%2001/notes.md), commits `534780a`, `aa2414e` |
| 5 | `git --version` in the VS Code terminal | Done | Version shown after fixing `git--version` → `git --version` |
| 6 | Ask Claude "Explain what this folder contains" | Done | Claude listed and read `.vscode`, `Day 01`, `Day 02` and the PDF (14 Oct) |

## Day 2 – Git and GitHub (13–14 Oct 2026)

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | GitHub account (work email) | Done | Account [renukajadhav-spec](https://github.com/renukajadhav-spec) |
| 2 | "Introduction to GitHub" exercise | Not required | Manager confirmed on 14 Oct that this exercise is not needed |
| 3 | Repo `training`, connected to Day 1 folder | Done | [training](https://github.com/renukajadhav-spec/training), first commit `5fb1348` |
| 4 | Change `notes.md`, commit + push ×3 | Done | `aa2414e` Format notes · `dbe0ac1` Git commands section · `7800e3b` Day 2 template – [history](https://github.com/renukajadhav-spec/training/commits/main) |
| 5 | Branch `practice`, change, merge back | Done | Commit `57cd23a` on [practice](https://github.com/renukajadhav-spec/training/tree/practice), fast-forward merged into `main` |

**Extra work:** 5-page PDF presentation `Training Day 1 Presentation.pdf`; INDEX/MATCH practice file checked (2/20 correct, Task 3 fix explained).

**Open fixes for Day 2:**
- [x] Repo name: renamed `Training_` → `training` on 14 Oct; local folder re-pointed with `git remote set-url`.
- [x] Delete the accidental duplicate repo `Training.` (deleted 14 Oct; confirmed via GitHub API, now returns 404).
- [x] Commit email: switched to `renuka.jadhav@verveadvisory.com` on 14 Oct. Earlier commits keep the Gmail; add it on GitHub → Settings → Emails so they link to the profile too.
- [x] Commit "Added Day 2 notes" with the content of `Day 2.docx` (14 Oct).
- [x] Send Day 1 and Day 2 daily notes to the manager (sent 14 Oct).

## Day 3 – Profile page with Claude Code (14 Oct 2026)

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Write page wishes in `notes.md` | Done | Commit `d4b0c19` "Added Day 3 page plan" |
| 2 | Plan mode: plan first, read it, adjust | Done | Plan shown with page sketch, approved before building |
| 3 | Claude builds the page, check in browser | Done | Commit `ac69018` "Add Day 3 profile page" (`docs/index.html`) |
| 4 | Ask for at least 2 changes in plain words | Done | `9d6a1a7` swap colours (white header, blue cards) · `8d46950` add Reconciliation skill |
| 5 | Commit, push, put live with GitHub Pages | Done | Live: https://renukajadhav-spec.github.io/training/ (Pages: `main` / `docs`) · screenshot [proof/day3-profile-page.png](proof/day3-profile-page.png) |
| 6 | No phone number or personal email on the page | Done | File checked: 0 email addresses, 0 phone numbers |

**Open for Day 3:**
- [x] Send Day 3 daily note to the manager (sent 14 Oct).

## Day 4 – First database with Supabase (15 Oct 2026)

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Supabase account + project `training` | Done | Signed in with GitHub; project `training`, region South Asia (Mumbai), status Healthy – [proof/day4-supabase-project.png](proof/day4-supabase-project.png) |
| 2 | 15 fake vendors (name, city, GSTIN, credit limit, balance, due date) as CSV | Done | [Day 04/vendors.csv](Day%2004/vendors.csv) – commit `b9fc611` (5 over limit, 6 overdue as of 15 Oct) |
| 3 | Create `vendors` table in Supabase, import CSV | Done | Table `vendors`: 15 records, primary key `gstin`, `due_date` as date, RLS on – [proof/day4-vendors-table.png](proof/day4-vendors-table.png) |
| 4 | SQL queries: balance above credit limit, total balance by city | Done | [Day 04/queries.sql](Day%2004/queries.sql) · saved in Supabase as Q1–Q3 · results: [Q1 over limit – 5 vendors](proof/day4-query1-over-limit.png) · [Q2 balance by city – 8 cities](proof/day4-query2-balance-by-city.png) · [Q3 bonus overdue – 6 vendors (15 Oct)](proof/day4-query3-overdue.png) |
| 5 | Notes: Supabase table vs Excel sheet | Done | "Day 4: Supabase table vs Excel sheet" in [Day 01/notes.md](Day%2001/notes.md) – alike + 5 differences + notebook vs office register |

**Open for Day 4:**
- [x] Send Day 4 daily note to the manager (sent 15 Oct).

**Extra (15 Oct):** Profile page upgraded to v2: a professional two-column résumé built from my CV – commit `c487019`, live at https://renukajadhav-spec.github.io/training/, screenshot [proof/day3-profile-page-v2.png](proof/day3-profile-page-v2.png).

## Day 5 – Connect a page to the database (19 Oct 2026)

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | New folder and repo `vendor-page` | Done | Folder `Desktop\vendor-page` · repo [vendor-page](https://github.com/renukajadhav-spec/vendor-page) |
| 2 | Plan mode first: page shows vendors from Supabase in a table, overdue vendors in red | Done | Plan read and approved before building · 15 vendors, 7 overdue in red on 19 Oct – [proof/day5-overdue-red.png](proof/day5-overdue-red.png) |
| 3 | Small form to add a vendor; check it appears in Supabase | Done | Added "Shivam Enterprises"; table now 16 records – [proof/day5-new-vendor.png](proof/day5-new-vendor.png) |
| 4 | Ask "Which key did you use? Is it safe to push this?"; no secret key in any pushed file | Done | Only the publishable key used; search for `service_role` / `sb_secret` found nothing. Two RLS policies (read + add only) – [proof/day5-rls-policies.png](proof/day5-rls-policies.png) |
| 5 | Commit and push | Done | Commit `bf4f463` on `vendor-page` main |

## Extra – Portfolio website (21 Oct 2026)

Built a job-search portfolio from my resume, with Claude Code. Live: https://renukajadhav-spec.github.io/training/portfolio/ (file [docs/portfolio/index.html](docs/portfolio/index.html)).

| # | Step | Proof |
|---|---|---|
| 1 | Plan mode: chose company names + email + LinkedIn, **no phone**; new page beside the Day 3 page | Plan approved before building |
| 2 | Built the page with photo, menu, skills, experience, projects, education, contact | Commit `820c9f1` · PR #3 |
| 3 | Personality: teal + gold, motto "Accuracy first, speed next", How I work, Currently learning, hobbies | Commit `effb252` · PR #5 (PR #4 went into `add-portfolio` by mistake: base was not `main`) |
| 4 | Floating menu that follows you down the page | Commit `e3cb8a8` · PR #6 |
| 5 | Safety check before every push: no passwords, keys or phone number | Done for all 3 commits |

**Lessons:** a host (GitHub Pages) is needed to give an HTML file a public link · always check the PR **base is `main`** · Pages only publishes `main` · a browser cache can show an old version (use Ctrl + F5 or Incognito).

**Open:** screenshot of the live page → `proof/portfolio.png`.

---

# Learning Path – Days 6 to 20

How every topic works: Why → What → How → Where → Do (hands-on) → Explain back.
Learning happens in the claude.ai Project **My Training** (one chat per topic). At the end of each chat I type `summary` and paste it into my Learning Notebook.
Review: up to 30 minutes a day with my manager. I explain without notes. Clear = move on, not clear = repeat.

## Before Day 6 – Set up the Claude tutor

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Create Project **My Training** in claude.ai | To do | |
| 2 | Paste the project instructions (Learning Path page 3) | To do | |
| 3 | Start a Learning Notebook (Word or Google doc) | To do | |

## Day 6 – The big picture, VS Code, Git and GitHub

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: how software gets built | To do | |
| 2 | Draw idea → live app on paper; mark VS Code, Git, GitHub, Supabase, GitHub Pages, Claude Code; check with Claude | To do | |
| 3 | Session 2 chat: VS Code as a workbench | To do | |
| 4 | Write what each part of the VS Code screen does; let Claude correct me | To do | |
| 5 | Session 3 chat: Git and GitHub as an audit trail | To do | |
| 6 | Explain my Day 2 commits; make 1 new commit, explaining each step before running it | To do | |
| 7 | Summaries + 3 open questions in the notebook | To do | |

**Review (explain without notes):**
- [ ] Idea → live app, in my own words
- [ ] What VS Code is for, plus one alternative
- [ ] Git vs GitHub
- [ ] What a commit is and why history matters (accounting comparison)
- [ ] Why we never work directly on the main copy

## Day 7 – How a web app works: pages, databases, going live

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: what happens when you open a link | To do | |
| 2 | View page source of my profile page and discuss it; change one line, push, watch it update | To do | |
| 3 | Session 2 chat: databases vs Excel | To do | |
| 4 | Design a `vendor invoices` table on paper; 3 SQL questions (guess first, then run) | To do | |
| 5 | Session 3 chat: how a page talks to the database (API, keys) | To do | |
| 6 | Explain the visitor → page → API → Supabase diagram as if to a new joiner | To do | |
| 7 | Summaries + 3 open questions in the notebook | To do | |

**Review (explain without notes):**
- [ ] What happens when someone opens my page link
- [ ] Front end, back end, database (Zoho example)
- [ ] Why apps use a database instead of Excel
- [ ] My vendor + invoice table design and the link between them
- [ ] What an API key is and which kind must stay secret

## Day 8 – What AI really is, and where it goes wrong

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: how Claude works | To do | |
| 2 | Catch the mistake: 5 GST/TDS questions, mark wrong / half-right / unsure | To do | |
| 3 | Session 2 chat: context and tokens | To do | |
| 4 | Ask about Day 7 outside vs inside the Project; explain the difference | To do | |
| 5 | Session 3 chat: many AI models | To do | |
| 6 | Same question to Claude and ChatGPT/Gemini; comparison table | To do | |

**Review (explain without notes):**
- [ ] How Claude produces an answer
- [ ] Why AI can be confidently wrong, with my own example
- [ ] What context is, and why one chat per topic
- [ ] One difference between models, and when I'd pick which

## Day 9 – Claude's toolbox

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: chat, Projects, files, search | To do | |
| 2 | 20 fake bank entries in Excel; Claude categorises and totals; check line by line | To do | |
| 3 | Session 2 chat: artifacts | To do | |
| 4 | TDS calculator artifact: write spec first, test 5 known cases, find and fix 1 mistake | To do | |
| 5 | Session 3 chat: Claude Code | To do | |
| 6 | "Explain this project", then Plan mode for 1 small change, then "explain what you changed" | To do | |
| 7 | One line each: when I use chat, a Project, an artifact, Claude Code | To do | |

**Review (explain without notes):**
- [ ] Which part of Claude for 4 situations my manager names
- [ ] My TDS artifact and the mistake I caught
- [ ] What Plan mode is and why I read the plan first

## Day 10 – Good instructions, and checking AI's work

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: what makes an instruction good | To do | |
| 2 | Rewrite 5 vague instructions; compare vague vs improved results | To do | |
| 3 | Session 2 chat: ask first, plan first | To do | |
| 4 | "Vendor ageing report tool" with and without "ask me questions first, then show your plan" | To do | |
| 5 | Session 3 chat: checking AI's work as a non-coder | To do | |
| 6 | My "Before I accept AI's work" checklist (5–7 points) | To do | |

**Review (explain without notes):**
- [ ] One vague-to-good rewrite and what changed
- [ ] Why "ask me first" and "plan first" help
- [ ] My checklist

## Day 11 – The market: picking the best tool

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: map of AI building tools | To do | |
| 2 | GST invoice calculator page twice: Lovable (free) and Claude Code; compare (fake data only) | To do | |
| 3 | Session 2 chat: choosing with reasons (4 requests) | To do | |
| 4 | Decision table: request → tool → why → risk, plus 2 of my own | To do | |

**Review (explain without notes):**
- [ ] My two GST pages: which I'd pick and why
- [ ] Tool choice for 3 situations my manager names
- [ ] Why company or client data never goes into free tools

## Day 12 – From a one-line request to a clear brief (Expense Claim app)

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: interview Claude acting as the requester | To do | |
| 2 | Write `prd.md`: users, what it does, screens, rules, Must have / Nice to have | To do | |
| 3 | Session 2 chat: break it into build steps | To do | |
| 4 | Add "Build steps" with a "Done when…" line for each | To do | |
| 5 | Send `prd.md` to my manager before the review | To do | |

**Review (explain without notes):**
- [ ] The brief is clear enough for someone else to build from
- [ ] Why each Nice to have is not a Must have
- [ ] Why the build steps are in that order

## Day 13 – Data, screens, and who sees what

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: design the tables (Claude asks, I design) | To do | |
| 2 | Draw the tables; compare with employee master / transactions / maker-checker; Claude reviews | To do | |
| 3 | Session 2 chat: screens and flow + clickable mockup artifact | To do | |
| 4 | Walk the mockup as employee and as manager; get at least 2 things changed | To do | |
| 5 | Session 3 chat: login, roles, Row Level Security | To do | |
| 6 | Access rules in plain words added to `prd.md` (with tables and screens) | To do | |

**Review (explain without notes):**
- [ ] My tables and how they link
- [ ] Mockup walk-through as employee and manager
- [ ] How the app stops an employee seeing others' claims

## Day 14 – Build part 1: setup, login, claim submission

Safety rules: 1) no passwords or keys in GitHub (ask "is anything secret in this change?" before every push) · 2) fake data only · 3) ask my manager before deleting files, tables or data.

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: setting up a project the right way | To do | |
| 2 | Repo `expense-claims` with `prd.md`, `rules.md` (safety rules, plan first, ask before adding tables, explain changes simply), empty `handoff.md` | To do | |
| 3 | Plan mode: plan for login + claim submission; check tables match Day 13 | To do | |
| 4 | Build on a new branch; ask "explain what you changed and why" after each change | To do | |
| 5 | Test each screen with fake users using my Day 10 checklist | To do | |
| 6 | Update `handoff.md`, open a pull request, merge | To do | |
| 7 | Notebook: one change I understand, one I don't yet | To do | |

**Review (explain without notes):**
- [ ] Live demo: log in as employee and submit a claim
- [ ] One change Claude made, and why
- [ ] My `rules.md`, and no secret keys in the repo

## Day 15 – Build part 2, and testing like an auditor

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | New Claude Code chat that reads `handoff.md` first | To do | |
| 2 | Plan and build the manager screen: pending claims, approve/reject with remark | To do | |
| 3 | Test full flow: submit → approve → employee sees "Approved" | To do | |
| 4 | Session 2 chat: how software is tested; my test checklist | To do | |
| 5 | Run checklist (pass/fail), fix failures, retest; try blank, negative, very long description | To do | |
| 6 | Update `handoff.md`, pull request, merge; keep test results | To do | |

**Review (explain without notes):**
- [ ] Live demo of the full flow
- [ ] My test checklist with results
- [ ] One problem I found myself, and how it was fixed

## Day 16 – Going live and working like a team

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: putting a real app live (GitHub Pages vs Vercel vs Netlify) | To do | |
| 2 | Put the app live; run 3 checklist tests on my phone; confirm no secret key visible | To do | |
| 3 | Session 2 chat: how a team works on one app | To do | |
| 4 | One improvement on a branch; PR with what / why / how tested; explain each change | To do | |
| 5 | Share the live link with my manager | To do | |

**Review (explain without notes):**
- [ ] Live link works on my manager's phone
- [ ] What happens between my push and the live app updating
- [ ] What a good pull request description contains

## Day 17 – Finding the real cause of a problem

FR comment format: Problem · Root cause · Fix · Tested · Status (Fixed / Need more info)

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Session 1 chat: root cause thinking, error messages, browser console | To do | |
| 2 | FR 1: repeat → root cause → fix on branch `fr-1-…` → retest | To do | |
| 3 | FR 2: repeat → root cause → fix on branch `fr-2-…` → retest | To do | |

**Review (explain without notes):**
- [ ] One FR end to end: problem, root cause, fix, test
- [ ] Fixing the cause vs hiding the problem

## Day 18 – Finishing FRs and talking to users

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Finish remaining FRs; rerun full checklist on the live app | To do | |
| 2 | Session 2 chat: writing to users | To do | |
| 3 | User comment for each FR; questions + "Need more info" for any vague FR | To do | |

**Review (explain without notes):**
- [ ] FR comments readable by a non-technical person
- [ ] How I handled the vague FR

## Day 19 – Build something new, on my own

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Get the one-line request from my manager | To do | |
| 2 | Pick the tool and write down why | To do | |
| 3 | Short brief: users, screens, data, rules, Must have | To do | |
| 4 | Build, test, put live if the tool allows | To do | |

**Review:**
- [ ] Why I chose that tool
- [ ] My brief, and how close the app is to it
- [ ] What I'd do differently next time

## Day 20 – Finish, demo, and the road ahead

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Finish the Day 19 app | To do | |
| 2 | `README.md` for the expense app | To do | |
| 3 | 20-minute demo: profile page, expense app, one FR, Day 19 app | To do | |
| 4 | Notebook: 3 things I'm confident about, 3 I still find hard | To do | |

**Sign-off (8 or more = ready for small real tasks):**
- [ ] Explain why we need VS Code, Git, GitHub, a database and hosting, and how they fit
- [ ] Explain how AI works, where it goes wrong, how I check it
- [ ] Choose the right AI tool for a request, with reasons
- [ ] Turn a one-line request into a clear brief with build steps
- [ ] Design simple tables, screens and access rules
- [ ] Use Claude Code with Plan mode and explain its changes
- [ ] Test like an auditor and fix what fails
- [ ] Find a root cause and write a clear user update
- [ ] Follow the 3 safety rules without being reminded
- [ ] Build a small app alone from a one-line request

## Extra – PO–Invoice Checker MVP (23 Oct 2026)

Built ahead of the plan (the app part belongs to Days 12–16), with fake data only.

| # | Task | Status | Proof |
|---|---|---|---|
| 1 | Plan approved in Plan mode (CSV upload, new repo + GitHub Pages) | Done | |
| 2 | Repo `po-invoice-checker`, README on `main` | Done | commit cc5eff4 |
| 3 | App on branch `mvp-checker`: 6 checks, 5 samples, templates | Done | commit 2b270de |
| 4 | Secret check before push (no keys or passwords) | Done | nothing found |
| 5 | PR opened and merged | Done | https://github.com/renukajadhav-spec/po-invoice-checker/pull/1 |
| 6 | Live on GitHub Pages | Done | https://renukajadhav-spec.github.io/po-invoice-checker/ |
| 7 | Run all 5 samples on the live link + screenshots | To do | |
| 8 | PDF and image upload with a review step (pdf.js + Tesseract.js OCR, fake sample PDFs/PNG) | Pushed, PR to merge | commit 25e6a33 on branch `pdf-image-upload` |
