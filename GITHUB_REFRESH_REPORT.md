# GitHub refresh, September 2026

A recruiter-facing pass over the account: profile text, repository metadata and additive README blocks, so that the three analyst flagships lead and every repository says what it is. Nothing was deleted. No repository, branch, file, history, workflow, README section or existing claim was removed, no repository was renamed, archived or made private, and no license was added.

## Profile

| Field | Before | After |
|---|---|---|
| Bio | Analytics Engineering, Applied ML, and Reproducible Data Science | Applied AI & Data Engineering \| Agentic systems, LLM evaluation, analytics pipelines \| Python, TypeScript, SQL |
| Website | empty | Tableau Public profile |
| Available for hire | not set | yes |
| Location | Indiana | Indiana (unchanged) |

`README.md` opens with the engineering framing, then a featured table of five projects: RecruitOS and Checkpoint for agentic and applied-AI work, and the three analytics flagships with their published dashboards. Each row says what the project is, what to open first, and the engineering evidence behind it. `How I build` and `Where this work applies` carry the earlier paragraphs and the role bullets, with a line added for applied AI and software engineering. The previous featured table is kept in full under `Additional projects`, and the honesty and reproducibility principles are unchanged.

RecruitOS is a private repository and is named without a link. Its GitHub description was changed from a placeholder to what it actually does. Nothing private was published.

## Repository changes

| Repository | Commit | Change |
|---|---|---|
| `saas-revenue-intelligence` | `6567833` | Tableau Public link and its Executive overview screenshot now lead the README, above the offline HTML dashboard, which is kept with its own screenshot and instructions. Homepage set to the workbook. Topics: `tableau`, `excel`, `mrr`, `retention-analytics`, `revenue-operations`. |
| `medicare-claims-utilization-cost-quality` | `7e65e9b` | Added an `Open first` row: Tableau Public, executive summary PDF, metric dictionary, data limitations. Homepage set to the workbook. Topics: `tableau`, `excel`, `dbt`, `business-intelligence`, `claims-analytics`. |
| `diabetes-care-gaps-diagnostic-equity` | `1ccdde1` | Added an `Open first` row: HTML dashboard screenshot, quality brief, Excel quality review, methods, limitations. Topics: `data-analytics`, `healthcare-data`, `biostatistics`, `data-visualization`. No Tableau claim and no homepage, because no workbook exists. |
| `crm-pipeline-analysis` | `0abc95c` | Synthetic-data line and a `Key outputs` row under the title. Dated note in the Tableau section pointing at the two workbooks that now exist elsewhere; this repository still has none and the original paragraph is kept. Description and eight topics added. |
| `Satellite-Message-Delivery-QoE-Pipeline` | `066a133` | Synthetic-data line before the metrics, and a `What runs where` paragraph separating the local end-to-end pipeline from the BigQuery, Lambda and Looker Studio deployment guides, which are not hosted services. Description and seven topics added. |
| `elastic-revenue-forecast` | `45acbf8` | One line under the title with the investor-relations source and a statement that this is not investment advice. Description and six topics added. |
| `Exploring-Space-Missions` | `9451868` | README was a title only. Added an Overview with the dataset, method, how to run it, outputs and limitations, including that the forecast has no held-out evaluation and that the loader uses an absolute Codespaces path. Description and six topics added. |
| `VSCOpenAI-to-Z-ChallengeSubmission` | `a60a2d5` | No README on the default branch. Added one: question, data, the two-stage pipeline, the negative result, how to run it, and the limits of one unvalidated vision-model judgment per site. Labeled a competition submission, not validated research. Seven topics added. |
| `ADT` | `3aa75e0` | No README on the default branch. Added one naming each notebook, crediting the open course materials the two labs follow, and noting the homework notebook reads an uncommitted local CSV by absolute path. Labeled coursework, not a portfolio project. Description and five topics added. |
| `pfas-toxicogenomics-kspaces` | `ddbf039` | One-line summary of the method under the title. Topics `data-analysis`, `statistical-analysis` added. |
| `checkpoint`, `usaspending-sat-bunching`, `snap-retailer-did-analysis`, `walmart-markdown-analysis`, `creator-pulse`, `maintenance-equipment-pipeline` | metadata only | Topics added, and a description for `maintenance-equipment-pipeline`. No file changed. |
| `cloud-asset-discovery-pipeline`, `emergency-sos-anomaly-detection-rca`, `remittance-fraud-analytics`, `hub-delay-audit` | none | Already had a description and topics. Left as they are, including the GitHub Pages homepage on `remittance-fraud-analytics`. |

