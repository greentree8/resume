# Career Evidence Bank

This is the source of truth for resume facts. Add evidence here before tailoring a resume.

## Fintive

### Scope
- Multi-tenant financial-services platform for banking workflows
- Work across loan, obligor, collateral, financial statement, risk-review, export, and document workflows
- Employment dates: November 2025 through August 2026 (end date confirmed 2026-10-27).
- Technical environment: React, TypeScript, Node.js, Express, MySQL, Sequelize, Playwright, Vitest, Cypress, Redux Toolkit, AWS, Auth0, Docker, Bash, and Claude Code
- Cloud experience: Fintive work was performed on AWS.
- Fintive platform operated under SOC and PII compliance constraints (source: personal recollection, 2026-10-16).

### Quantified Evidence
- 134 commits attributed to the author's known Git identities in the checked-out repository history
- 55 test-related commits identified by commit subject
- Standardized reusable fixtures and templates to ensure stable test behavior across the engineering team; productivity impact was not measured.
- Stabilized flaky tests and reduced CI pipeline reruns, saving approximately 5-15 hours of deployment-pipeline time per month.
- Converted exploratory test findings into structured user stories, accelerating sprint velocity by approximately 0.5-1 day per sprint.
- Shadow-copy workflow reduced new-story setup time from approximately 10 minutes to 2 minutes
- Shadow-copy workflow reduced local storage requirements from approximately 1 GB to 200 MB
- Day.js configuration centralized across 10 files
- Repository architecture includes four primary packages, eight business domains, and 51 database tables

### Accomplishments
- Built historical and annualized trend analysis, including per-statement basis selection, trend-table refresh behavior, uneven-period handling, and export summaries showing the number of months represented.
- Did a lot of integration testing with Playwright, written as end-to-end tests (source: personal recollection, 2026-10-27; confirm the tests ran against the real API and database rather than mocks).
- Expanded Playwright automation for BFS and CRE calculations, debt schedules, DSCR, NOI, EBITDA adjustments, import scenarios, requirement states, and zero-divisor edge cases.
- Built reusable Playwright page objects, fixtures, and custom matchers for complex financial-statement workflows.
- Resolved defects involving CRE DSCR and CFADS formulas, pro forma adjustments, deposit-rate normalization, balance-sheet liquidity, debt-schedule periodization, and historical-period handling.
- Improved data integrity across loan, obligor, and document workflows by fixing trial-date persistence, debt-schedule row ordering, exposure-table borrower navigation, existing-obligor rendering, and entity document rollover behavior.
- Hardened AI-assisted appraisal and document-extraction workflows with malformed-JSON handling, retry behavior, feature-flagged rollout controls, and bank-cohort configuration.
- Centralized Day.js configuration to eliminate repeated plugin registration and improve Vitest test isolation and performance.
- Collaborated with business stakeholders, project leadership, and subject-matter experts to clarify an ambiguous pro forma and historical reporting request, prototype the workflow, uncover unstated requirements, and deliver the feature on schedule and within budget.
- Used Claude Code heavily as a core development tool, with agents and subagents automating much of the development process (source: personal recollection, 2026-10-23).
- Applied AI-assisted workflows to codebase analysis, story refinement, requirements clarification, technical documentation, troubleshooting, test planning, and implementation support.
- Strong transferable QA, data-quality, SQL, automation, reporting, and business-rule experience across financial-analysis and operational workflows.
- Wrote Bash scripts to automate development tasks and complex Git workflows; the shadow-copy workflow was implemented in one of these scripts (source: personal recollection, 2026-10-19).
- Shared practical AI techniques with teammates and influenced engineering practices around TypeScript standards, automated testing, documentation quality, code review, maintainability, and technical-debt management.
- Influenced TypeScript engineering practices by replacing loosely modeled boolean state with domain-specific enums, removing unnecessary type assertions, aligning shared client/server/export types, and promoting consistent type-safe patterns through code review.

