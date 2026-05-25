# Interpersonal Functioning and Shared Psychedelic Experiences: A Mixed Methods Investigation of Psychedelic Co-use

**Author:** Robert Hutto  
**Degree:** Master of Science in Psychological Research  
**Institution:** Brooklyn College – City University of New York  
**Year:** 2026  

---

## Project Overview

This study examined whether individuals who have used psychedelics with their current romantic partner (co-users) differ from those who have used psychedelics outside of their relationship (discordant users) across several dimensions of relationship functioning. The central question was whether the relational context of psychedelic use — specifically, whether a romantic partner was present — is associated with differences in interpersonal closeness, relationship satisfaction, commitment, investment, quality of alternatives, and sexual satisfaction.

The study used a mixed-methods design, combining quantitative group comparisons and moderation analyses with qualitative thematic analysis of open-ended survey responses. Understanding how the interpersonal context of psychedelic use shapes relational outcomes is a meaningful gap in a literature that has predominantly focused on individual-level effects.

---

## Repository Contents

| Folder / File | Contents |
|---|---|
| `data/` | See `data/README_data.md` — raw data are not included (see Data section below) |
| `code/` | R analysis scripts |
| `output/` | Figures and tables generated from analysis |
| `docs/` | Thesis PDF |
| `LICENSE` | License for reuse of code and materials |
| `CITATION.cff` | Citation file for this repository |

---

## Data

Data were collected via an anonymous Google Forms survey distributed on Reddit. Participants were English-literate adults with at least one lifetime psychedelic experience, recruited from subreddits related to psychedelic use and New York City neighborhoods near CUNY campuses. The final quantitative analysis sample comprised 118 adults currently in romantic relationships.

**Raw data are not included in this repository.** The survey collected demographic and relationship information that could potentially identify participants. Data are restricted to protect participant privacy consistent with informed consent procedures. Researchers interested in the data may contact the author directly to discuss access.

Data format: The raw data were collected in Google Forms and exported as a spreadsheet. Quantitative variables included Investment Model Scale Short Form subscales, Inclusion of Other in Self Scale (IOS) responses, sexual satisfaction, and psychedelic use history items. One open-ended item served as the qualitative data source.

---

## Code / Analysis

All quantitative analyses were conducted in **R (version 4.4.1)**.

Key packages:

- `readxl` — data import
- `tidyverse` — data wrangling
- `psych` (version 2.4.12) — descriptive statistics
- `effsize` (version 0.8.1) — Cohen's *d* effect sizes
- `interactions` (version 1.2.0) — simple slopes analysis

**`code/analysis.R`** covers the full quantitative pipeline in six steps:

1. Data loading and variable construction (renaming, recoding, subscale scoring)
2. IOS variable construction (perceived, desired, discrepancy)
3. Sample descriptives by group (Table 1)
4. Primary group comparisons via Welch's independent-samples *t*-tests
5. Moderation analyses via OLS regression (IOS discrepancy and perceived IOS as moderators, tested separately)
6. Simple slopes analyses for significant interactions

Qualitative thematic analysis followed the six-phase reflexive framework described by Braun and Clarke (2006, 2022) and was conducted independently of the quantitative pipeline. No qualitative analysis code is included because the analysis was conducted manually.

Raw data are not required to inspect the code structure; the script includes inline comments describing each analytical decision.

---

## Thesis

The full thesis document is available in `docs/`.

---

## Citation

*To be added upon Zenodo DOI generation.*

---

## Session Info

```
R version 4.4.1
Packages: readxl, tidyverse, psych 2.4.12, effsize 0.8.1, interactions 1.2.0
```
