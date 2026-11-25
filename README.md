# Result Explainer · 看图说话大师

用于解读科研数据、图表和比较结果，撰写或审阅中英文 Results、Discussion 及合并章节。稳定调用名是 **`results`**，显式调用为 **`$results`**。

A research skill for interpreting data, tables, figures and comparisons, and drafting or reviewing Results, Discussion, or combined sections in Chinese and English. The stable identifier is **`results`**; invoke it with **`$results`**.

## 能做什么 / Capabilities

- 围绕“分析目的—关键发现与比较—简短结论”组织解释，并串联多张图表。Organize evidence around the analytical question, meaningful comparisons and a brief conclusion.
- 按研究问题与数据设计选择比较，区分效应大小、不确定性和实际意义；判断正文与补充材料的证据分工。Choose design-compatible comparisons and separate decisive findings from supplementary detail.
- 用 Writer / Reviewer 两个角色检查论证、证据、过度推断与重复防御表达；数据计算仍需合适工具及真实输出。Use Writer / Reviewer roles to check reasoning, evidence, overinterpretation and unnecessary defensive prose. Calculations require suitable tools and verified outputs.

## 安装 / Installation

这是公开发布版本，无需申请仓库权限。将两个仓库分别安装到下列稳定技能目录；依赖仓库名中历史保留的 `-private` 不应带入本地技能目录名。

Both repositories are publicly accessible. Keep the local companion directory named `be-human-and-less-defense`, without the repository's historical `-private` suffix.

```bash
skill_home="${CODEX_HOME:-$HOME/.codex}/skills"
mkdir -p "$skill_home"
git clone https://github.com/AISlowDown/results.git "$skill_home/results"
git clone https://github.com/AISlowDown/be-human-and-less-defense-private.git "$skill_home/be-human-and-less-defense"
```

配套技能 [be-human-and-less-defense](https://github.com/AISlowDown/be-human-and-less-defense-private) 从初稿开始约束表达。若未安装，`results` 有内置降级规则，并会简要说明缺少配套技能。

The companion guides expression from the first draft. If it is unavailable, `results` uses its embedded fallback rules and briefly reports the missing companion.

`SKILL.md` 另有指向 `../plain-academic-writing/SKILL.md` 的可选扩展示例引用。核心直说规则已内置；该可选技能不包含在本仓库中。

`SKILL.md` also references optional worked examples in `../plain-academic-writing/SKILL.md`. Core direct-prose rules are embedded; that optional skill is not included here.

## 调用示例 / Examples

```text
$results 分析这张图和表，说明关键差异、异常及其对研究问题的意义。
$results 根据这些结果撰写 Results，再用 Reviewer 角色检查证据与推断。
$results Review this Results and Discussion section against the supplied figures and data.
```

提供图表、必要的数据或统计输出、研究问题和写作范围。仅解释已有图表不会自动授权新增实验、推断不存在的统计量或改写源文件。

Supply the figures, relevant data or statistical outputs, research question and desired scope. Interpretation does not authorize new experiments, invented statistics or unrequested source-file edits.

## 内容 / Contents

- [SKILL.md](SKILL.md): 工作流与证据规则 / workflow and evidence rules.
- [references/](references/): 比较方法、指标解读、政策结果表达、正文与补充材料分工 / supporting guidance.
- [agents/openai.yaml](agents/openai.yaml): 界面元数据与自动调用策略 / UI metadata and invocation policy.

本发布版本保留源技能的写作规则与学术案例；未新增许可声明。

This release preserves the source skill's writing rules and academic examples. No new license is assigned.
