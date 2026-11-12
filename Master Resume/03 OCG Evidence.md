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

- Designed the migration from MegaMax's existing Miss Dig objects and workflows to the provider's new platform, wrote the initial integration, the architecture, and how-to documentation, then worked closely with a team member who completed, tested, and deployed the rest against the design (source: MegaMax git history and personal recollection, 2026-11-12).
- Modeled new provider concepts and fields while preserving MegaMax workflows for viewing ticket status, refreshing status data, and associating tickets with jobs.
- Addressed integration reliability concerns including callback signature validation, missing-ticket handling, member-response persistence, provider-side configuration problems, legal-start-date behavior, and longer provider ticket identifiers.
- Modernized a high-touch external integration so ticket status was more accurate and timely for back-office staff and field crews, while reducing manual status upkeep.
- Miss Dig rewrite moved from pull to push. The old integration (2020-2021) kept a queue of open tickets and polled Miss Dig's Positive Response API for changes. The provider's new platform (Pelican POSR) supported registered, signed webhooks for ticket creation, member responses, all members responded, and legal start date. MegaMax was notified of each change, updated that one ticket, and the new status applied to every job linked to it. This improved the design and reduced complexity (source: MegaMax code and git history, verified 2026-11-12).
- Remaining batch work is a scheduled sweep for date-driven status changes the provider does not push: legal start date passed and ticket expired. Batch lookup was not used for initial ticket ingest; the 2026-11-05 recollection of that was wrong (verified in code, 2026-11-12).
- David designed and implemented automatic ticket-to-job linking, and a team member tested and submitted it (source: David, 2026-11-12): when a ticket is filed with MegaMax job IDs in its User Reference field, the ticket-created webhook links the ticket to every listed job with no manual step, and invalid IDs are logged and skipped (source: MegaMax code, verified 2026-11-12). The feature was available in production; staff mostly kept linking tickets by hand after ticket creation, which they may have found easier or which more training would likely have changed (source: David, 2026-11-12). Low use reflects user habit, not a defect. Claim the feature as built and available; do not claim it reduced linking effort, since no usage data supports that. Usage is likely undercounted: links are written with INSERT IGNORE, so when staff linked a ticket before its webhook arrived, the automatic attempt left no record. Recorded automatic links: 25 of about 63,600 from 2023 through May 2025 (source: production database snapshot of 2025-05-21, analyzed 2026-11-12).
- Timeline (git history and production data, verified 2026-11-12): polling ran August 2020 - December 2021, then Miss Dig retired its old system. David began the new integration around May 2022 and committed the initial webhook and POSR integration (more than 1,300 lines: webhook controller, signature validation, POSR inquiry service, member service, routes) on 2022-08-23, then paused it because Miss Dig's new system would not be ready for the 2022 dig season. Work resumed in April 2023 and went live in June 2023, with David fixing signature validation, member-response persistence, and a provider-side route misconfiguration against real pre-production traffic. About 6 months of development across two phases; about 13 months from start to go-live, mostly waiting on the provider. The deadline was the spring 2023 dig season, and the business pressed to be ready for it (source: David, 2026-11-12). Say the work had a hard seasonal deadline; do not claim a short build window, since most of the elapsed time was spent waiting on the provider.
- Status tracking was fully manual from January 2022 until the webhooks went live, because the old API was gone and the new platform was not ready (production snapshot of 2025-05-21: no automated revisions or member responses recorded in that period).
- Manual effort (production snapshot of 2025-05-21): back-office staff made about 13,800 manual job status updates in the April-October 2022 dig season (about 1,970 a month) and about 1,590 in April-October 2024 (about 227 a month), an 88% drop, while tickets created per year grew from 579 (2022) to 7,007 (2024), about 12 times. January-May 2025 averaged about 95 manual updates a month. This replaces the 2026-11-05 recollection of "about 5,000 a year to about 400." Compare only against the manual gap years: under the old poller (2020-2021) manual overrides were also low, so do not claim webhooks cut manual effort compared with polling. 2022 ticket volume was low because the old system had been retired.
- Volume (same snapshot): about 120,000 utility member responses processed automatically from June 2023 through May 2025 (about 5,000 a month, peaking above 11,500 in April 2025); about 88,000 automated job status changes from August 2023 through May 2025 (August 2023 includes a one-time backfill of about 21,000); about 16,000 tickets carrying about 63,600 job links in that period, about 4 jobs per ticket and up to 33.
- Status lag: the old poll interval is not recorded in the code. In production data, the old poller's last-poll times fall only between 07:00 and 18:59 and spread across every business hour, so it polled repeatedly during the business day, not in a nightly batch (production database snapshot of 2025-05-21, analyzed 2026-11-12; this corrects the 2026-11-05 recollection). A change made after hours waited until the next morning's polls. Webhooks deliver each change as it happens, at any hour. Do not claim a specific interval.
- Not measured: hours saved (about 1,750 fewer manual updates a month at season peak; confirm minutes per update with the back office before converting to hours), and safety or scheduling gains from crews seeing legal clearance sooner (reasonable inference only; do not quantify).

## Source Notes

- Evidence extracted from David Gordhamer resume 2.4 and related resume documents in the parent resume folder on September 3, 2026.
- Corrected OCG end date: November 13, 2025.
- Confirm whether the utility pole inspection work was a separate title, an initiative within OCG, or both.
- Add documented business metrics, customer counts, project savings, delivery time, or operational-volume measures when available.
