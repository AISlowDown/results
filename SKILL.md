---
name: results
description: >-
  Result Explainer：分析实验数据、图表与论文结果。
  Use automatically when analyzing or interpreting experimental data, result tables, figures, or
  research comparisons, even without an explicit skill request or an existing manuscript. Also use
  for drafting, revising, or reviewing academic Results and related Discussion in Chinese or English.
  Organize interpretation as analytical purpose, evidence-grounded findings, and a brief conclusion,
  linking multiple figures or tables through a shared question. Select comparisons and statistical
  methods according to the research question and data design. Decide which evidence belongs in
  the main Results and which detailed support belongs in the supplement. Apply be-human-and-less-defense
  from the first generated prose. Use appropriate data tools for calculations; not for executing
  experiments or formatting alone.
---

# Result Explainer

## User manuscript style

- For this user's newly authored or revised academic prose, do not use first-person plural `We/we`, `our`, `ours` or `ourselves`. Name the study, model, analysis or research object as the subject, or use appropriate passive voice. Vary the subject rather than repeatedly opening with `This study`.
- In paper and thesis titles, headings, abstracts, body text, captions and supplementary prose, use statements or descriptive noun phrases instead of interrogative or rhetorical questions. Express a research question as a specific objective, unresolved relationship or evidence gap without presuming its answer. Descriptive titles need not assert a result.
- Keep editing labels such as `疑问句转陈述句` out of the finished manuscript. Deliver the revised wording directly; put any requested explanation outside the manuscript.
- Before delivery, check the authored prose for whole-word first-person forms and question-form sentences or headings, including `?` and `？`. Preserve verbatim quotations, reviewer comments, verified reference or official titles, code, mathematical notation and formal names such as `Weibull`. Internal planning questions and necessary questions to the user remain available. Apply these conventions over conflicting generic voice advice in imported references or templates.

User-facing names: Result Explainer / 看图说话大师. Stable invocation identifier: `results` (`$results`).

## Scope and Delivery

Select this skill automatically for substantive analysis or interpretation of experimental data, research tables, figures, and manuscript Results, even without an explicit skill invocation, a manuscript, or a request to rewrite. Requests such as "分析这些实验数据", "解释这个表格", "比较这些结果", and "根据图表写结果" activate this workflow when they concern research findings. Match the response to the request: answer a focused question directly, discuss an outline when structure is at issue, and draft only when text is requested. In discussion-only mode, use the Writer role to formulate the explanation and the Reviewer role to check it; do not force a manuscript draft or a visible multi-stage review. Discussion does not authorize file edits. Follow the user's explicit "write it in" or equivalent instruction before saving approved text.

Support Results only, Discussion only, separate sections, or a combined Results and Discussion section. Preserve the journal's required structure and the user's chosen scientific scope. Do not add experiments, redesign methods, or invent new section hierarchies simply to improve prose.

For whole-manuscript polishing, use one top-level chapter (or paper section) as the review and editing unit, retaining numerical and citation anchors. Group proposed changes by subsection in one chapter-level itemized Chinese review table; a long table may be displayed in parts, but complete the chapter's proposals before asking for row-level or whole-table decisions or writing changes. A request limited to one subsection keeps that narrower scope. When generating new analysis rather than revising source prose, provide a bounded Chinese candidate directly. Sync approved meaning to English only when requested. An explicit request to edit directly or waive the review stage overrides this default. Distinguish proposed wording from text actually inserted and saved.

## Automatic Pairing During Generation

Before composing a new explanation, analytical narrative, or Results/Discussion draft, read and
apply [be-human-and-less-defense](../be-human-and-less-defense/SKILL.md), unless it has already been
read in the current context. Apply its evidence-calibrated language, direct scope statements,
punctuation, and sentence-variety rules from the first draft. When the task is instead to polish
existing Results/Discussion wording, follow that skill's itemized review-table stage before changing
or writing back the text, unless the user explicitly requests direct editing. No separate skill
invocation is needed. If the companion is unavailable, use the embedded direct-prose rules below
and report the missing companion briefly outside manuscript prose.

Use this skill to organize the scientific interpretation and the companion to guide its expression.
For raw-data calculations, statistical tests, or spreadsheet operations, use appropriate analytical
tools or skills and inspect actual outputs before making claims. This pairing does not run experiments
or authorize additional analyses beyond the user's task. Do not force an essay or a change report for
simple numerical questions; match the requested output while applying these principles to any prose.

## Establish the Evidence Before Writing

1. Identify the exact supplied dataset, table, or figure and the analytical question. When a manuscript is involved, identify its current version and requested subsection. Inspect the associated figures, all relevant subfigures, tables, captions, and underlying numerical output where available. Do not infer map patterns from a caption or filename.
2. Match the analysis population, model, parameters, denominator, and data version. Approved methods text does not establish that the corresponding experiment has been run. Do not silently combine old results with new imputation, samples, weights, or models.
3. Map each proposed finding to its supporting figure/table/output. A lightweight working record is enough: finding, source location, population/setting, number/unit, and interpretation boundary. Show this record only when useful or requested.
4. If evidence is missing, describe only what is supported and identify the gap outside the manuscript candidate. Never fill in plausible values, spatial clusters, mechanisms, uncertainty intervals, or literature findings. Old results may be translated for review if explicitly labeled as old outside the candidate; they are not a finalized new-results section.

### Section purpose, metric meaning, and figure emphasis

For a multi-section Results review, first identify the main question, each subsection's distinct
comparison, and the evidence needed for its answer. Keep this map lightweight and internal unless the
user requests an outline or audit. Organize around supported differences and exceptions; a new spatial
analysis, temporal breakdown, or model is not an automatic remedy for a comment asking for "depth".