- Collaborated with the team to design and build a three-agent Claude code review covering functional review, code analysis, and coding standards; all three reviews had to pass, and the agents exchanged findings (source: personal recollection, 2026-10-28).
- Guided Claude with the team's existing coding standards and React and Node.js patterns to write full features, then verified the patterns were followed (source: personal recollection, 2026-10-28).
- Met regularly with teammates to develop new Claude skills and improve AI-assisted coding practices (source: personal recollection, 2026-10-28).
- The shadow-copy workflow supported a per-story Git worktree process; 10 minutes to 2 minutes confirmed (source: personal recollection, 2026-10-28).
- Trained Claude continuously while using it: found errors and mistakes and corrected them permanently with memories and instructions (source: personal recollection, 2026-10-28). Examples (source: personal recollection, 2026-10-28):
  - Spelled out common mistakes, such as preferring role-based locators over CSS selectors in Playwright tests.
  - Built a dictionary of domain language so naming stayed consistent and clear.
  - Gave explicit code snippets showing the best way to handle tricky UI interactions, such as toast popups.
- Created Claude skills for routine work: pulling up diffs against branches and gauging change complexity, creating pull requests with before-and-after screenshots via the Playwright MCP server, and writing detailed PR descriptions of the code changes and why they were needed (source: personal recollection, 2026-10-28).
- Wrote shell script utilities with AI help and shared them with the team, including resetting the local dev environment, cleaning up build artifacts, and building and resetting Docker images (source: personal recollection, 2026-10-28).
- Used AI to load and analyze AWS logs to troubleshoot production issues (source: personal recollection, 2026-10-28).
- Used AI heavily to analyze existing front-end and back-end code patterns and extracted rules to use going forward for new development and end-to-end tests (source: personal recollection, 2026-10-28).

## OCG Companies

### Scope
- Director of Software Development / Technical Lead, August 2021 through November 13, 2025.
- Led MegaMax and related operational platforms supporting field services, utilities, finance, reporting, dispatch, and customer visibility.
- Managed four offshore engineers, two onshore engineers, and one intern.
- Offshore engineers were supplied through a vendor. Owned the entire relationship with that vendor, meeting with its technical and business owners, negotiating vendor costs, and meeting regularly to maintain team performance and address concerns (source: personal recollection, 2026-10-16 and 2026-10-20; confirmed 2026-10-20 that this was the offshore staffing vendor, not Fleetio).
- Set performance goals, including SMART goals, with all developers (source: personal recollection, 2026-10-20).
- Some feature requests had hard deadlines; other work followed a regular release schedule managed internally (source: personal recollection, 2026-10-20).
- Team measured throughput by story points and completed stories per week, and set its own goals to improve estimation accuracy and predictability; not dictated top-down (source: personal recollection, 2026-10-20).
- Built the engineering team from scratch, screening candidates and making the final hiring decisions (source: personal recollection, 2026-10-15; confirm number of candidates screened).
- Much of the OCG platform work was performed on AWS.
- Developed, but did not fully implement, a warehouse storage system for equipment and supplies.
- Added supplies and equipment tracking to MegaMax job-cost reporting, giving the business visibility into materials and equipment associated with work.

