# Hi, I'm Dani 👋

**Software QA Engineer with QA Lead responsibilities, moving into QA Automation / SDET.** API, Web & Android Testing · AI-Driven Test Execution · Python · pytest · Linux

I'm the only QA at a software company in Valencia, Spain, where I built the QA function from scratch for three products, two of them for video and live streaming. I run it as an AI-driven process: AI agents execute the tests on web, API and Android, and I verify every finding. Before software I spent nearly a decade running the technical side of live radio programmes and nearly two years in live event sound, and I earned a certificate in telecommunications infrastructure.

I'm studying a part-time Computer Engineering degree at UOC. My next step is writing test code and automating tasks, as a QA Automation engineer or SDET, and growing towards test infrastructure.

---

## 🎯 What I'm looking for

**A QA Automation or SDET role where I write test code and work close to the infrastructure that runs it: CI/CD, test environments, networks or embedded systems**, in an experienced team I can keep learning from. I'm also open to QA Engineer roles. I'm an EU citizen, open to relocation or to a fully remote role.

📫 **Contact:** [LinkedIn](https://www.linkedin.com/in/daniloberr) · daniellopezberrocal@gmail.com

## 🧭 What I'm building

### SDET → Platform 2027

**[vikunja-test-suite](https://github.com/DaniLoBerr/vikunja-test-suite)** — an automated test suite for Vikunja, an open-source task manager, tested from the outside the way a QA team tests an app it didn't write. It grows one version at a time, from API tests in CI towards the infrastructure that runs them, and each version is published as a tagged release.

**✅ Done — the environment and the first tests.** Vikunja runs locally in Docker Compose, pinned to a fixed version. One script brings it up and creates a test user through the API; another tears it down with its data. The first API tests are in Python with pytest and HTTPX, on fixtures for the HTTP client and the authentication token.

**🔜 v0.1 — API suite and CI** *(in progress)*. The API suite for projects, and the task operations that depend on them: positive, negative and boundary cases, and 401 and 403 checks, with responses validated with pydantic. A custom API client and test markers make the suite reusable, and test data is created and cleaned up so no test depends on the order they run in. It runs on GitHub Actions with Vikunja inside the job, and a green run is required to merge. The README explains the test strategy: what is tested through the API, what isn't, and why.

**v0.2 — Robot Framework, Wireshark and Jenkins.** The project cases again in Robot Framework with RequestsLibrary, with their HTML report in CI. The traffic between the tests and Vikunja captured with Wireshark and tshark inside Docker, with a note on diagnosing a failure from a real capture. And the same pipeline as a Jenkinsfile on a local Jenkins, compared with GitHub Actions.

**v0.3 — UI tests with Playwright.** End-to-end tests in TypeScript with Playwright and the Page Object Model, covering the main flows: login, projects, tasks, filtering and deleting. State is prepared through the API and checked through the UI, to keep the suite fast and stable, and the UI tests run in CI next to the API ones. The README adds what is tested through the UI, what through the API, and what never.

**v0.4 — The suite in a container.** Its own Dockerfile and a test service in Docker Compose: one command brings Vikunja up and runs the suite, the same locally as in CI.

**v0.5 — Linux and Bash.** Bash scripts to bring the suite up, seed data and collect logs, checked with shellcheck and used by CI, and a note on following a request end to end with `ip`, `ss`, `curl`, `dig` and `tcpdump`.

**v0.6 — Performance with k6.** Load, stress and spike scenarios against the API with realistic per-user data, running in CI with thresholds that fail the build, and a report with throughput, p95, p99 and where Vikunja starts to degrade.

**v0.7 — A cloud test environment with Terraform.** Vikunja on AWS, built from code with Terraform. The suite runs against the local or the cloud environment by changing only variables, and a CI job creates the environment, runs the suite and destroys it.

**v0.8 — Kubernetes.** Vikunja on a local cluster with its own manifests, and the suite running against it as a Kubernetes Job.

**v1.0 — Security testing.** Authorization tested from the outside: a guest can't write, and nobody sees what wasn't shared with them. A basic OWASP ZAP scan of the API runs in CI, with its report on every run.

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
