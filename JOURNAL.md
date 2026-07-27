\# PathReview Contribution Journal



\## Week 7 — Issue Selection



\*\*Name:\*\* Muhammad Raza



\*\*GitHub Username:\*\* Muhammad8640



\*\*Issue Link:\*\* https://github.com/ascherj/pathreview/issues/50



\*\*Issue Title:\*\* Add a `has\_tests` boolean to the repo analysis output



\*\*Tier:\*\* ☑ Tier 1 ☐ Tier 2 ☐ Tier 3



\### Problem Summary



The repository analysis currently does not indicate whether a GitHub repository contains automated tests. This issue requires adding a new boolean field called `has\_tests` to the analysis output. The value should be `true` when the repository contains common testing indicators such as a `tests/` or `test/` directory, a `pytest.ini` file, or Python test files matching the `test\_\*.py` naming convention. A successful implementation will allow users to quickly determine whether a repository includes automated tests.



\### "Is this the right issue for me?" Reasoning



I selected this issue because it is labeled as a Tier 1 issue and a good first issue. The scope is well defined, the expected behavior is clearly described, and the issue identifies the primary files that will likely need modification. It appears to be a manageable feature to implement while helping me become familiar with the PathReview codebase.



\*\*Branch Name:\*\* `feat/50-add-has-tests`



**Setup Confirmation:** ☑ App runs locally at `http://localhost:5173`


**Cohort Ledger:** ☑ Issue added to the cohort issue ledger



## Week 8 — Reproduction & solution planning

**Reproduction commit link: https://github.com/Muhammad8640/pathreview/commit/ca18d9c**

**Reproduction summary:**

Inspected the current implementation of `agent/tools/github_tool.py` and `ingestion/parsers/repo_analyzer.py`. Confirmed that `RepoAnalyzer` already supports detecting whether a repository contains tests and includes a `has_tests` field, but `GitHubTool` does not expose this field or gather the repository file structure needed to determine it. This reproduces the missing functionality described in Issue #50.

**PLAN.md link:https://github.com/Muhammad8640/pathreview/blob/feat/50-add-has-tests/PLAN.md**

**Walkthrough video (recommended):**

Not recorded.

**Blockers or open questions:**

Need to determine the best way for `GitHubTool` to retrieve the repository file structure so `has_tests` can be detected without negatively affecting performance.