### Accomplishments
- Met with senior leadership to develop a new roadmap for MegaMax, and established product owners and a structure for communication and sign-off on feature development. Reported regularly to senior leadership on features deployed and on user-requested features before implementing them (source: personal recollection, 2026-10-19).
- Led initiatives from concept through delivery while remaining hands-on in architecture, development, troubleshooting, and stakeholder engagement.
- Translated vague business requests into production-ready solutions through iterative discovery, stakeholder feedback, pragmatic technical design, and prioritization.
- Improved SDLC execution through stronger documentation, QA automation, release planning, issue triage, engineering standards, and repeatable development practices.
- Designed the API and workflow foundation for Jarvis, a native mobile operations app providing personalized foreman job lists, map-based planning, efficient route organization, scheduling, and field job management.
- Served as a primary API designer and code reviewer, frequently providing concrete implementation patterns that connected job dimensions, task configuration, crew eligibility, completion state, and mobile scheduling behavior.
- Designed and reviewed MegaMax reporting APIs and implementation patterns across job cost, measurement, job status, activity, billing, and field-operation workflows.
- Used GitHub Copilot extensively to accelerate development (source: personal recollection, 2026-10-23).
- Heavy SQL experience: wrote reporting queries, custom ad hoc queries, and complex queries backing MegaMax search functionality (source: personal recollection, 2026-10-15).
- Led the Fleetio integration for MegaMax equipment workflows, synchronizing vehicle types and fleet records into the internal equipment model, mapping external fields to operational work types, and supporting create, update, and delete webhooks.
- Connected Fleetio vehicle status and meter data to crew check-in and job-scheduling workflows, exposing current vehicle state, measurement units, mileage, and warnings for field operations.
- Fixed an existing, broken notification system for sending account-assistance emails; did not build it originally (source: personal recollection, 2026-10-20).
- Wrote custom ETL scripts to transform client-formatted pole data into the ArcGIS database structure (source: personal recollection, 2026-10-19).
- Data imports were push-button triggered and ran without manual intervention; not scheduled, but could have been (source: personal recollection, 2026-10-16); confirm which imports (assumed ArcGIS pole-data imports).
- Expanded Job Cost into an admin-configurable domain with React setup screens, PHP controllers, domain objects, DAOs, services, routes, migrations, and configuration options for job-cost items and equipment.
- Improved soft-surface and hard-surface measurement reports with manager filters, multi-select workflows, duplicate-measurement handling, report counts, export fixes, and billing-oriented corrections.
- Turned Job Search into a reusable ad-hoc reporting tool by adding filters and drill-down detail for dates, customers, jurisdictions, work dimensions, tasks, statuses, and other operational attributes; supported saved searches as standardized reports.
- Designed the migration from MegaMax's existing Miss Dig objects and workflows to a new provider model, accounting for new fields and concepts while preserving ticket status visibility, live refresh, and automatic or manual ticket-to-job assignment.
- Guided a team member through the broader Miss Dig rewrite using the migration design, improving status accuracy and timeliness while reducing back-office effort to maintain ticket-job associations and getting assignments to field workers faster.
- Designed and delivered a GIS-enabled utility pole inspection platform for a new business offering, connecting field data capture, office operations, inspections, reporting, billing support, and customer visibility.
- Worked directly with every user group, including back-office staff, field users, finance analysts, internal stakeholders, and clients (source: personal recollection, 2026-10-15).
- On the pole-inspection program, met weekly with clients to monitor software usability and stability and identify improvements (source: personal recollection, 2026-10-15).
- Trained field workers both on inspection procedures and on using the inspection software the team built (source: personal recollection, 2026-10-15).
- Configured and deployed the field data-collection app (ArcGIS Collector) and maps through ArcGIS Online, a low-code configuration platform, rather than custom code. Trained a foreman to independently set up new maps and arrange crew assignments in ArcGIS Online once data was imported (source: personal recollection, 2026-10-19).
- Integrated ArcGIS Online and spatial visualization into utility-inspection and asset-management workflows, and automated maps, dashboards, reporting, and project tracking.
- Designed a greenfield pole-inspection platform that scaled from approximately 200 to 1,000 poles per week, connecting ArcGIS Online mapping, offline field capture, inspection photos, Dcalc structural analysis, audit dashboards, customer reporting, and contract-based billing.
- Pole-inspection audit dashboards were custom code, not ArcGIS Dashboards (source: personal recollection, 2026-10-19).
- Reduced false-positive audit findings from approximately 300 per 1,000 poles to fewer than 40 per 1,000 poles by creating dashboards that flagged likely errors across roughly 50 inspection data points for targeted review.
- Designed the ArcGIS data model, map templates, field-user configuration, and APIs for inspection data and photo exchange; replaced manual photo association with offline-capable workflows that linked evidence to the correct pole in low-connectivity areas.
- Automated customer-specific billing output by combining precise inspection results with contract-pricing rules, while standardizing map generation through reusable segment, icon, and color templates.

