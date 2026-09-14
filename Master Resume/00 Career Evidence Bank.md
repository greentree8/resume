# Career Evidence Bank

This is the source of truth for resume facts. Add evidence here before tailoring a resume.

## Fintive

### Scope
- Multi-tenant financial-services platform for banking workflows
- Work across loan, obligor, collateral, financial statement, risk-review, export, and document workflows
- Technical environment: React, TypeScript, Node.js, Express, MySQL, Sequelize, Playwright, Vitest, Cypress, Redux Toolkit, AWS, Auth0, and Docker
- Cloud experience: Fintive work was performed on AWS.

### Quantified Evidence
- 134 commits attributed to the author's known Git identities in the checked-out repository history
- 55 test-related commits identified by commit subject
- Shadow-copy workflow reduced new-story setup time from approximately 10 minutes to 2 minutes
- Shadow-copy workflow reduced local storage requirements from approximately 1 GB to 200 MB
- Day.js configuration centralized across 10 files
- Repository architecture includes four primary packages, eight business domains, and 51 database tables

### Accomplishments
- Built historical and annualized trend analysis, including per-statement basis selection, trend-table refresh behavior, uneven-period handling, and export summaries showing the number of months represented.
- Expanded Playwright automation for BFS and CRE calculations, debt schedules, DSCR, NOI, EBITDA adjustments, import scenarios, requirement states, and zero-divisor edge cases.
- Built reusable Playwright page objects, fixtures, and custom matchers for complex financial-statement workflows.
- Resolved defects involving CRE DSCR and CFADS formulas, pro forma adjustments, deposit-rate normalization, balance-sheet liquidity, debt-schedule periodization, and historical-period handling.
- Improved data integrity across loan, obligor, and document workflows by fixing trial-date persistence, debt-schedule row ordering, exposure-table borrower navigation, existing-obligor rendering, and entity document rollover behavior.
- Hardened AI-assisted appraisal and document-extraction workflows with malformed-JSON handling, retry behavior, feature-flagged rollout controls, and bank-cohort configuration.
- Centralized Day.js configuration to eliminate repeated plugin registration and improve Vitest test isolation and performance.
- Collaborated with business stakeholders, project leadership, and subject-matter experts to clarify an ambiguous pro forma and historical reporting request, prototype the workflow, uncover unstated requirements, and deliver the feature on schedule and within budget.
- Applied AI-assisted workflows to codebase analysis, story refinement, requirements clarification, technical documentation, troubleshooting, test planning, and implementation support.
- Shared practical AI techniques with teammates and influenced engineering practices around TypeScript standards, automated testing, documentation quality, code review, maintainability, and technical-debt management.
- Influenced TypeScript engineering practices by replacing loosely modeled boolean state with domain-specific enums, removing unnecessary type assertions, aligning shared client/server/export types, and promoting consistent type-safe patterns through code review.

## OCG Companies

### Scope
- Director of Software Development / Technical Lead, August 2021 through November 13, 2025.
- Led MegaMax and related operational platforms supporting field services, utilities, finance, reporting, dispatch, and customer visibility.
- Managed four offshore engineers, two onshore engineers, and one intern.
- Much of the OCG platform work was performed on AWS.
- Developed, but did not fully implement, a warehouse storage system for equipment and supplies.
- Added supplies and equipment tracking to MegaMax job-cost reporting, giving the business visibility into materials and equipment associated with work.

