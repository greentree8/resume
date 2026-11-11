# OCG Companies Evidence Dossier

## Role Positioning

Director of Software Development / Technical Lead at OCG Companies from August 2021 through November 13, 2025, leading software delivery while remaining hands-on in architecture, development, troubleshooting, and stakeholder engagement.

## Leadership and Team Scope

- Managed a blended engineering team of four offshore engineers, two onshore engineers, and one intern.
- Built the engineering team from scratch, screening candidates and making the final hiring decisions (personal recollection; confirm counts).
- Offshore engineers were supplied through a vendor. Owned the entire relationship with that vendor, meeting with its technical and business owners, negotiating vendor costs, and meeting regularly to maintain team performance and address concerns (personal recollection, 2026-10-16 and 2026-10-20; confirmed this was the offshore staffing vendor, not Fleetio).
- Set performance goals, including SMART goals, with all developers (personal recollection, 2026-10-20).
- Some feature requests had hard deadlines; other work followed a regular release schedule managed internally (personal recollection, 2026-10-20).
- Team measured throughput by story points and completed stories per week, and set its own goals to improve estimation accuracy and predictability; not dictated top-down (personal recollection, 2026-10-20).
- Met with senior leadership to develop a new roadmap for MegaMax, and established product owners and a structure for communication and sign-off on feature development. Reported regularly to senior leadership on features deployed and on user-requested features before implementing them (personal recollection, 2026-10-19).
- Aligned priorities across business and technical stakeholders.
- Led initiatives from concept through delivery, including architecture, implementation, troubleshooting, and stakeholder communication.
- Improved SDLC execution through documentation, QA automation, release planning, issue triage, engineering standards, and repeatable development practices.
- Translated vague business requests into production-ready solutions through iterative discovery, stakeholder feedback, pragmatic design, and prioritization.

## Jarvis Mobile Operations Platform

- Designed the API and workflow foundation for Jarvis, a native mobile application that gave field crews and foremen more robust scheduling, planning, and job-management capabilities than the prior web workflow.
- Built API patterns that supplied personalized job lists for each crew and foreman, giving users a focused view of their assigned work.
- Supported map-based job planning and efficient route organization so foremen could understand the day's work and plan field activity more effectively.
- Connected job dimensions, task configuration, crew eligibility, completion state, and scheduling data so mobile users received relevant, actionable work information.
- Served as the primary API designer and code reviewer, frequently proposing concrete implementation patterns and reviewing code for consistency, maintainability, and correct cross-layer behavior.

## MegaMax and Operational Platforms

- Led software delivery for MegaMax and related operational platforms supporting field services, utilities, finance, reporting, dispatch workflows, and customer-facing visibility.
- Connected operational workflows with financial processes, reporting, and customer visibility.
- Fixed an existing, broken notification system for sending account-assistance emails; did not build it originally (personal recollection, 2026-10-20).
- Used GitHub Copilot extensively to accelerate development (personal recollection, 2026-10-23).
- Used AI-assisted analysis for technical research, troubleshooting, requirements review, documentation, and development planning as AI tooling became part of the engineering workflow.
- MegaMax architecture: PHP and Laravel for routing and services, with Apache in front; React and Vue.js front-end code bundled with webpack into compact production files for faster downloads and fewer network requests at load time; static content served from a read-only path (source: personal recollection, 2026-11-04).
- MegaMax data tier: MariaDB on AWS, with managed RDS for production and self-managed instances on Linux EC2 servers for lower environments such as test and sandbox (source: personal recollection, 2026-11-04).
- MegaMax used an address normalization service when creating new addresses and jobs (source: personal recollection, 2026-11-04).
- MegaMax job visibility was layered by role: foremen saw only their assigned jobs; client users saw all of their own company's jobs regardless of assigned foreman, and a contract permission, used only for client users, could further limit them to the jobs under a given contract. Back-office project managers set up the contract configuration (source: personal recollection, 2026-11-04).

## Fleetio Integration