- Team composition confirmed: four offshore developers, two onshore developers (one short-term local developer), and one intern; one team member handled QA and also developed. A half-time business analyst on loan ran Jira reporting and story refinement with a dotted-line report (source: personal recollection, 2026-10-28).
- Held one-on-ones with each developer and onboarded developers onto team systems; HR handled formal onboarding paperwork (source: personal recollection, 2026-10-28).
- Replaced annual reviews with monthly performance conversations that fed into year-end raises (source: personal recollection, 2026-10-28).
- Main contact point for every user group, gathering and coordinating requests and managing stakeholder expectations about what could and could not be delivered (source: personal recollection, 2026-10-28).
- OCG had two of its best years while using the software heavily; partial credit only (source: personal recollection, 2026-10-28).
- Encouraged offshore developers to use AI heavily. Created an AI code-review prompt developers ran first to catch naming and style issues, followed by a human review of structure and functionality (source: personal recollection, 2026-10-28).
- Used an automated AI code-review tool on every check-in (tool name unconfirmed; possibly Qodo), later moving AI code review to GitHub Copilot and Claude (source: personal recollection, 2026-10-28).
- Built client-facing job progress, job status, and photo report pages (three pages) largely with GitHub Copilot, enforcing strict per-client data isolation in a multi-client system. Real clients beta tested in production about one week after requirements were settled; refinements finished in about three weeks (source: personal recollection, 2026-10-28).
- Migrated MegaMax front end off PHP-rendered pages toward React (and Vue.js): no new PHP front-end code, PHP front-end pages rewritten in React when touched, PHP retained for back-end services. The cutoff was David's decision (source: personal recollection, 2026-10-28).
- Each client had configured billing rules, job types, and measurements; automated bill delivery in the specific format required by a Detroit electric utility (source: personal recollection, 2026-10-28).
- Code review became a bottleneck: David was spending review time on issues (style, naming) that should not have reached him, when his focus needed to be logic and business goals. He implemented an AI code review with specific instructions that developers ran before handing off for his review; by his estimate it caught about 90% of those issues, freeing his reviews for product quality and making the team more self-reliant and efficient (source: personal recollection, 2026-10-28). AI review began around late September/October 2024 (confirmed 2026-10-28). The AI review prompt was introduced shortly after the team started using AI; earlier recollection of AI adoption "around 2023" may be early (source: personal recollection, 2026-10-28).
- MegaMax git history (analyzed 2026-10-28): commits by other developers referencing PR/MR/review suggestions rose from 0 (Jan-May 2024) to 2 of 49 (Jun), 10 of 104 (Jul), 11 of 102 (Aug), and 15 of 107 (Sep 2024, 14%), then 0 of 75 in Oct 2024 and 1 total from Nov 2024-May 2025. PR feedback still happened after October 2024 but was likely committed under messages like "fix xyz", so describe the drop as "nearly 0%" (source: personal recollection, 2026-10-28). Causation is inferred from timing; release speed could not be measured because activity declined from Nov 2024 as OCG wound down.
- Coaching cadence: standups three times a week, one-on-one coaching and feedback twice a month with each developer, and ad hoc check-ins while monitoring story progress (source: personal recollection, 2026-10-28).
- Offshore developers were all contractors selected from the staffing vendor. Handled the initial contract negotiation and the ongoing relationship as attrition occurred or different skill sets were required, including working through scheduling and workload logistics during a developer's maternity leave (source: personal recollection, 2026-10-28).
- Throughput per sprint increased after the AI review, but this is not measurable from available data; do not claim (source: personal recollection, 2026-10-28).
- Pioneered AI use in OCG software development; the team used it heavily to augment development. Also encouraged business users to use AI in their spreadsheets and other daily workflows, such as assembling photos to send to clients and massaging spreadsheets for import into OCG systems (source: personal recollection, 2026-10-28).
- Collaborated with user groups and stakeholders to establish clear direction for the product, deciding how features fit into the timeline and feature set, and prioritized the work (source: personal recollection, 2026-10-28).
- Screened each offshore contractor candidate from the staffing vendor and built the team to work well with OCG and with each other, with attention to team culture (source: personal recollection, 2026-10-28).
- Miss Dig migration design maintained backward compatibility with existing MegaMax workflows (source: personal recollection, 2026-10-28).
- The code review situation was heading in an unsustainable direction; after the AI pre-review the team became more self-reliant and settled into a performing state, delivering the features the business wanted in the expected timeframe (source: personal recollection, 2026-10-29). A reviewer misread "PR-feedback commits" as "comments"; describe the metric as rework commits from review feedback.

