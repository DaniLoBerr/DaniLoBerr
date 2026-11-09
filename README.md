# Hi, I'm Dani 👋

**Software QA Engineer with QA Lead responsibilities, moving into QA Automation / SDET.** API, Web & Android Testing · AI-Driven Test Execution · Python · pytest · Linux

I'm the only QA at a software company in Valencia, Spain, where I built the QA function from scratch for three products, two of them for video and live streaming. I run it as an AI-driven process: AI agents execute the tests on web, API and Android, and I verify every finding. Before software I spent nearly a decade running the technical side of live radio programmes and nearly two years in live event sound, and I earned a certificate in telecommunications infrastructure.

I'm studying a part-time Computer Engineering degree at UOC. My next step is writing test code and automating tasks, as a QA Automation engineer or SDET.

---

## 🎯 What I'm looking for

**A QA Automation or SDET role where I write test code and work close to the infrastructure that runs it: CI/CD, test environments, networks or embedded systems**, in an experienced team I can keep learning from. I'm also open to QA Engineer roles, especially fully remote. I'm an EU citizen, open to relocation or to a fully remote role.

📫 **Contact:** [LinkedIn](https://www.linkedin.com/in/daniloberr) · daniellopezberrocal@gmail.com

## 🧭 What I'm building

**[vikunja-test-suite](https://github.com/DaniLoBerr/vikunja-test-suite)** — an automated test suite for Vikunja, an open-source task manager, tested from the outside the way a QA team tests an app it didn't write. It grows one version at a time:

| Version | What it adds |
|---|---|
| ✅ Done | A reproducible test environment in Docker Compose, pinned to a fixed app version, and the first API tests in Python with pytest and HTTPX |
| 🔜 v0.1 | The API suite for projects and tasks, running in CI on every push, with a short test strategy |
| v0.2 | The same API cases in Robot Framework, the suite's network traffic analysed with Wireshark, and the pipeline also running in Jenkins |
| v0.3 | End-to-end UI tests in TypeScript with Playwright |
| v0.4 | The whole suite in its own container: one command brings everything up and runs it |
| v0.5 | Bash tooling for the suite and Linux networking diagnostics |
| v0.6 | Performance tests with k6, with thresholds that fail the build |
| v0.7 | A cloud test environment on AWS, built with Terraform and torn down after each run |
| v0.8 | Vikunja and the suite running on Kubernetes |
| v1.0 | Security testing: permissions between users and an OWASP ZAP scan in CI |

---

## 💼 Where I am right now

**Software QA Engineer @ Elite Sports 17** *(since January 2026)* — the company's only QA engineer, working as a QA Engineer with some QA Lead responsibilities, covering three products, each with a web app and a native Android app. There was no QA function before me: I built it on hands-on testing, and scaled it into an AI-driven process. AI agents take most of the testing role; I mainly hold the test management role: planning, monitoring and control, and completion.

- The QA process lives in Git, organised by the phases of the ISTQB test process: a master test plan, the test conditions, test cases with traceability, and the results of every run
- I built and run the execution workflow: AI agents (Claude) execute the test cases through the browser, the API and the Android emulator and draft the results and defects, and I test what the emulator can't reproduce on a physical device
- I verify by hand every defect the agents find before it is published, approve what reaches development, and triage it as an issue in the product's repository (severity, priority, assignee); every fix gets a confirmation test and regression testing around the change, and one that only partly passes stays open
- I scope and prioritise the testing of each release
- I own the public user guide of the video product: I walked through its flows with the app and the real recording device, and I publish its changes
- I also run quality reviews of training datasets for computer-vision models, carried out by AI agents (Claude) against written criteria, with a report per batch

**What I'm learning and applying at work:** taking back the hands-on testing role without letting go of test management, with a structured learning plan applied to real releases:

- **Test design techniques** on real features and fixes: equivalence partitioning, boundary values, decision tables and state transitions, and selective regression around each change
- **Technical diagnosis:** API traffic in DevTools, status codes and permissions, placing each failure in its layer (web, API, data or environment), Android debugging with adb and logcat, and Git to know exactly which build and which change I'm testing
- **Reviewing AI output with judgement:** my own catalogue of how the agents get things wrong, practice reviews with seeded defects, and one extra test the AI didn't list in each daily check, so every defect I sign off is one I could have found myself
- **ISTQB CTFL v4.0** in preparation alongside it; next in the plan, test automation with pytest

---

## 🛠️ Stack

| | |
|---|---|
| **Using at work** | Claude (AI agents) · Git and GitHub (branches, pull requests, issues) · Postman · Chrome DevTools · Android Studio emulator · Linux (Ubuntu) · API testing · mobile (Android) testing · test planning and test case design · defect management |
| **Building in my own project** | Python · pytest · HTTPX · Docker Compose · API testing |
| **Studied (Harvard CS50)** | Python · C · SQL · pytest · Django · GitHub Actions · relational database design |

---

## 🤖 How I use AI

I use AI every day, and I'm explicit about how. In what I'm still learning, I write the code and the AI explains and reviews. Once I can do something without help, I delegate the repetition and review it like a pull request. At work, AI agents run the tests and draft the documentation, and I verify what they report before anyone else sees it.

---

## 🎓 Background

- **BSc Computer Engineering** — Universitat Oberta de Catalunya *(part-time, since 2026)*
- **Harvard CS50** — CS50x, CS50P (Python), CS50SQL, CS50W *(2024–2025)*
- **Telecommunications infrastructure certificate** *(2021)*, and a one-month internship supporting a copper-to-fibre migration
- **Higher Vocational Degree in Audiovisual Sound** *(2013)*
- **Sound technician in live radio at Cadena COPE** *(2015–2024)*, most of that time as lead sound technician
- **Supporting testing and quality control of professional sound equipment at Rent Music** *(2013–2014)*
- **Six months in Cork, Ireland** *(2025–2026)*, where I studied English
- **Languages:** Spanish (native) · English (C1, full professional proficiency)

---

## 🤔 Why the career change

For nearly a decade I ran the technical side of live radio programmes: the broadcast equipment, the timing, and the first response when something failed on air. In 2024, at 31, I left because I had stopped growing in that job, and I started studying programming on my own. I moved to Ireland to keep studying and improve my English, and in January 2026 I came back to Spain for my first software job, in QA.

My whole career has been with technical equipment: first sound and radio, then telecommunications, and now software. What I want next is to write test code and automate tasks.