- Led the Fleetio integration for MegaMax equipment workflows, synchronizing vehicle types and fleet records into the internal equipment model and mapping external fields to operational work types.
- Implemented support for Fleetio vehicle create, update, and delete webhooks so MegaMax equipment data could remain aligned with the external fleet system.
- Connected Fleetio vehicle status and meter data to crew check-in and job-scheduling workflows, exposing vehicle state, measurement units, mileage, and warnings for field operations.

## MegaMax Reporting, Search, and Job Cost

- Designed and reviewed reporting APIs and implementation patterns across job cost, measurement, job status, activity, billing, and field-operation workflows.
- Heavy SQL experience: wrote reporting queries, custom ad hoc queries, and complex queries backing MegaMax search functionality (source: personal recollection, 2026-10-15).
- Added the concept of tracking supplies and equipment through MegaMax job-cost reports, improving visibility into materials and equipment associated with work.
- Expanded Job Cost into an admin-configurable domain with React setup screens, PHP controllers, domain objects, DAOs, services, routes, database migration support, and configuration options for job-cost items and equipment.
- Delivered job-cost reporting and activity-report capabilities that gave operations and finance users visibility into job expenses, equipment usage, task costs, and related activity.
- Improved soft-surface and hard-surface measurement reports with manager filters, multi-select workflows, duplicate-measurement handling, report counts, export fixes, and billing-oriented corrections.
- Used the Job Search page as a powerful ad-hoc reporting tool by expanding filters and result detail for dates, customers, jurisdictions, work dimensions, tasks, statuses, and other operational attributes.
- Supported saved searches that back-office users could reuse as standardized operational reports rather than rebuilding the same queries manually.
- Added drill-down behavior from report counts and status results into the underlying job records, helping users move from summary information to corrective action.
- Served as the primary API designer and code reviewer for these workflows, often providing concrete code patterns to keep server, database, and UI behavior consistent.

## Utility Pole Inspection Platform

