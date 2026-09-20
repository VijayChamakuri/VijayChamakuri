# Vijay Chamakuri

I live in graphs, think in loops, and breathe pipelines.

I build applied-AI systems where the language model does the part it is good at and deterministic code does the part that has to be right, and data systems where every published number traces back to a test. TypeScript and Python, agents and pipelines, with evaluation and the audit trail treated as part of the product rather than as reporting.

I use AI agents as force multipliers to explore faster, automate repetitive work, and build complete systems from raw ideas to working products. Agents may accelerate the code, but I own the problem, architecture, judgment, quality, and outcome.

[LinkedIn](https://www.linkedin.com/in/vijaychamakuri/) · [Tableau Public](https://public.tableau.com/app/profile/vijay.chamakuri/vizzes)

## Featured work

| Project | What it is | What to open first | Engineering evidence |
|---|---|---|---|
| **RecruitOS** (private repository) | An agentic recruiting control plane built on one rule: the model may only extract verbatim, citation-grounded evidence from candidate documents, and deterministic code evaluates it against a locked rubric, routes uncertainty into human resolution tasks, and records every event in an append-only ledger. | Private, walkthrough on request | Ungrounded quotes are rejected rather than scored; exact rational arithmetic instead of float scores, shown as a decomposition table; five review workspaces including an audit timeline and a trust center; strict TypeScript with architecture-boundary, dynamic-code and browser-bundle gates; unit, property, integration and Playwright end-to-end suites |
| [Checkpoint](https://github.com/VijayChamakuri/checkpoint) | An integration layer that lets an agent drive a legacy back-office web application that has no API: the model discovers how to reach a goal once, and that capability is replayed deterministically afterwards with no model in the loop. | [`REPORT.md`](https://github.com/VijayChamakuri/checkpoint/blob/main/REPORT.md) | Typed, versioned, parameterized capability artifacts; deterministic replay; a real human-escalation path when replay gets stuck; TypeScript, Playwright, vitest |
| [SaaS Revenue Intelligence](https://github.com/VijayChamakuri/saas-revenue-intelligence) | A revenue analytics system that reconciles MRR, finds billing defects and scores churn risk, with every dashboard number tied back to the warehouse. | [Tableau Public](https://public.tableau.com/app/profile/vijay.chamakuri/viz/SaaSRevenueIntelligenceMRRRetentionBillingControls/Executiveoverview) | dbt/DuckDB models, a governed metric contract validated against the marts, extract-to-mart tie-out before publication, CI on two Python versions; synthetic data is labeled |
| [Medicare Claims Utilization, Payment & Quality](https://github.com/VijayChamakuri/medicare-claims-utilization-cost-quality) | CMS synthetic claims turned into a tested star schema with governed KPIs and published dashboards. | [Tableau Public](https://public.tableau.com/app/profile/vijay.chamakuri/viz/MedicareClaimsUtilizationPaymentQualityAnalyticsCMSDE-SynPUF/ExecutiveOverview) | SQL star schema with a dbt layer, blocking reconciliation that stops the build, independent recomputation in pandas, identifier guards on every export |
| [Diabetes Care Gaps & Diagnostic Equity](https://github.com/VijayChamakuri/diabetes-care-gaps-diagnostic-equity) | Survey-weighted NHANES analysis of the undiagnosed diabetes gap and of what changes when the training label changes. | [HTML dashboard](https://github.com/VijayChamakuri/diabetes-care-gaps-diagnostic-equity/blob/main/dashboard/screenshots/01_care_gap_overview.png) | SQL cohort construction, Python and R cross-checks, pre-specified comparison, limitations stated in the first screen |

## How I build

My work sits at the intersection of agentic software, data engineering, analytics, and applied machine learning. I enjoy turning ambiguous problems into reliable pipelines, intelligent workflows, useful interfaces, and systems that people can trust.

My work emphasizes traceable metrics, honest treatment of synthetic data, time-aware evaluation, and documentation that lets another analyst reproduce the result.

My portfolio separates measured, public, simulated, and synthetic data; defines metrics before visualization; and ties reported numbers back to tested analytical outputs.

## Where this work applies

Master's in data science, Indiana University. The same standards travel across the roles this portfolio speaks to:

- **Data Analyst:** SQL analysis, reproducible Python/R workflows, validation, and decision-focused reporting.
- **Healthcare Analyst:** claims utilization and care-gap analysis with clear definitions, privacy boundaries, and domain limitations.
- **BI Analyst:** governed KPIs, dimensional models, reconciliation, Tableau dashboards, and Excel review artifacts.
- **Business Analyst:** business questions translated into documented metrics, stakeholder-ready outputs, acceptance checks, and decision logs.
- **Applied AI and software engineering:** agent architectures with deterministic boundaries, evaluation harnesses, typed interfaces, human-in-the-loop escalation, and tests that run in CI.

## Additional projects

| Project | What it demonstrates | Evidence available in the repository |
|---|---|---|
| [SaaS Revenue Intelligence: MRR, Churn & Billing Leakage](https://github.com/VijayChamakuri/saas-revenue-intelligence) | Revenue analytics, finance reconciliation, churn modeling, forecasting, dbt, DuckDB, Spark, R, and Airflow | Locked Python environment, active CI, automated tests, dbt tests, architecture and metric documentation, and source-backed result visuals |
| [PFAS Toxicogenomics K-Spaces](https://github.com/VijayChamakuri/pfas-toxicogenomics-kspaces) | Reproducible bioinformatics, consensus modeling, stability analysis, ontology-backed interpretation, and research software guardrails | Executed analysis notebook, 45 local tests across the analysis and integrated system, CI, data provenance, checksums, citation metadata, and documented scientific limitations |
| [Emergency SOS Reliability Intelligence](https://github.com/VijayChamakuri/emergency-sos-anomaly-detection-rca) | Temporal anomaly detection, leakage-aware evaluation, root-cause analysis, and simulated intervention measurement | Deterministic synthetic data, chronological holdout, five automated tests, model card, architecture notes, and a generated executive dashboard |
| [Cloud Asset Discovery Pipeline](https://github.com/VijayChamakuri/cloud-asset-discovery-pipeline) | Spark data engineering, PII governance, data-quality gates, graph clustering, dbt, DuckDB, and event-driven notification | Sample and full-scale paths, unit tests, independent result verification, architecture documentation, and source-generated charts |
| [CreatorPulse](https://github.com/VijayChamakuri/creator-pulse) | Automated reporting, public-data ingestion, optional LLM narrative and QA, static dashboards, and scheduled delivery | Live GitHub Pages output, explicit real versus synthetic provenance, deterministic offline mode, automated tests, and a weekly workflow |
| [Remittance Fraud Analytics](https://github.com/VijayChamakuri/remittance-fraud-analytics) | Imbalanced classification, chronological evaluation, entity and velocity features, root-cause analysis, and experiment design | Reproducible synthetic benchmark, automated leakage and provenance checks, documented limitations, static dashboard, and a real ULB-compatible input path |

## Technical focus

- Analytics engineering: SQL, dbt, DuckDB, data modeling, metric governance, and reconciliation
- Data science: Python, R, statistical modeling, causal inference, forecasting, experimentation, and applied machine learning
- Data platforms: Spark, Airflow, AWS analytics services, PostgreSQL, and reproducible local pipelines
- Decision support: Power BI, Tableau, executive reporting, data storytelling, and operational dashboards

## How I work

- Separate measured, public, simulated, and synthetic data clearly.
- Prefer chronological evaluation and leakage checks when deployment happens over time.
- Keep analytical claims proportional to the design and available evidence.
- Treat tests, provenance, limitations, and reproducibility as part of the deliverable.

## Connect
 [LinkedIn](https://www.linkedin.com/in/vijaychamakuri/)

Last portfolio review: September 2026