Read [Purpose, metrics, emphasis, and cases](references/purpose-metrics-emphasis.md) when comments
identify unclear section aims, unexplained scores, arbitrary bold labels, isolated examples, or a
conclusion not established in Results. It covers framework–method–result alignment, compatible
comparisons, figure–prose emphasis, case transitions, and policy-text interpretation. Apply only the
parts relevant to the task; do not impose the CDW example's categories or section count elsewhere.

When figure editing is authorized, every highlighted label or mark should support a specific
comparison in the prose. A maximum is not automatically the analytical focus. When only prose review
is requested, propose the corresponding visual change without silently redrawing the figure.

### Explain what a change changes in the scientific judgment

After a central numerical comparison, explain its consequence for the subsection's actual question.
Distinguish score magnitude, ordering, threshold-based classification, and frequency or interval
under sampled settings; a change in one does not establish a change in the others. Identify the
reference and denominator, then state the supported mechanism and the specific judgment or action
that follows. Changing model settings is not an observed improvement through time, and rank movement
does not measure a physical resource gain. If the evidence supports only an association or an
unresolved mechanism, keep that status. Do not add a generic significance sentence or invent a cause
to satisfy a request for deeper interpretation. Read the worked change-interpretation guidance in
[Purpose, metrics, emphasis, and cases](references/purpose-metrics-emphasis.md#interpret-score-ordering-and-classification-changes)
when a draft lists changes without explaining their meaning.

### Describe the Research Object Rather Than Its Coding State

In policy or document analysis, express Results in terms of the provisions, actions, or relationships being studied. Keep coding rules and processing states in Methods unless they are themselves the research finding. For example, replace `尚未编码到源头减量规定` with a supported, corpus-scoped statement such as `起步期样本尚无明确的源头减量规定`. A zero code alone does not establish absence beyond the sampled, accessible text. Retain coding terminology when evaluating coding performance or explaining a result that depends on the coding procedure.

For the worked policy example and its scope checks, see [Policy Results in Domain Language](references/policy-results-domain-language.md) when revising policy-analysis Results.

## Choose Comparisons Before Composing Results

Use the sequence `research question -> comparison target and independent unit -> relevant comparison
 directions -> design-compatible analysis -> purpose, findings, small conclusion`. The prose structure
is a writing convention, not an official statistical method or a requirement to run every test.

Before interpreting experimental data or tables, identify the outcome, comparator, population,
independent experimental/sampling unit, and whether observations are independent, paired, repeated,
or clustered. Distinguish raw observations, aggregate summaries, and model estimates. Do not treat
clips from one recording, repeated measurements of one object, or overlapping validation folds as
independent field replications. If the structure is unknown, use supported descriptive comparisons
and identify what is needed before inferential claims.

Select only directions that answer the actual question and have evidence: level and difference size,
trend and incremental gain, variation, subgroup differences, interactions, component breakdown,
sensitivity, performance-resource tradeoffs, and exceptions. These are a menu, not a checklist to
complete for every table. Identify important exceptions as well as improvements; do not select
comparisons solely because they produce favorable or significant results.

Read [Comparison directions and statistical method selection](references/comparison-methods.md)
when choosing comparisons, proposing a statistical method, or assessing inferential claims. Use its
NIST and ASA sources for methodological grounding, not as a universal Results template. Verify the
relevant source and method assumptions when making a technical recommendation or implementing a test.

For each central comparison, distinguish **effect magnitude**, **uncertainty**, and **practical
meaning**. Report uncertainty only when supported by the design and available output. A p-value does
not measure effect size or practical importance; absence of significance does not establish equality.
Keep percentage-point differences distinct from relative percentage changes, with the baseline clear.
Use stated application constraints rather than inventing thresholds for an optimal or adequate result.

Respect the requested scope: interpreting an existing table does not require adding new hypothesis
tests. When calculations or tests are requested, use appropriate tools, check assumptions and actual
outputs, and label exploratory analyses honestly. Never infer p-values, intervals, causality, or
population-level validity from a descriptive plot or a single aggregate score.

## Decide What Belongs in the Main Results and Supplement

During Results review or drafting, identify which findings carry the paper's central answer and
which material provides completeness, verification, or secondary detail. Read
[Main-text and Supplement triage](references/main-vs-supplement.md) when a Results section is
crowded, multiple figures/tables compete for space, or the user asks what to relocate.

First ask whether an item directly answers the experiment's stated purpose or supplies evidence
needed to judge that answer. Keep the corresponding finding and its decisive comparison in the main
Results, including the magnitude, supported uncertainty, and material exceptions. A figure or table
belongs in the main text when readers need to inspect it to assess a central claim. Treat calculation
stages, intermediate variables or indices, full underlying rows, parameter grids, diagnostics, and
secondary examples as candidates for Supplementary material when the main conclusion remains
assessable without their full detail. Keep a key intermediate contrast in the main text if it is the
only evidence separating competing explanations or establishing a central result. Neither statistical
significance nor visual complexity alone determines placement.

A move is valid only when the main text remains understandable and evidence-backed: retain a compact
result statement, a specific Supplementary Figure/Table reference, and any exception that changes
the conclusion. The supplement must preserve definitions, units, populations, model/version,
concise titles and calculation context, with explanatory material in the supplement body immediately after the relevant figure/table citation rather than in appended captions or table notes. Do not treat an unwritten or unverified supplement
as an existing destination, and do not move a finding merely because it is inconvenient for the
argument. Check the target journal's current supplement rules when preparing an actual submission.

For an existing manuscript review, return a small `retain in main / condense in main / move to
supplement / delete as repetition` map with source locations and reasons before substantial cuts.
A direct request to implement authorizes the scoped placement work; the map is for traceability.
When that work also polishes existing prose, complete the companion skill's chapter-level proposed-change
table before writing unless the user explicitly waives that review stage. When editing both files,
update captions and cross-references, then reopen
and verify each saved artifact and the main-to-supplement pointers. If only a candidate is requested,
show proposed wording and placement without claiming the move is complete.

## Results: Analytical Purpose, Findings, and a Small Conclusion

Use a three-part progression for each coherent analysis or subsection, without imposing three
paragraphs or printing these planning labels in the answer:

1. **Analytical purpose:** at the start of a coherent analysis or subsection requested as manuscript
   Results, make the analytical purpose explicit. Name the comparison and the question
   it answers, for example `The analysis compared classification accuracy across the three
   tested recording durations to assess the contribution of recording length.` Do not substitute a bare first finding (`Accuracy
   increased...`) for the purpose sentence. Keep this opening concise and specific to the
   experiment actually performed; avoid rhetorical questions, generic previews, and repeated Methods.
   For a direct numerical answer or a brief table explanation outside manuscript drafting, an
   explicit purpose sentence is optional when it would only restate the user's question.
   In manuscript body prose, state the section's analytical aim directly rather than identifying
   its ordinal experiment: avoid openings such as `The first experiment compared...`, `The second
   experiment assessed...`, or `第三个实验旨在...`. Use natural, varied constructions such as
   `This section evaluates...`, `The comparison assesses...`, or `The scenario analysis examines...`.
   Do not repeat `This section aims to...` mechanically across sections. Retain numbered experiment
   labels in Methods headings or cross-references when they help navigation.
2. **Findings:** lead evidence paragraphs with a concrete, supported finding or consequential
   comparison, then supply the relevant figure/table and decisive magnitudes, groups, conditions,
   and exceptions. Do not repeat the subsection's purpose at the start of every evidence paragraph.
   Give the finding enough specificity to identify the task, actor, outcome, or relationship at issue;
   `values increased` or `differences exist` alone rarely answers the research question. Explain what
   the evidence reveals rather than transcribing cells or listing visual features. Support substantive
   interpretations with the actual comparison, and distinguish proposed explanations from findings.
3. **Small conclusion:** close with a brief answer to the opening purpose, normally one or two
   sentences. State what the preceding findings establish together. It can be the final sentence of
   the evidence paragraph; a separate closing paragraph is optional. It need not introduce a new
   result or interpretation, and should not repeat all numbers or drift into broad implications.
   If the final concrete comparison already answers the purpose, it is the conclusion; stop there.
   Do not add a generic summary merely to make this three-part progression visible.

### Direct declarative body prose

For this user’s manuscript body prose, avoid `how` and `when` constructions. State the analytical object, relationship or condition directly: `evaluates the effects of separate thresholds on workload` instead of `examines how thresholds affect workload`; `under threshold-based selection` instead of `when selection uses thresholds`. Preserve the scientific condition and temporal meaning through precise declarative wording, rather than simply deleting the clause. Check purpose statements, transitions, Discussion and Conclusions as well as Results. This rule does not alter exact source quotations, reference titles, variable names or mathematical notation.

### Multiple Figures or Tables: Separate Analyses with a Shared Logic

For this user's manuscripts, highlighting a figure or table reference means bold text only. Bold the numbered reference in body prose and the numbered label in captions; do not add a background highlight, shading, or a colored box. Remove background highlighting previously added for this purpose while preserving unrelated, explicitly requested color coding. Apply the same convention to Chinese 图 and 表 references. A later explicit request for a background color overrides this preference.

When several figures or tables serve the same analysis, identify the common question and the distinct
evidence each display contributes before drafting. This also applies when a single image contains a
chart and a data table. Use separate paragraphs when their analytical roles differ: for example, a
line chart locates changes over time while its accompanying table provides exact comparisons and
index levels. Connect the paragraphs through the finding, without restating the same values in both.
Do not force all displays into one paragraph or automatically assign one paragraph to every panel.

Keep the opening focused on the research question rather than an inventory of figures and their
roles. The common question and each display's contribution can remain an internal planning map.
For figures taking different analytical angles, develop one analysis before introducing the next:
state the first figure's finding, provide its decisive comparisons and meaning, then use the
substantive relationship to introduce the next figure. For example, finish the temporal pattern
in Fig. 1 before turning to the geographical distribution in Fig. 2. Avoid combining `Fig. 1 and
Fig. 2` in an opening paragraph merely because both belong to the same subsection. Cite each figure
beside the finding it supports. Joint citations remain appropriate for a finding established by
both displays; select the sequence by analytical logic rather than imposing figure-number order.

For both ordinary image/table analysis and manuscript Results prose, keep the purpose-findings-
conclusion structure implicit. Do not introduce paragraphs with process labels such as `分析目的：`,
`折线图：`, `数据表：`, `小结：`, or their English equivalents. Write natural opening and transition
sentences instead, and integrate the brief conclusion into the final evidence paragraph when possible.
Use labeled breakdowns only when the user explicitly requests an outline or labeled format.

Choose the order from the analytical relationship, not the figure letters alone. Useful relationships
include overall pattern to subgroup detail, aggregate outcome to measured component breakdown,
comparison to an observed exception, or main finding to sensitivity within tested settings. Select
only a relationship supported by the actual analyses. Do not imply that a later figure explains a
causal mechanism or validates an earlier result unless the evidence establishes that role.

A useful multi-figure progression is:
`shared purpose -> first figure's findings -> the question or comparison motivating the next figure
-> next figure's findings -> brief conclusion combining their contribution to the shared purpose`.
With more figures, extend the evidence sequence without mechanically repeating this wording.

Make transitions substantive. For example, if Fig. 2 establishes an aggregate difference and Fig. 3
contains compatible component results, introduce Fig. 3 by stating that the analysis next compares
how this difference is distributed across components. Merely saying `Fig. 3 shows...` or `Furthermore`
does not explain the link. When a subsection contains several figures that address different analytical angles, close the
first figure’s analysis with a one-sentence, evidence-grounded takeaway, then state the question
or comparison that motivates the next figure. For example, decision-utility evidence and feature
attribution evidence need a transition from what the model adds to which attributes shape its
output. Do not imply causal explanation or validation unless supported. Reuse an adequate existing
closing sentence instead of appending a second recap. Figures contributing to the same comparison
do not each require a separate summary. If displays address unrelated questions, give each its own
purpose and conclusion rather than inventing a connection.

Across consecutive Results paragraphs, vary opening syntax according to the analytical role. Avoid
repeated openings such as `Figure X shows...`, `The results indicate...`, or `To assess...`. A figure
reference can follow the analytical point or appear within the sentence. Preserve technical terms
and useful parallelism; do not merely substitute synonyms or repeat a new template.

Identify the actual source precisely, for example `Fig. 2` or `Fig. 2(c)`, without using `panel`.
For this user's manuscript prose, use figure references throughout instead of `panel` or `panels`. Use verified subfigure labels such as `Fig. 3(a)` when present. If the figure has no lettered subdivisions, write `the left-hand curve in Fig. 3` or `the right-hand comparison in Fig. 3`; do not invent subfigure labels or use `the left figure` when both parts belong to one figure. Check the finished manuscript for remaining uses of `panel`, preserving exact quoted or bibliographic titles.
Figures need not have subfigures, and there is no requirement to narrate (a), then (b), then (c).
Integrate related evidence from tables where useful. Do not manufacture findings merely to mention
every subfigure.

For familiar bar charts, line charts, and similar standard displays, rely on the existing axes and legend instead of explaining their ordinary reading mechanics. Explain an encoding only when the display or metric is sufficiently unusual that the explanation changes interpretation. Place that brief explanation immediately after the relevant figure/table citation, following 图表标题与说明的位置 below. Full procedures belong in Methods. Do not append explanatory captions or table notes. Use map labels and source tables to check place names, groups, and spatial claims. Do not call visually neighboring high values a statistically significant cluster without a corresponding test.

Select high-signal numerical anchors: direction and magnitude of a difference, key groups, contrasting cases, and important exceptions. Preserve units, denominators, rounding, and observation/estimate distinctions. A relative rank is not an adequacy rate; category membership is not statutory compliance; a sensitivity range is not automatically a confidence interval.

### Result values belong in sentences, not parentheses

For this user's Chinese and English Results prose, do not use parentheses to carry result values, model comparisons, or interpretive asides. State the model, metric and value in the sentence, and explain the comparison directly. For example, replace `Average precision was higher (CatBoost 0.1134; logistic regression 0.0816)` with `Average precision was 0.1134 for CatBoost and 0.0816 for logistic regression.` Retain only numerical anchors needed for the argument. Integrate standalone figure references into the sentence instead of placing them in parenthetical asides.

This prose rule does not alter mathematical notation such as R(30), numbered equations, subfigure identifiers such as Figure 3(a), necessary first-use abbreviation definitions, or exact reference titles. Do not delete or change scientific symbols to satisfy a punctuation check.

### Analytical Depth: Complete the Evidence-Based Comparison

Depth comes from fully explaining relationships within available evidence, not adding speculation. Before drafting, translate the subsection's purpose into the concrete judgment its evidence can support: which objects differ, in what respect, under which conditions, and which exceptions change the overall reading. A purpose such as "analyze spatial differences" is insufficient if the results can establish a more specific comparison.

Build the narrative around consequential comparisons rather than a list of examples. Depending on the evidence, useful contrasts include similar demand with different capacity, different aggregate categories with similar functional mismatch, a trend and its exception, or a change that appears only under certain conditions. These are options, not mandatory comparison types. Explain what each selected contrast contributes to the subsection's central judgment. Preserve the model, population and data version when comparing; one model's functional breakdown cannot explain another model's score without supporting evidence.

Do not use statements such as "differences exist", "a comprehensive assessment is needed", or "further analysis is required" as substitutes for an interpretation already supported by the displayed data. State the specific difference and its consequence for the analytical judgment. If the evidence genuinely does not support a finer explanation, identify that boundary rather than inventing mechanisms, recommendations or numerical details.

Analytical completion does not require causal explanation, exhaustive description of every object, or a longer paragraph. Prefer a few well-supported contrasts that answer the purpose. Do not relegate the subsection's central answer to Discussion merely because explaining the comparison requires more than listing values.

### Decisive synthesis and question-level figure titles

For this user's Results, a closing synthesis must take a clear, evidence-supported position. State which method is preferable for the evaluated task, what the integrated approach demonstrably adds, or which condition changes the decision. Avoid neutral endings such as “provides a basis” or “requires consideration” when the comparison supports a specific judgment. A directional conclusion does not authorize stronger evidence: retain the tested population, objective, workload and uncertainty boundaries; do not manufacture a winner when results do not distinguish one.

Figure titles should name the broader analytical question or decision supported by the display rather than merely enumerate its plotted metrics. For example, use “Resource allocation for additional deterioration detection” instead of “Additional inspection yield and cost.” Keep titles specific, concise and evidence-bounded; place metric definitions and reading instructions in the body.

### Small Conclusion: Answer the Purpose, Do Not Repeat

The closing sentence(s) or final paragraph of a Results subsection should integrate the preceding findings into an overall answer to its analytical purpose, rather than repeat the same numbers, county names, categories, or individual conclusions with "overall" added. Apply this principle to a chapter-level Results summary as well, if one is requested.

A useful synthesis identifies a relationship across findings: a shared pattern, a meaningful contrast, complementary information provided by two measures, or a condition under which the conclusion changes. Explain what the evidence establishes when considered together. The added value is a concise answer to the purpose, not a requirement to introduce a new interpretation beyond the individual findings.

Make that synthesis concrete when the research purpose calls for it. For a screening subsection, identify supported higher-concern and relatively less prominent objects, explaining the different evidence behind their positions; do not declare lower-ranked objects safe or impose an untested priority threshold. For other purposes, identify the supported relationship, contrast, or condition instead. Do not force every Results section to end with a list of priority locations. Avoid re-listing all earlier examples: retain only the objects necessary to express the integrated judgment.

Do not satisfy this requirement by inventing mechanisms, causal explanations, broad generalizations, or policy recommendations. Leave these to Discussion when evidence warrants them. Avoid generic closing statements such as "these results provide an important basis" or "a comprehensive assessment is necessary" without a specific demonstrated connection.

Before retaining the closing paragraph, ask: if it were deleted, would the reader lose a meaningful synthesis or only a recap? If it adds no synthesis, rewrite it around a supported relationship, merge its useful point into the preceding paragraph, or omit the separate closing paragraph while retaining a concise answer in the preceding text. Do not force an extra summary paragraph merely to complete a template. Normally avoid repeating numerical details unless a concise comparison is indispensable to the synthesis.

The last specific finding can itself complete the answer. Once a comparison identifies the resource
concern in each area, a sentence stating that “resource concerns differ” adds no synthesis. End at
the supported comparison instead of rephrasing it as a broader conclusion.

## Discussion: Meaning, Credibility, and Implications

Organize around a small set of substantive findings, not one paragraph per figure. For this user's preferred structure, prioritize:

- **Meaning of the findings:** explain the substantive pattern and how it extends, qualifies, or contrasts with existing knowledge.
- **Method credibility and applicability:** identify what the comparisons, validation, and sensitivity tests actually establish and where the approach applies.
- **Implications:** connect findings to concrete decisions, actors, or preparedness functions at the resolution justified by the evidence.

A useful paragraph moves from finding to interpretation, relevant literature, and consequence. Vary this pattern when the argument benefits; do not mechanically repeat all four elements in every paragraph. Use a few numerical anchors only when necessary, rather than repeating Results.

Distinguish explanation supported by data from a plausible mechanism. Verify original scholarly sources before adding new citations or attributing claims to them; preserve existing citations during translation without pretending that this constitutes a fresh source audit. A methods reference supports the method's origin, not automatically its validity for the current dataset or parameter choices.

Separate kinds of evidence:

- Comparing models demonstrates consequences of assumptions, not superiority or accuracy by itself.
- Sensitivity analysis supports stability within tested settings, not external validity.
- A numerical allocation identity checks implementation consistency, not physical stock availability.
- Agreement with independent, comparable observations can support empirical validity; identify temporal, geographic, or measurement mismatches.

State important boundaries once at the point where they constrain interpretation. Do not fill the section with repeated disclaimers. Integrate limitations or use a separate subsection according to user/journal needs; do not force a new limitations section, but never omit a consequential limitation for stylistic reasons.

Implications should follow the chain `finding -> relevant decision -> condition for applying it`. Avoid inventing budgets, numerical resource targets, causal effects, or actionable dispatch plans from relative indices alone. A synthesis table or diagram may clarify evidence-to-decision links when requested, but should not simply duplicate a Results figure or introduce unsupported recommendations.

## 图表标题与说明的位置

适用于本用户的论文撰写、结果解读与图表文字修订，中英文一致。图表只保留编号和简短标题；说明在正文引用处展开。

1. **标题标明主题。** 使用简洁、自然的名词短语，保留区分图表所需的研究对象或比较维度。不要写成结果总结句，不把变量清单、分析步骤、方法细节、结论和含义全部塞进标题；也不要缩成 “Results” 或 “Analysis” 等无法辨认主题的空泛词语。不设机械字数上限。
2. **减少词汇与概念堆砌。** 用准确的上位概念概括细项，避免多层修饰和连续列举；以实际图表内容为准，不能为了缩短而误述范围。示例：`Data sources and processing procedures for estimating demand, local capacity, and regional accessibility` → `Data sources categorized by demand and capacity`；`Experimental settings for demand, resource availability, road access, and classification` → `Parameters and settings for mismatch assessment`。示例体现精简尺度，不是套用到其他图表的固定标题。
3. **不附加解释性图注或表注。** 图表旁仅有 `Fig. X. 简短标题` 或 `Table X. 简短标题`，不在标题后、下一段或图表下追加长说明，也不改名为 `Note:`、技术注释、脚注或文本框来绕过规则。此处 caption 样式仅承载编号与标题，不代表允许扩展说明。保留图内必要图例、坐标标签、单位和表头；本规则不要求删改图表资产。
4. **说明紧随正文引用，按理解难度控制篇幅。** 默认用图内图例、坐标和标签说明常规含义，不逐项复述读者已能直接读出的颜色、位置、分图名称或数字。正文首次实质性引用图表后，只简要解释影响正确理解的指标、单位、尺度、分母或比较条件，并随即报告发现。只有图形或指标确实难懂时才展开必要解释，仍融入正文对应段落；后续才涉及的口径放在相应引用之后。不要在图下另写 Note／注释段，也不把长图注原样搬成独立正文段落。完整计算方法保留在 Methods。
5. **迁移信息，不丢信息。** 修改既有稿件时，将原图注和表注中的必要信息逐项对应到正文引用处，保留来源、数值、定义和限制。正文已解释的内容合并去重，不重复添加；只删除重复内容或已迁移内容，检查编号、引用与分图对应关系。
6. **遵守编辑范围。** 仅提取标题、只读解读或纯格式任务不自动授权改写和移动正文。要求落实本规则属于图表文字及对应正文的局部内容修订，应选用相应编辑模式。保留无关段落。
7. **交付前核对。** 标题是否简短、自然且能区分图表；图下是否只保留编号与标题，有无独立 Note／注释或读图说明；正文是否只解释必要口径，并以具体发现为主；迁移后是否保全解释与证据。若明确的期刊要求与此规则冲突，说明具体冲突并按用户指示处理，不自行恢复长图注。

## Language and Headings

### Research purpose and domain language before descriptive detail

Before retaining a subgroup comparison, identify the research domain and the subsection's question. Keep a count, grouping, contrast, or exception only when it contributes to that question. Do not add generic reminders such as one observation equalling a percentage-point increment, a small group requiring consideration, or a group existing solely because the data were divided that way. Preserve the actual sample and denominator in Methods or the existing source table.

Results report findings about the research object. Do not narrate analytical procedures or the article's limitations in Results. Put reproducible methods and display processing in Methods, and consequential study limitations in the relevant Discussion text. Express a finding at its supported scope so that moving these explanations does not turn an association into an effect or policy text into implementation performance. Preserve a local condition when removing it would change the finding itself.

Choose established words from policy analysis, CDW management, or the actual study field. Replace an unfamiliar imported label with the measured object before writing a long explanation of it. For example, report the market-support categories included in policies instead of unexplained `breadth`; explain small display offsets in Methods rather than introducing `jitter` in Results. Keep necessary established method names and notation. Avoid conversational `so` in authored scientific prose; state the relationship directly or use a full stop, without altering quotations or reference titles.

In figure revisions, remove arbitrary bold emphasis before deciding whether any data label needs renewed emphasis. Restore emphasis only when the body develops the exact contrast and that contrast contributes to the subsection's question. A largest value alone is insufficient. Preserve ordinary figure-reference typography in the manuscript unless the user also asks to change it. A later request to remove all in-figure bold applies to headings, labels, and values alike.

Prefer the research field's own vocabulary when naming indicators, figures, and findings. First
replace unnecessary imported abstractions with an established domain term or a direct description
of the measured object; a longer explanation of a complicated label is not the default repair.
Choose names from the study's accepted terminology and supplied disciplinary sources, then use a
direct description if no suitable term exists. Check necessity before explaining or introducing a
new abstract label. Preserve the indicator's definition, formula, unit, and scope. Retain
cross-disciplinary method names where the analysis genuinely needs them, define them in Methods,
and express their substantive findings in the field's language.

For policy or document studies, read the terminology-selection steps and worked examples in
[Policy Results in Domain Language](references/policy-results-domain-language.md) when drafting or
reviewing indicator labels and substantive findings. Apply the same naming principle in other
fields using their own research objects. Check headings, axes, legends, and body prose together;
an accessible explanation does not repair an unnecessarily abstract label left in the figure.

Replace vague phrases such as "connected evidence layers" with the actual comparison or finding.
Avoid repeated section previews, unexplained abbreviations, decorative jargon, and colloquial
commentary. Readability does not require reducing the scientific argument to conversational slogans.

Keep titles concise, neutral, and specific to the studied phenomenon. Avoid unsupported evaluative headings such as "validated superiority". Introduce symbols where their meaning matters and avoid using model codes as a substitute for explanation. Do not rename technical terms in equations, citations, or data keys solely for stylistic variety.

### Simple, concrete findings (学术直说)

Use the plain-statement method during initial drafting and authorized revision, not only as a final
wording pass. Read the whole comparison first, then write the object, observed difference, and
supported meaning in familiar words. Keep analysis focused on relationships in the supplied evidence.

- With the study population and M1 setting defined, write `纳入道路支援后，小金的错配仍然最高。`
  instead of `纳入道路支援的M1仍以小金居首，可达的外部资源尚未改变其突出的相对薄弱状况。`
  Name the measured result rather than describing an abstract “relative weakness”.
- If concrete cases already establish the difference, retain those cases and their decisive values.
  Do not append “different functional combinations occur” or “further functional analysis is needed”
  after already identifying each area's main resource concern. Add interpretation only if it explains
  another supported relationship relevant to the subsection's question. Analytical depth does not
  require a longer paragraph or a new statistical analysis.
- For joint-sampling results, report the actual frequency or range. “In most draws” must not become
  “in every draw”. If the input only reports group frequencies and contains no investment-order
  analysis, stop at the frequencies and their direct interpretation; remove an appended investment-order
  rebuttal. Keep that limitation if the research actually evaluates investment ordering.
- Explain necessary definitions once in direct language. Preserve the comparison set, denominator,
  classification thresholds and equality rules, and the difference between a relative score and an
  actual resource quantity. A demand–capacity category is not a top-N mismatch ranking. A set formed
  by selecting the top three within each function and removing duplicates is not the overall top nine.
- Keep natural paragraph connections and meaningful exceptions. Simple wording must retain the
  argument, adverse findings, uncertainty, notation, and citations. Do not substitute generic advice
  for explanation or compress a technical definition until its calculation becomes ambiguous.

These examples illustrate editing decisions, not portable research findings. Further worked examples
are in [学术直说](../plain-academic-writing/SKILL.md). The rules above are embedded in this skill;
no separate plain-academic-writing invocation is required.

### Direct, Natural Prose with Less Defense

Apply this pass during both drafting and review, in Chinese and English. These rules integrate the
relevant principles of `be-human-and-less-defense` as an operational checklist. Load the companion
as specified above and apply both from initial generation; these embedded rules also provide a
fallback if the companion is unavailable.

- **Scope the claim itself.** Prefer a precise statement of what the analysis establishes over a
  broad assertion followed by a disclaimer. When the tested scope is established, `Across the three
  tested conditions, Model A had higher F1 scores than Model B` is sufficient. Do not routinely append
  `This does not imply superiority under all conditions`. Do not repeat scope in every sentence when
  it is already unambiguous from the subsection.
- **Audit generic defense.** Inspect `X does not imply Y`, `this does not mean that`, `should not be
  interpreted as`, `applicability is limited`, `xxx 并不代表 xxx`, `不能据此认为`, and `适用条件有限`.
  Delete them when they add no evidence, scope, logical distinction, or guidance needed to interpret
  the finding. Replace vague boundaries with source-supported conditions when needed. Do not invent
  conditions or add a generic caution to every paragraph ending.
- **Keep consequential boundaries where they matter.** A distinction such as association versus
  causation or relative ranking versus adequacy can be essential. State it concisely once at the
  relevant level, repeating only if a later claim creates a new ambiguity. Keep qualifications that
  change a local result's meaning in place. Broader generalizability may belong in Discussion, but
  move existing text between sections only within authorized restructuring scope.
- **Keep Methods explanations concrete.** When explaining relevant Methods or editing them within
  the user's requested scope, state procedures, selection reasons, assumptions, and operating
  conditions directly. Preserve reproducibility requirements. Do not expand a Results task into a
  Methods rewrite merely to remove defensive wording.
- **Remove self-undermining and hypothetical rebuttals.** Review `merely`, `only a preliminary attempt`,
  `本研究仅仅`, and habitual `not X but Y`. Preserve real distinctions and study-design information,
  but remove apology-like framing and defenses against objections no one has raised. In a response
  to an actual reviewer comment, retain the explanation required to answer it.
- **Reduce punctuation clutter.** Avoid rhetorical em-dashes and dash-delimited asides. Reduce
  semicolons joining separate claims, preferring direct syntax or full stops. Keep punctuation needed
  for complex lists, citations, technical hyphens, ranges, mathematical signs, and formal notation.
  Do not replace every dash with another recurring punctuation pattern or create comma splices.
- **Vary prose according to meaning.** Check openings, sentence structures, and endings across
  paragraphs. Reduce repeated `These results suggest that`, `X ..., while Y ...`, `By doing X, we ...`,
  `..., highlighting ...`, and their Chinese equivalents. Preserve warranted uncertainty, consistent
  technical terms, and useful parallelism in matched comparisons. Do not force synonym variation.
- **Make claims concrete without changing evidence.** Replace empty praise and template emphasis
  with the actual finding where supported. Preserve all numbers, results, equations, technical terms,
  and citations. Do not invent evidence or strengthen a claim to make the prose sound more confident.

## Writer and Reviewer Workflow

Use two distinct roles for drafting and substantive revision. They are workflow roles, not permission to create new user-facing tasks. When an authorized subagent tool is available, a separate Reviewer can provide an independent pass. Otherwise perform a separate reviewer pass in the current task and describe it honestly as role-based self-review, not an independent agent evaluation. Review-only requests begin with the Reviewer; activate the Writer only when a revision is requested.

### Writer

- Read the evidence and identify the subsection's purpose and central finding. Establish the independent unit and design, then select the comparison directions needed to answer that purpose.
- Specify the concrete answer the subsection should deliver, select the comparisons that establish it, and remove examples that add no analytical role. For multiple figures, identify each figure's role and the logical transition connecting it to the next. Close the analysis with a brief answer to its opening purpose. Decide which decisive evidence stays in the main Results and which verified detail belongs in the supplement.
- Draft in the requested language and scope, arranging evidence by logical relevance rather than figure lettering. Apply `be-human-and-less-defense` during this initial composition, not only after the candidate is written.
- Separate direct observations, supported interpretations, and hypotheses. Prefer a narrower supported statement over a speculative statement followed by a disclaimer.
- Apply the direct-prose pass before submitting the candidate: consolidate shared scope, remove redundant defensive endings, and check punctuation and repeated sentence templates across paragraphs.
- Give the Reviewer the candidate, relevant Methods and adjacent text, and the original evidence with version information. Do not supply only the Writer's interpretation of the evidence or demand approval of the draft.

### Reviewer

Evaluate the candidate against the sources, not just grammar. Check:

1. **Argument logic:** the stated purpose is answered; each conclusion follows from the evidence presented; comparisons use compatible populations, denominators and settings; adjacent paragraphs progress rather than repeat or contradict one another.
2. **Excessive inference:** flag causal claims from descriptive associations, accuracy claims from model differences, broad generalizations from selected cases, and mechanisms or recommendations unsupported by the analysis. Check that cited literature supports the exact claim, rather than merely sharing its topic. Remove or narrow unsupported inference; labeling it "possible" is not by itself a sufficient repair.
3. **Excessive defense:** identify repeated limitations, anticipatory rebuttals, unnecessary "not X but Y" sentences, and qualifications that overwhelm the finding. Delete redundant defense or consolidate it at the point where it matters. Retain limitations that materially change interpretation, even when they make the conclusion less favorable. Do not remove necessary uncertainty simply to make the prose confident. Apply the concrete phrase and scope checks above. Prefer narrowing the original claim over appending another disclaimer. Require a new caveat only when its absence causes a specific interpretive error, and identify that error under the Reviewer Finding Threshold.
4. **Results/Discussion distinction:** Results report and synthesize findings; Discussion interprets their meaning and implications without repeating the entire result. For combined sections, preserve the observation-to-interpretation distinction within the narrative.
   Check the small conclusion specifically: does it answer the opening purpose by bringing the findings together? It may be one or two sentences rather than a separate paragraph. If it only repeats earlier content, locate both the repeated sentences and their earlier counterparts, explain the redundancy, and propose consolidation or removal. Do not demand novel interpretation when the evidence supports no additional synthesis.
5. **Evidence and readability:** confirm numbers, figure references, citations and version alignment; check that terminology is disciplinary and understandable, without turning academic prose into slogans. If material was condensed or relocated, check that the main claim remains assessable and every supplementary pointer resolves to a matching source. Check rhetorical dashes, repeated semicolons, and recurring sentence or paragraph-ending templates. Treat minor style preferences as optional unless the user explicitly requested that language pass; do not use them to prolong substantive review.
6. **Analytical completion:** check that the section actually answers its purpose through specific differences, contrasts and exceptions rather than a catalog of values followed by a generic conclusion. For vague phrases such as "differences exist", "these factors should be considered together", or "further analysis is needed", inspect whether the available evidence already supports a more specific statement. If so, identify that evidence and the omitted judgment, then request the smallest adequate clarification. If not, do not demand unsupported depth. For screening results, check that any identification of higher-concern or less prominent objects is supported and scoped to the assessed outcome. For other research purposes, do not impose a screening interpretation.

Check statistical comparisons where relevant: independence or pairing, repeated/clustered observations,
compatible outcomes and denominators, effect size versus uncertainty, multiplicity when making many
inferential comparisons, and whether an interaction was actually assessed. Check the exact method
against its assumptions rather than requiring a named test for every comparison. Apply the finding
threshold below to concrete errors, not to hypothetical requests for more analysis.

### Reviewer Finding Threshold

Do not manufacture or continually add objections to appear rigorous. Review quality is measured by consequential errors identified and resolved, not the number of criticisms or revision rounds. No minimum finding count or arbitrary quality score is required.

Every required revision must contain all of the following:

- **Location and wording:** quote the specific sentence and identify its section/paragraph. For a missing logical link, identify the adjacent sentences; for a contradiction or repetition, identify both locations.
- **Actual problem:** explain the concrete error, ambiguity, unsupported inference, or redundancy. "Insufficient rigor", "needs depth", or "a reviewer may question this" alone is not a finding.
- **Evidence:** identify the conflicting source, internal inconsistency, or evidence needed to establish the claim. Distinguish an observed error from a verification gap; lack of access does not establish that a statement is false.
- **Consequence:** state how the problem changes a reader's understanding, the validity or scope of a conclusion, or the ability to follow the argument. A hypothetical objection with no concrete consequence is not a required revision.
- **Proportionate repair:** propose the smallest adequate action: delete, narrow, clarify, reorder, correct, or verify. Do not default to more citations, experiments, qualifications, or defensive prose.

Use a compact format when reporting: `Location/quote | Problem and evidence | Effect on understanding or conclusion | Minimal repair`.

Separate required corrections from optional style preferences. If two formulations are accurate and comparably clear, do not require the Writer to adopt the Reviewer's preferred wording. Omit negligible preferences unless the user requests stylistic alternatives. Merge comments with the same underlying cause; do not count the same issue separately in each paragraph.

An already resolved finding stays closed unless new evidence, a regression, or a newly identified substantive error warrants reopening it. A later finding must meet the same threshold; do not move the acceptance criteria merely to prolong review. State "No material issue found within the reviewed scope" when appropriate, and separately identify any genuine verification gaps. This restraint must not suppress real errors or material limitations.

### Revision and Release

The Writer addresses review findings without changing underlying data or inventing new analyses. The Reviewer then rechecks the changed claims and transitions. Use one draft-review-revision cycle by default, adding a targeted pass only for unresolved substantive issues. Stop when material issues are resolved or further progress requires evidence or a user decision; report the unresolved point rather than looping or silently approving it.

Return the revised candidate and, when useful, a short account of substantive fixes. Do not put internal reviewer comments, warnings about unfinished tool work, or editorial labels inside manuscript prose. During bilingual review, user approval remains required before synchronizing the candidate to the source manuscript. Do not claim this process guarantees correctness.

## Saved Manuscript Changes

When authorized to edit a document, use the available document or paper-format workflow for file mechanics. Preserve user edits, references, equations, figure-number fields, and table structure. For this user, save a new file using the original filename plus version and timestamp, with a concise Markdown version-management entry.

Reopen the saved artifact and compare requested changes against the source. For layout-sensitive edits, render and inspect the affected pages; report if visual inspection could not be completed. Do not claim that a newly saved manuscript, figures, supplementary materials, and submission archive are all synchronized unless each was updated and verified.

## Final Quality Check

- When drafting manuscript Results, does the opening sentence explicitly state the analytical purpose before reporting the first finding? Does evidence precede interpretation?
- Does it complete a concrete analytical judgment using meaningful comparisons, rather than merely list findings or postpone an answer already supported by the evidence?
- Does the analysis close with a brief, supported answer to its opening purpose, integrated into the last evidence paragraph when a separate conclusion would be redundant?
- Are findings stated directly, with empty abstractions and duplicate explanations removed? If the last concrete comparison already answers the purpose, has the text stopped there while retaining necessary definitions and conditions?
- For multiple figures or tables, including a chart and table in one image, is each display's analytical role clear, with separate paragraphs when their contributions differ and substantive transitions connecting them? Has the answer avoided unrequested process labels and duplicate narration of the same values?
- When adjacent figures use different analytical angles, does a one-sentence takeaway close the first analysis and a substantive transition introduce the next? Do consecutive paragraph openings vary without changing technical meaning?
- Are comparison directions chosen for the research question, with the independent unit and dependence structure respected?
- Are effect magnitude, supported uncertainty, and practical meaning distinguished, without invented tests or significance claims?
- Are decisive findings and exceptions retained in the main Results, with detailed secondary evidence placed in a verified supplement and cross-referenced accurately?
- Can all values, groups, spatial claims, and citations be traced to the correct version?
- Do emphasized labels and marks match the comparisons actually discussed, and are illustrative cases introduced by a supported finding or an explicit case-level question?
- Does each conclusion trace to a finding established in Results, with metric meaning and units kept consistent across Methods, figures, and prose?
- Do indicator names and findings use the study field's own terms or concrete objects, with unnecessary imported abstractions removed consistently from headings, figures, and prose without changing the measurements?
- Does each Discussion claim add interpretation rather than restate a result?
- Has the Reviewer checked the argument against the evidence, narrowed excessive inference, and removed redundant defense without suppressing material limitations?
- Does every required review comment identify specific wording, an evidenced problem, its concrete consequence, and a proportionate repair, rather than an optional preference or invented objection?
- Is scope expressed directly without repetitive "does not imply" or "applicability is limited" endings, while retaining locally necessary qualifications?
- Have rhetorical dashes, excessive semicolons, and repeated prose templates been reduced without altering technical notation, evidence, or useful parallelism?
- Are accuracy, stability, comparative differences, and implementation checks distinguished?
- Are relative scores, imputed inputs, unrun analyses, and uncertainty honestly represented?
- Does the final message distinguish proposed wording, saved edits, and pending calculations?

For review-only requests, lead with consequential findings and locations, then provide a focused revision. For drafting requests, deliver the requested text rather than an unsolicited long audit.