- Designed and delivered a greenfield GIS-enabled inspection and workflow platform for a new OCG business offering where no complete software platform previously existed.
- Translated real-world pole-inspection processes and customer requirements into a software workflow used by field inspectors, foremen, program auditors, and finance staff responsible for billing and reporting.
- Imported customer-provided pole data, GPS coordinates, descriptions, and dates into an ArcGIS Online data model, then generated standardized maps for pole segments and subsegments assigned to field crews.
- Imports were push-button triggered and ran without manual intervention; not scheduled, but could have been (personal recollection, 2026-10-16; confirm which imports).
- Wrote custom ETL scripts to transform client-formatted pole data into the ArcGIS database structure (personal recollection, 2026-10-19).
- Configured and deployed the field data-collection app (ArcGIS Collector) and maps through ArcGIS Online, a low-code configuration platform, rather than custom code (personal recollection, 2026-10-19).
- Designed the ArcGIS database structure, map templates, field-worker configuration, user-management setup, and APIs that exchanged inspection data and photos with ArcGIS Online.
- Integrated the inspection solution with Dcalc, a third-party engineering system (not written by David), so pole strength was calculated accurately from the measured pole dimensions and damage areas captured during inspection (wording confirmed by David, 2026-11-11).
- Implemented rules that limited equipment-damage choices based on pole location, age, and customer-provided attributes, reducing data-entry errors and speeding field lookup.
- Replaced error-prone manual photo association with offline-capable field workflows that kept photos linked to the correct pole in low-connectivity areas.
- Created reusable map templates that standardized pole imports, segment presentation, icons, and colors, reducing manual map-preparation work; later trained a foreman to independently set up new maps and arrange crew assignments in ArcGIS Online once data was imported (personal recollection, 2026-10-19).
- Built custom-code audit dashboards (not ArcGIS Dashboards; personal recollection, 2026-10-19) that flagged likely errors across approximately 50 inspection data points, enabling program managers to focus review on high-risk records.
- Improved audit quality by reducing false-positive findings from approximately 300 per 1,000 poles to fewer than 40 per 1,000 poles, with remaining issues clearly flagged for rapid correction.
- Pole-inspection billing was an automated process, custom per program and contract. Several contracts with differing pricing structures had to be maintained, and billing applied the pricing of whichever contract was in force for the particular circuit of poles (source: David's correction, 2026-11-11). Billing rules configured per customer were MegaMax, not pole inspections; do not describe pole billing as per-customer rules.
- Scaled the operation from approximately 200 poles to 1,000 poles per week, with photo-processing volumes reaching approximately 35 GB per circuit over two weeks.
- Technical environment included PHP, Laravel, JavaScript, Vue.js, React, MySQL, MariaDB, Flutter, Rust, ArcGIS Online, ArcGIS Field Maps, ArcGIS Collector, Google Maps APIs, Docker, AWS, GitHub, GitHub Copilot, GitLab, Jira, REST APIs, and Google Maps APIs.

## Stakeholder and Product Delivery

- Partnered with business, field, finance, operations, project-management, and technical stakeholders to identify system improvements and turn business needs into deliverables.
- Worked directly with every user group, including back-office staff, field users, finance analysts, internal stakeholders, and clients (personal recollection, 2026-10-15).
- On the pole-inspection program, met weekly with clients to monitor software usability and stability and identify improvements (personal recollection, 2026-10-15).
- Trained field workers both on inspection procedures and on using the inspection software the team built (personal recollection, 2026-10-15).
- Jarvis service design: rather than duplicating services for the mobile app, kept one service for each function, reused by both the back-office applications and Jarvis. This avoided maintenance headaches and kept results accurate and consistent between the apps (source: personal recollection, 2026-11-05).
- Used AI constantly to understand the legacy PHP: tracing calls and flows through the code to see how a change would affect other areas of the code and connected systems. For example, when changing services for Jarvis, used this to make sure other systems and parts of the original app were not adversely affected (source: personal recollection, 2026-11-05). This is separate from the PHP-to-React rewrite, which David has said did not use AI heavily.
- Balanced hands-on engineering decisions with team leadership, delivery planning, troubleshooting, and stakeholder communication.

## Miss Dig Integration Modernization

- Designed the migration from MegaMax's existing Miss Dig objects and workflows to a new provider model, then guided a team member who implemented the broader rewrite closely against the design.
- Modeled new provider concepts and fields while preserving MegaMax workflows for viewing ticket status, refreshing status data, and associating tickets with jobs.
- Designed for both automatic and manual ticket-to-job assignment, reducing back-office effort required to maintain ticket associations and improving the speed at which accurate job status reached field workers.
- Addressed integration reliability concerns including callback signature validation, missing-ticket handling, member-response persistence, provider-side configuration problems, legal-start-date behavior, and longer provider ticket identifiers.
- Modernized a high-touch external integration so ticket status was more accurate and timely for back-office staff and field crews, while reducing manual data-entry overhead.
- Miss Dig rewrite moved from pull to push. The old integration batched up tickets and polled for status changes. The new provider supported registered webhooks, so MegaMax was notified of each ticket status change and updated that one ticket, and the change was reflected on every job using it. This improved the design and reduced complexity. Batch ticket lookup remained, used only for initial ticket ingest and assignment; David is not certain of that scope, so confirm before claiming it (source: personal recollection, 2026-11-05).
- Miss Dig role and timing: the vendor shut off its old system, so the work had to move quickly. David wrote the initial integration with the new system, plus how-tos, documentation, and the overall architecture, then handed the rest to a junior developer, who completed it in time. The old integration polled in a nightly batch, so a daytime ticket update waited until night or needed a manual pull; webhooks gave crews status in real time (source: personal recollection, 2026-11-05).
- Miss Dig manual ticket updates fell from about 5,000 a year to about 400 one-offs after the webhook change (source: personal recollection, 2026-11-05). Not verified against data; confirm before using on a resume.

## Source Notes

- Evidence extracted from David Gordhamer resume 2.4 and related resume documents in the parent resume folder on September 3, 2026.
- Corrected OCG end date: November 13, 2025.
- Confirm whether the utility pole inspection work was a separate title, an initiative within OCG, or both.
- Add documented business metrics, customer counts, project savings, delivery time, or operational-volume measures when available.
