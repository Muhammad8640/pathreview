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
