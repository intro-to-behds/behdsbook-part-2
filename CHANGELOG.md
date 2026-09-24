# Changelog

All notable changes from the upstream Irizarry *Introduction to Data Science*
(`rafalab/dsbook-part-2`) are documented here, as required by the
[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0) license
under which this adaptation is distributed.

## [Unreleased] — Behavioural Data Science adaptation

### Changed
- Retitled to "Introduction to Behavioural Data Science".
- Split `index.qmd` preface/acknowledgments into separate, clearly labeled sections for the adaptation vs. the original Irizarry edition, and added a **Disclaimers** section (reflavoured datasets are adaptations of real data with fictional behavioural framing, not to be cited as genuine behavioural/statistical/predictive-modeling data; notes LLM assistance in the adaptation), matching `behdsbook-part-1/index.qmd`'s pattern.
- Updated self-referential GitHub/site links (`_quarto.yml`, `index.qmd`, `intro.qmd`) from the upstream `rafalab/dsbook-part-2` repo to this fork, `intro-to-behds/behdsbook-part-2`; `index.qmd`'s cross-link to Part 1 now points to the `intro-to-behds`-hosted site instead of the original edition.
- `intro.qmd`: package reference "All datasets used in the book are available in the **dslabs** package" → "**behdslabs**".
- Enabled a PDF download button in the book navbar (`book: downloads: [pdf]`).

### Added
- **New part, `behav/` — "Behavioural Measurement"** — original material with no equivalent in the upstream book, placed first in the chapter list (immediately after `intro.qmd`) because it is course Week 4 and precedes every other Part 2 topic. Three new files:
  - `behav/intro-behav.qmd` — part introduction.
  - `behav/measurement.qmd` — **"Measurement in Psychology"**, an original chapter by Giorgio Arcara covering constructs vs. proxies, Stevens' (1946) scales of measurement, Suppes & Zinnes' (1963) homomorphism definition, Classical Test Theory, the interval-scale assumption in Likert data, reaction time and signal detection theory as measurement problems, the five sources of validity evidence (AERA/APA/NCME, 2014), the four kinds of reliability, and attenuation/disattenuation. Adapted and translated from the author's Italian psychometrics book *Oltre i punteggi*, with all examples re-anchored from clinical neuropsychology to human–technology research. This file previously contained an unregistered verbatim copy of `inference/bootstrap.qmd`, now replaced.
  - `behav/simulating-measurement.qmd` — **"Behind the Simulations"**, a companion chapter documenting the generative models behind the simulated data used in the measurement chapter.
- The two chapters above depend on `behdslabs` ≥ 0.10.0, which adds the `simulate_likert()` and `simulate_sdt()` functions written for them.
- Two further original chapters in the `behav/` part, which now also hosts the course's Week 7 and Week 10 custom content:
  - `behav/research-ethics.qmd` — **"Research Ethics and Data Privacy"**, an original chapter by C. Costa (with G. Arcara) covering ethical principles in research with human participants, ethics review and informed consent in technology-based studies, vulnerable participants, deception and debriefing, personal and sensitive data, anonymisation vs. pseudonymisation, GDPR principles across the data life cycle, open science and data sharing, scientific integrity, bias and fairness in analysis, and the use of AI and external tools.
  - `behav/experimental-designs.qmd` — **"Experimental Designs in Psychology"**, an original chapter by C. Costa (with G. Arcara) covering operationalisation and units of analysis, association vs. causality and confounding, validity of designs, cross-sectional/longitudinal/intensive longitudinal designs, experimental control, random assignment vs. random sampling, between- and within-subjects designs, trials and stimuli in cognitive experiments, factorial and mixed designs, bias and control procedures, and planning before data collection.

### Replaced
- (dataset/case-study swaps land here as they're made, chapter by chapter — see `PART2_PLAN_DIARY.md` for the concrete, file-scoped migration plan: package-source switch to `behdslabs`, then `mnist_27`/`mnist_127`, `tissue_gene_expression`, `movielens`, `pr_death_counts`, `olive`, `stars`, and the 2012/2016 election datasets, each mapped to their `behdslabs` behavioural equivalents)
