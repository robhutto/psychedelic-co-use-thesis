Code / Analysis
All quantitative analyses were conducted in R (version 4.4.1).
Key packages:

readxl — data import
tidyverse — data wrangling
psych (version 2.4.12) — descriptive statistics
effsize (version 0.8.1) — Cohen's d effect sizes
interactions (version 1.2.0) — simple slopes analysis

code/analysis.R covers the full quantitative pipeline in six steps:

Data loading and variable construction (renaming, recoding, subscale scoring)
IOS variable construction (perceived, desired, discrepancy)
Sample descriptives by group (Table 1)
Primary group comparisons via Welch's independent-samples t-tests
Moderation analyses via OLS regression (IOS discrepancy and perceived IOS as moderators, tested separately)
Simple slopes analyses for significant interactions

Qualitative thematic analysis followed the six-phase reflexive framework described by Braun and Clarke (2006, 2022) and was conducted independently of the quantitative pipeline. No qualitative analysis code is included because the analysis was conducted manually.
Raw data are not required to inspect the code structure; the script includes inline comments describing each analytical decision.