## Pearson VUE

### Scope
- Education note: BYU-Idaho Computer Science coursework; degree not completed (source: personal recollection, 2026-10-16).
- Software Developer, Senior Java Developer, and Engineering Lead, December 2009 through July 2021, immediately followed by the OCG role beginning in August 2021.
- Enterprise candidate-registration and client-facing systems supported by distributed Java services and modernized web application platforms.
- Worked closely with quality assurance engineers to structure and write tests, with a longstanding interest in QA and testability.
- Partnered with QA and development teams to improve accessibility (a11y), semantic correctness, and maintainability of web applications.
- Helped make page elements easier to identify in automated tests by using meaningful named attributes and stable selectors instead of brittle XPath expressions.
- Technical environment: Java EE, Spring, Spring Boot, Spring Data, Hibernate, JPA, OAuth2 (not recalled by David on 2026-10-28; don't use unless confirmed), AngularJS, Backbone.js, Node.js, Gradle, JBoss, TeamCity, Jenkins, Kubernetes, JUnit, Mockito, and PowerMockito.
- Much of the Pearson VUE work was performed on Microsoft Azure; Azure was used almost exclusively (source: personal recollection, 2026-10-19).
- CI/CD mostly used Jenkins; some Azure DevOps usage is believed but not confirmed (source: personal recollection, 2026-10-19).

### Accomplishments
- Progressed from software developer to engineering lead while delivering and supporting enterprise candidate-registration and client-facing applications.
- Led onshore and offshore development work and coordinated backlog readiness with business analysis, project management, quality engineering, and management stakeholders.
- Helped pilot rich-client JavaScript single-page application patterns backed by RESTful Java services and distributed service integrations.
- Helped establish Agile delivery, code review, automated testing, mentoring, and cross-team knowledge-sharing practices.
- Owned defect triage by prioritizing reported issues, assessing root causes, assigning work across teams, and implementing fixes and enhancements.
- Resolved complex multi-tier issues involving domain-object serialization, cross-tier proxy communication, RESTEasy error handling, and application-infrastructure behavior. David doesn't recall "cross-tier proxy communication"; don't use it unless he can explain it (2026-10-28).
- Tuned New Relic alerting and performance metrics, used New Relic and Splunk to troubleshoot reported user issues and resolve account problems, and added application signals for user-conversion and progress tracking to improve the overall user experience.
- Worked with architects to standardize REST practices, HTTP error-code usage, REST verbs, JPA patterns, and persistence-layer conventions.
- Introduced and trained teammates on Mockito and PowerMockito testing and mocking practices.
- Used Spring Boot for API services. Not full microservices (no service discovery), but followed microservice principles, with each service tightly scoped to a single action or domain (source: personal recollection, 2026-10-23).
- Kubernetes was used to automatically scale nodes based on traffic; the team was responsible for initial setup and tuning of each new application according to established templates (source: personal recollection, 2026-10-20).
- Participated regularly in on-call rotations and production release support (source: personal recollection, 2026-10-27).
- Worked on WebNG and VTS (source: personal recollection, 2026-10-28).
- Front-end framework experience at Pearson VUE was AngularJS; no Angular 2+ experience (source: personal recollection, 2026-10-28).
- AngularJS and Backbone.js were likely part of the SPA pilot, but recollection is foggy; did front-end work in both (source: personal recollection, 2026-10-28).
- Integrated an SMS system for candidate notifications, including user opt-in and mobile phone number entry (source: personal recollection, 2026-10-20; confirm level of ownership).

## Previous Employers

Add one section per employer. Capture:
- Business context and product scope
- Role and level of ownership
- Technologies and tools
- Projects delivered
- Problems solved
- Metrics and measurable outcomes
- Leadership, collaboration, and stakeholder examples
- Evidence source: resume, performance review, project record, or personal recollection

## Evidence Rules

- Use exact metrics when documented.
- Label estimates as approximate.
- Do not convert commit counts into business impact claims.
- Keep repository scale metrics as supporting context, not as the primary accomplishment.
- Mark recollections that need confirmation before using them in a final resume.
