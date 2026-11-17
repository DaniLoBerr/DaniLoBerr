# Hi, I'm Dani 👋

**Software QA Engineer with QA Lead responsibilities.** AI-Driven Testing · Test Strategy · API, Web & Android · Test Automation · Python · pytest · SQL · Docker · Linux

I'm the only QA at a software company in Valencia, Spain, where I built the QA function from scratch for three products, two of them for video and live streaming. I run it as an AI-driven process: AI agents execute the tests on web, API and Android, and I verify every finding. Before software I spent nearly a decade running the technical side of live radio programmes and nearly two years in live event sound, and I earned a certificate in telecommunications infrastructure.

I'm studying a part-time Computer Engineering degree at UOC, and in my free time I'm building my test automation with an open-source test suite.

---

## 🎯 What I'm looking for

**A QA Engineer role inside an established QA team with mature engineering practices, where I can grow my test design and automation and learn from more experienced engineers.** In return, I'd bring an end-to-end view of the test process, from planning to the confirmation test, and real experience using AI agents in testing with the checks they need. I'm an EU citizen, open to relocation or to a fully remote role.

📫 **Contact:** [LinkedIn](https://www.linkedin.com/in/daniloberr) · daniellopezberrocal@gmail.com

## 🧭 What I'm building

### The roadmap

**[vikunja-test-suite](https://github.com/DaniLoBerr/vikunja-test-suite)** — an automated test suite for Vikunja, an open-source task manager, tested from the outside the way a QA team tests an app it didn't write. It grows one version at a time, from API tests in CI towards the infrastructure that runs them, and each version is published as a tagged release.

**✅ Done — the environment and the first tests.** Vikunja runs locally in Docker Compose, pinned to a fixed version. One script brings it up and creates a test user through the API; another tears it down with its data. The first API tests are in Python with pytest and HTTPX, on fixtures for the HTTP client and the authentication token.

**🔜 v0.1 — CI and the first API tests** *(in progress)*. The suite runs on GitHub Actions on every push, with Vikunja inside the job, and a green run is required to merge. The first API tests cover the full lifecycle of a project: create, read and list, update and delete. The README explains the test strategy: what is tested through the API, what isn't, and why.

**v0.2 — The first UI flow with Playwright.** The login flow, end to end, in Python with Playwright and the Page Object pattern, running in the same CI as the API tests. The README adds what is tested through the UI, what through the API, and what never.

**v0.3 — Automation in depth.** A reusable framework, with uv, ruff, a custom API client and test markers. Test data is created and cleaned up, so no test depends on the order they run in. The API is covered in depth: negative and boundary cases, 401 and 403 checks, responses validated with pydantic, and the task operations that depend on a project. More UI flows (projects, tasks, filtering and deleting), with state prepared through the API and checked through the UI, to keep the suite fast and stable.

**v0.4 — Jenkins, Bash and the suite in its own container.** Docker in depth (images, layers, networks and volumes) on the suite's own setup. Its own Dockerfile and a test service in Docker Compose: one command brings Vikunja up and runs the suite, the same locally as in CI. Bash scripts to bring the suite up, seed data and collect logs, checked with shellcheck and used by CI. And the same pipeline as a Jenkinsfile on a local Jenkins, compared with GitHub Actions.

**v0.5 — Performance with k6.** A first scenario, then realistic load against the API, running in CI with thresholds that fail the build, and a report in the README.

**v0.6 — A cloud test environment with Terraform.** Vikunja on AWS, built from code with Terraform, with a second environment, and a CI job that deploys it, runs the suite and destroys it.

**v0.7 — Kubernetes.** Vikunja on a local cluster, and the suite running against it as a Kubernetes Job.

**v1.0 — Security testing.** Authorization tested from the outside: a guest can't write, and nobody sees what wasn't shared with them. A basic OWASP ZAP scan of the API runs in CI, with its report on every run.

---

## 💼 Where I am right now

**Software QA Engineer @ Elite Sports 17** *(since January 2026)* — the company's only QA engineer, working as a QA Engineer with some QA Lead responsibilities, covering three products, each with a web app and a native Android app. There was no QA function before me: I built it on hands-on testing, and scaled it into an AI-driven process. AI agents take most of the test execution; I cover the test management activities of the ISTQB process: planning, monitoring and control, and completion.

- The QA process lives in Git, organised by the phases of the ISTQB test process: a master test plan, the test conditions, test cases with traceability, and the results of every run
- I built and run the execution workflow: AI agents (Claude) execute the test cases through the browser, the API and the Android emulator and draft the results and defects, and I test what the emulator can't reproduce on a physical device
- I verify by hand every defect the agents find before it is published, approve what reaches development, and triage it as an issue in the product's repository (severity, priority, assignee); every fix gets a confirmation test and regression testing around the change, and one that only partly passes stays open
- I audited my own QA process with metrics from Git, GitHub and AI usage, and I lead a phased plan to improve it: risk-based verification tiers, batch approval, WIP limits, acceptance sampling, and new tooling in rollout (Playwright, Hurl, Maestro, axe-core, visual regression)
- I orchestrate the AI agents, one session per product plus a coordinator, with security guardrails as code: a Claude Code hook that blocks forbidden commands, covered by its own tests and replayed against real commands with zero false positives
- I scope and prioritise the testing of each release
- I own the public user guide of the video product: I walked through its flows with the app and the real recording device, and I publish its changes
- I also run quality reviews of training datasets for computer-vision models, carried out by AI agents (Claude) against written criteria, with a report per batch

**What I'm learning and applying at work:** taking back the hands-on testing role without letting go of test management, with a structured learning plan applied to real releases:

- **Test design techniques** on real features and fixes: equivalence partitioning, boundary values, decision tables and state transitions, and selective regression around each change
- **Technical diagnosis:** API traffic in DevTools, status codes and permissions, placing each failure in its layer (web, API, data or environment), Android debugging with adb and logcat, and Git to know exactly which build and which change I'm testing
- **Reviewing AI output with judgement:** my own catalogue of how the agents get things wrong, practice reviews with seeded defects, and one extra test the AI didn't list in each daily check, so every defect I sign off is one I could have found myself
- **ISTQB CTFL v4.0** in preparation alongside it

---

## 🛠️ Stack

| | |
|---|---|
| **Using at work** | Claude and Claude Code (AI agents, hooks) · Git and GitHub (branches, pull requests, issues) · Postman · Chrome DevTools · Android Studio emulator · Linux (Ubuntu) · API testing · mobile (Android) testing · test planning and test case design · defect management |
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

My whole career has been with technical equipment: first sound and radio, then telecommunications, and now software. What I want next is to keep growing in QA inside a team I can learn from, writing more test code along the way.
