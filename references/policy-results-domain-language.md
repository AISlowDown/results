# Policy Results in Domain Language

Use this reference when choosing policy-analysis terminology, explaining indicators, or replacing
analytical bookkeeping with substantive findings. Prefer names familiar to the study's field and
direct descriptions of policy provisions. The CDW examples are contextual choices, not a universal
replacement dictionary. The worked historical example below comes from the author's manuscript
revision on 15 October 2026.

## Choose terminology before adding explanations

1. **Identify the object and actual measure.** Establish whether the statement concerns a management
   task, provision, responsible actor, support measure, policy count, proportion, category score,
   citation, or text comparison. Check the definition and source output before changing the name.
2. **Prefer vocabulary already used by the field.** Start with the author's accepted terms and the
   supplied disciplinary literature. In a CDW paper, directly name source reduction, sorting,
   transport, disposal, resource utilization, recycled materials, procurement, and costs as relevant.
   Do not assume that an unfamiliar word is foreign to the field merely because it sounds abstract.
3. **Remove an unnecessary conceptual layer.** If a label adds no distinction beyond the actual
   object or comparison, replace it with that object or comparison. Do not retain a difficult label
   and compensate with a long explanatory paragraph. Avoid replacing one abstraction with another
   vague label such as "support capacity", "governance quality", or an undefined "degree".
4. **Retain a formal term when it performs real analytical work.** Keep the recognized name of a
   statistical method or a theoretical concept actually applied in the study. Define what is needed
   in Methods and express the substantive finding in domain language. Simplification does not
   authorize deleting a method, changing a formula, or redesigning the indicators.
5. **Use the selected name consistently.** In an authorized manuscript edit, check section and figure
   titles, axes, legends, tables, first-use definitions, Results, Discussion, and Conclusions. Maintain
   one name per measured object. Preserve formal method names, quotations, reference titles, and
   program/data keys where exact identity matters. For Chinese–English work, preserve meaning and
   use the field's natural expression rather than translating an abstract label word for word.

Keep a lightweight term map when several labels change: existing label, actual definition and unit,
proposed name, and affected locations. In a review-only task, propose replacements; do not claim they
were inserted or start new analyses. The term map need not become an extra deliverable for a simple
explanation or a single wording edit.

## Context-dependent examples

| Difficult or over-abstract expression | More direct wording when the stated condition holds |
|---|---|
| Support breadth / 支持广度 | `政策涉及的市场支持类别`; if it is the defined 0–1 mean of category indicators, label the metric `市场支持类别评分` and retain the definition. Do not relabel the score as a raw category count or a percentage. |
| Administrative completeness / 行政规定完备性 | If it only averages the presence of specified elements, use `行政规定评分` and identify responsibility, obligations, procedures, and facilities where relevant. Do not imply that a high score establishes legal adequacy or effective enforcement. |
| Policy translation / 政策转译 | `地方对中央要求的细化` for a descriptive clause comparison. Retain the formal term when a policy-translation theory is actually analyzed. |
| Task–tool co-occurrence structure / 任务—工具共现结构 | `管理任务与政策工具的组合` for the substantive comparison. Retain `共现份数` or `O/E` where naming the actual plotted metric is necessary. |
| Strengthened tool synergy / 工具协同增强 | If the evidence is only joint presence, describe the tools or measures appearing together. Do not call joint presence synergy or invent a temporal increase from pooled data. |

These examples guide naming decisions, not substitutions to run mechanically. A score's denominator,
unit, and interpretation must still match the calculation. Familiar words can also overstate a
result: policy count is not automatically policy strength, and citation is not implementation.

## Write the finding in terms of the policy content

State what the policies require, support, or connect, along with the comparison actually observed.
For example, if supported, `政策涉及的市场支持类别增加` communicates a category-score change directly.
`地方条款明确了监理审核减量方案的职责` identifies an actor and an action. Do not replace these with
an invented construct or a processing-state statement merely to sound more analytical.

Necessary indicator definitions belong with the method; result prose should emphasize the task,
measure, actor, or provision and its observed change or difference. Explaining a valid method and
reporting a concrete result are complementary. They do not require importing the method's vocabulary
into every substantive sentence.

## Observed problem

The Results paragraph described 28 policies from 1992–2004 and ended with:

> 资源化利用出现在39.3%的政策中，尚未编码到源头减量及市场支持规定。

The phrase `尚未编码到` describes the analytical operation. Readers need to know what the sampled policies actually provide for.

## Supported revision

After checking the analysis sample and the relevant provision categories, write:

> 资源化利用出现在39.3%的政策中，样本尚无明确的源头减量及再生材料市场支持规定。

The numbers and policy categories are unchanged. `样本` keeps the claim within the analyzed documents. The statement is not a claim that no such policy existed anywhere, or that no related activity occurred in practice.

## How to transfer the lesson

- Establish the research object first: policy provisions, management tasks, responsible actors, or implementation procedures specified in the documents.
- Translate analytical flags into that object's language when presenting substantive Results. Examples include `包含采购支持规定`, `明确建设单位责任`, and `未出现具体减量措施` when the accessible source supports those statements.
- Check what a zero actually means. A code may reflect inaccessible text, an exclusion rule, an ambiguous passage, or a verified absence. Use `可获取文本未明确规定…` when only that narrower statement is supported.
- Keep genuine method information in Methods: code definitions, multi-label treatment, denominators, inclusion/exclusion criteria, and treatment of missing text.
- Preserve technical coding language when coding accuracy, model classification, or annotation reliability is the analysis itself. This example does not turn coding into a prohibited term or classify all document coding as machine learning.

For this CDW example, the revised file also identifies the sample's earliest policy as Shanghai's 1992 regulation. An earliest-in-sample policy must not be called the country's first policy without a separate historical search.