All 21 public repositories now have a description. Approved values are recorded in [`PORTFOLIO_METADATA.md`](PORTFOLIO_METADATA.md).

## Checks run

- Both Tableau Public workbook URLs were opened and rendered the named workbook on its Executive overview page. The Tableau Public profile was opened and lists exactly two vizzes.
- The SaaS Tableau screenshot used as the lead image was compared with the live workbook and matches it.
- Every relative link added or reordered in a README resolves to a file that exists in that repository.
- `saas-revenue-intelligence`: full test suite, ruff and mypy pass; CI green on Python 3.11 and 3.12.
- `medicare-claims-utilization-cost-quality`: full test suite, ruff and mypy pass; CI green on Python 3.11 and 3.12.
- `diabetes-care-gaps-diagnostic-equity`: the README drift check passes, and figures the check regenerated with identical content were left untouched so the commit is README-only.
- No added line contains an em dash.
- `git diff --name-status` shows no `D` entries in any clone, and no file count decreased in any repository.

## Still to do by hand

1. **Pins.** GitHub exposes no API for pinning, so the six pins must be set from the profile page: `Customize your pins`, then choose, in this order, `checkpoint`, `saas-revenue-intelligence`, `medicare-claims-utilization-cost-quality`, `cloud-asset-discovery-pipeline`, `diabetes-care-gaps-diagnostic-equity`, `creator-pulse`. Pinning only changes what is shown; the previous pins stay on the account.
2. **Social previews.** Three 1280x640 images were produced for the flagships, each using that project's own chart with the project title, a role label, the name, and a data-provenance label. None of the three repositories has a custom preview today, so nothing would be overwritten. They are set per repository under `Settings > General > Social preview > Upload an image`.

## Claims that were rejected for lack of evidence

- **A Tableau workbook for `diabetes-care-gaps-diagnostic-equity`.** The local clone has no `.twb` or `.twbx`, and the Tableau Public profile lists two vizzes, neither of them this project. The README's statement that no Tableau or Power BI workbook exists was left exactly as written, the `tableau` topic was not added, and no homepage was set.
- **A hosted endpoint or dashboard for `Satellite-Message-Delivery-QoE-Pipeline`.** The repository ships deployment scripts and guides, not a running service, so the README now says so rather than implying a live endpoint.
- **Any metric, test count or dataset volume in the profile table.** The featured table names artifacts and evidence types only, so it cannot drift when a pipeline is rerun.

## Noted, not changed

- Eleven repositories carry no license file: `ADT`, `checkpoint`, `emergency-sos-anomaly-detection-rca`, `Exploring-Space-Missions`, `hub-delay-audit`, `Satellite-Message-Delivery-QoE-Pipeline`, `snap-retailer-did-analysis`, `usaspending-sat-bunching`, `VijayChamakuri`, `VSCOpenAI-to-Z-ChallengeSubmission`, `walmart-markdown-analysis`. A license grants rights, so none was added.
- `medicare-claims-utilization-cost-quality` tracks a Tableau recovery file, `tableau/workbook/.~medicare_claims_bi__49802.twbr`, committed by accident earlier. It was left in place rather than deleted.
- The profile README lists `SaaS Revenue Intelligence` twice, once in the new featured table and once in the preserved older table, because the older table was kept whole.

Last portfolio review: September 2026