### Accomplishments
- Led initiatives from concept through delivery while remaining hands-on in architecture, development, troubleshooting, and stakeholder engagement.
- Translated vague business requests into production-ready solutions through iterative discovery, stakeholder feedback, pragmatic technical design, and prioritization.
- Improved SDLC execution through stronger documentation, QA automation, release planning, issue triage, engineering standards, and repeatable development practices.
- Designed the API and workflow foundation for Jarvis, a native mobile operations app providing personalized foreman job lists, map-based planning, efficient route organization, scheduling, and field job management.
- Served as a primary API designer and code reviewer, frequently providing concrete implementation patterns that connected job dimensions, task configuration, crew eligibility, completion state, and mobile scheduling behavior.
- Designed and reviewed MegaMax reporting APIs and implementation patterns across job cost, measurement, job status, activity, billing, and field-operation workflows.
- Led the Fleetio integration for MegaMax equipment workflows, synchronizing vehicle types and fleet records into the internal equipment model, mapping external fields to operational work types, and supporting create, update, and delete webhooks.
- Connected Fleetio vehicle status and meter data to crew check-in and job-scheduling workflows, exposing current vehicle state, measurement units, mileage, and warnings for field operations.
- Expanded Job Cost into an admin-configurable domain with React setup screens, PHP controllers, domain objects, DAOs, services, routes, migrations, and configuration options for job-cost items and equipment.
- Improved soft-surface and hard-surface measurement reports with manager filters, multi-select workflows, duplicate-measurement handling, report counts, export fixes, and billing-oriented corrections.
- Turned Job Search into a reusable ad-hoc reporting tool by adding filters and drill-down detail for dates, customers, jurisdictions, work dimensions, tasks, statuses, and other operational attributes; supported saved searches as standardized reports.
- Designed the migration from MegaMax's existing Miss Dig objects and workflows to a new provider model, accounting for new fields and concepts while preserving ticket status visibility, live refresh, and automatic or manual ticket-to-job assignment.
- Guided a team member through the broader Miss Dig rewrite using the migration design, improving status accuracy and timeliness while reducing back-office effort to maintain ticket-job associations and getting assignments to field workers faster.
- Designed and delivered a GIS-enabled utility pole inspection platform for a new business offering, connecting field data capture, office operations, inspections, reporting, billing support, and customer visibility.
- Integrated ArcGIS Online and spatial visualization into utility-inspection and asset-management workflows, and automated maps, dashboards, reporting, and project tracking.
- Designed a greenfield pole-inspection platform that scaled from approximately 200 to 1,000 poles per week, connecting ArcGIS Online mapping, offline field capture, inspection photos, Dcalc structural analysis, audit dashboards, customer reporting, and contract-based billing.
- Reduced false-positive audit findings from approximately 300 per 1,000 poles to fewer than 40 per 1,000 poles by creating dashboards that flagged likely errors across roughly 50 inspection data points for targeted review.
- Designed the ArcGIS data model, map templates, field-user configuration, and APIs for inspection data and photo exchange; replaced manual photo association with offline-capable workflows that linked evidence to the correct pole in low-connectivity areas.
- Automated customer-specific billing output by combining precise inspection results with contract-pricing rules, while standardizing map generation through reusable segment, icon, and color templates.

## Pearson VUE

### Scope
- Software Developer, Senior Java Developer, and Engineering Lead, December 2009 through July 2021, immediately followed by the OCG role beginning in August 2021.
- Enterprise candidate-registration and client-facing systems supported by distributed Java services and modernized web application platforms.
- Technical environment: Java EE, Spring, Spring Data, Hibernate, JPA, OAuth2, AngularJS, Backbone.js, Node.js, Gradle, JBoss, TeamCity, JUnit, Mockito, and PowerMockito.
- Much of the Pearson VUE work was performed on Microsoft Azure.

### Accomplishments
- Progressed from software developer to engineering lead while delivering and supporting enterprise candidate-registration and client-facing applications.
- Led onshore and offshore development work and coordinated backlog readiness with business analysis, project management, quality engineering, and management stakeholders.
- Helped pilot rich-client JavaScript single-page application patterns backed by RESTful Java services and distributed service integrations.
- Helped establish Agile delivery, code review, automated testing, mentoring, and cross-team knowledge-sharing practices.
- Owned defect triage by prioritizing reported issues, assessing root causes, assigning work across teams, and implementing fixes and enhancements.
- Resolved complex multi-tier issues involving domain-object serialization, cross-tier proxy communication, RESTEasy error handling, and application-infrastructure behavior.
- Worked with architects to standardize REST practices, HTTP error-code usage, REST verbs, JPA patterns, and persistence-layer conventions.
- Introduced and trained teammates on Mockito and PowerMockito testing and mocking practices.

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
