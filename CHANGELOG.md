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
- (new chapters land here as they're written)

### Replaced
- (dataset/case-study swaps land here as they're made, chapter by chapter — see `PART2_PLAN_DIARY.md` for the concrete, file-scoped migration plan: package-source switch to `behdslabs`, then `mnist_27`/`mnist_127`, `tissue_gene_expression`, `movielens`, `pr_death_counts`, `olive`, `stars`, and the 2012/2016 election datasets, each mapped to their `behdslabs` behavioural equivalents)
