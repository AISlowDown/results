# Comparison directions and statistical method selection

Use this reference to plan or review comparisons in experimental-data and table interpretation.
The directions below are an editorial synthesis, not an official taxonomy. NIST provides statistical
methods and their assumptions; ASA provides principles for interpreting p-values. Neither prescribes
one universal Results narrative. Keep the main skill's purpose, findings, and small-conclusion flow.

## Select the comparison that answers the question

| Direction | Analytical question | Evidence and interpretation focus |
|---|---|---|
| Level and magnitude | Which outcomes differ, and by how much? | Compatible metrics, baseline, absolute difference or ratio, supported uncertainty. |
| Trend and incremental gain | How does the outcome change with time, dose, or a parameter? | Direction, interval-specific changes, plateaus and reversals; account for unequal spacing when comparing rates. |
| Variation and consistency | How dispersed or consistent are outcomes? | Distributions, SD/IQR or appropriate variability measures; distinguish observation spread from uncertainty in an estimate. |
| Subgroups and conditions | Does the overall pattern hold across groups? | Comparable strata, group sizes, direction and magnitude, important exceptions. |
| Interaction | Does one factor's effect depend on another factor? | A direct contrast of effects or an appropriate interaction model, supported factor combinations. |
| Components | Where in the measured components does the aggregate difference appear? | Compatible populations, decomposition definitions, denominators and weights; no invented mechanism. |
| Sensitivity | Does the conclusion change under alternative analysis settings? | Explicit tested settings, shifts in magnitudes/rankings; not automatically external validity. |
| Tradeoffs and constraints | Which option meets the specified goals and limits? | Joint performance and resource metrics, explicit decision criteria; no universal best option inferred from one metric. |
| Exceptions and failures | Which cases depart from the main pattern? | Source-verified outliers, failures, or reversals; avoid selective deletion or causal stories without evidence. |

For multiple figures/tables, use their roles to form a substantive sequence, such as overall pattern
to subgroup comparison or main finding to sensitivity analysis. Describe each source before combining
its contribution into a small conclusion. A follow-up figure need not explain a causal mechanism.

## Design and data determine the method

Establish what is estimated, the independent unit, sampling/assignment, outcome type, and dependence
structure before selecting a test. The candidates below are not automatic prescriptions.

| Question/design | Candidate approach | Checks before use |
|---|---|---|
| Difference between two independent means | Mean difference and interval, with a suitable two-sample method such as Welch's t-test when justified | Independent units, distribution/sample-size conditions, unequal variances and estimand. |
| Two measurements on the same units | Within-unit differences, paired confidence interval or suitable paired test | Actual one-to-one pairing, independent pairs, assumptions about the differences. |
| Several groups | Design-appropriate ANOVA or another suitable model, planned contrasts or multiplicity-aware follow-up comparisons | Independent versus repeated/clustered design, residual assumptions, comparison family. |
| Multiple experimental factors | Factorial analysis or regression with relevant interaction terms | Supported combinations, replication, confounding, model assumptions and outcome type. |
| Continuous trends or associations | Graphical exploration and an appropriate correlation/regression model | Nonlinearity, influential values, repeated observations, temporal dependence and confounders. |
| Proportions, counts, classification metrics or ranks | Outcome-specific model/test or design-respecting resampling when justified | Denominators, paired predictions, clustering, bounded/nonlinear metrics; do not apply a mean test mechanically. |

A model's single aggregate F1 or accuracy does not supply the independent repetitions needed for a
standard t-test. Shared test observations imply paired predictions, but not that every aggregate
metric should be analyzed with a paired t-test. Match inference to the metric and experimental unit.
Do not reconstruct raw observations from summary means. Compute uncertainty from summaries only
when the required sample sizes, dispersion/covariance information, and assumptions are available.

When ordinary assumptions do not fit, assess an appropriate alternative rather than selecting a
nonparametric test by label. Resampling must also respect pairing, clustering, and repeated measures.

## Interpretation checks

- Quantify the central difference and its supported uncertainty, then explain its relevance to the
  research question. Statistical significance alone does not establish a useful improvement.
- One subgroup being significant while another is not does not establish a difference between
  subgroup effects. Evaluate the difference directly when inferential support is required.
- Overlapping or non-overlapping separate group intervals are not a substitute for the appropriate
  interval or test for the contrast of interest.
- A nonsignificant result is not proof of equivalence. Equivalence claims require an appropriate
  design/analysis and justified margins, not margins chosen to fit the observed result.
- When making multiple inferential comparisons, define the comparison family and use an appropriate
  method where needed. Tukey and Bonferroni address particular comparison settings, not every problem.
- Distinguish prespecified analyses from exploratory follow-ups. Do not search for favorable
  significance and present the selected result as a prespecified test.
- Descriptive association supports an association statement. Causal interpretation requires an
  appropriate design and assumptions. State consequential boundaries once where they affect meaning.
- Keep data-derived selection separate from independent evaluation. Do not tune a model or threshold
  on a final test set and describe that same set as untouched validation of the selected approach.

## Authoritative references

These links support the methodological principles; consult the relevant page rather than importing
all methods into every task. Preserve existing manuscript citations; do not automatically insert
these references into the user's prose.

- [NIST: Exploratory Data Analysis](https://www.itl.nist.gov/div898/handbook/eda/section1/eda11.htm): discovering structure, anomalies, and assumptions.
- [NIST: Product and Process Comparisons](https://itl.nist.gov/div898/handbook/prc/prc_d.htm): comparison methods and confidence intervals.
- [NIST: Analysis of paired observations](https://www.itl.nist.gov/div898/handbook/prc/section3/prc311.htm): naturally paired measurements and analysis of differences.
- [NIST: Confidence intervals for differences between means](https://www.itl.nist.gov/div898/handbook/prc/section3/prc312.htm): design-specific interval construction.
- [NIST: Interaction Effects](https://www.itl.nist.gov/div898/handbook/pri/section6/pri623.htm): examination of interactions in factorial experiments.
- [NIST: Tukey's method](https://www.itl.nist.gov/div898/handbook/prc/section4/prc461.htm): simultaneous pairwise comparisons under its assumptions.
- [NIST: Bonferroni's method](https://www.itl.nist.gov/div898/handbook/prc/section4/prc473.htm): multiplicity adjustment for a defined family.
- [ASA: Statement on Statistical Significance and P-Values](https://www.amstat.org/asa/files/pdfs/p-valuestatement.pdf): p-values, effect size, context, and transparent reporting.
