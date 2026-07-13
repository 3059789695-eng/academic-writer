# English Academic Phrasebank — Fill-in-the-Blank Templates

> How to use: Find the section you're writing → pick a template → replace ____ with your content.
> Each template includes a Chinese note explaining when to use it.

---

## Part 1: Introduction

### 1.1 Establishing the Research Territory

**Template I-1: Opening with broad importance**
```
In recent years, ____ has attracted considerable attention in the field of ____.
```
> 用法：论文第一句，开门见山说清楚领域重要性。

**Template I-2: Opening with a trend**
```
With the rapid development of ____, there has been an increasing interest in ____.
```
> 用法：强调技术或社会趋势驱动的研究兴趣。中文："随着...的快速发展，...日益受到关注。"

**Template I-3: Opening with a problem**
```
____ has emerged as a critical challenge in ____, particularly in the context of ____.
```
> 用法：从问题切入，比趋势式开头更有力。

**Template I-4: Establishing significance**
```
Understanding ____ is essential for ____, as it directly affects ____ and ____.
```
> 用法：解释为什么这个研究是重要的。中文："理解...对于...至关重要。"

### 1.2 Identifying the Research Gap

**Template I-5: General gap**
```
Despite the growing body of research on ____, relatively little is known about ____.
```
> 用法：最常用的指出现有研究空白的句式。中文："尽管对...的研究日益增多，但对...仍知之甚少。"

**Template I-6: Specific limitation of prior work**
```
Previous studies have primarily focused on ____, while ____ remains underexplored.
```
> 用法：指出前人集中在某个方向，忽略了另一个方向。

**Template I-7: Methodological gap**
```
Existing approaches to ____ suffer from several limitations: (1) ____, (2) ____,
and (3) ____. In particular, ____ has not been adequately addressed.
```
> 用法：指出前人方法的不足，适合 CS/AI 论文。

**Template I-8: Contradictory findings**
```
Notably, findings on ____ have been inconsistent. While some studies report ____
(e.g., ___, 2023), others find ____ (e.g., ___, 2024).
```
> 用法：当文献中存在矛盾结论时使用，这本身就是一个研究空白。

**Template I-9: Context gap**
```
However, it remains unclear whether these findings generalize to ____,
as most studies have been conducted in ____ settings.
```
> 用法：前人研究的发现未必适用于你的场景/人群/文化。中文："但这些发现是否能推广到...仍不清楚。"

### 1.3 Stating the Purpose and Approach

**Template I-10: Stating purpose**
```
To address this gap, we investigate ____ using ____.
```
> 用法：最简洁的目的一句话。中文："为填补这一空白，我们使用...方法研究了..."

**Template I-11: Stating purpose (detailed)**
```
In this paper, we aim to ____. Specifically, we seek to answer the following
research questions:
(RQ1) ____?
(RQ2) ____?
(RQ3) ____?
```
> 用法：列出具体研究问题（社科/管理类论文常用）。CS 论文也可用 Contribution 列表代替。

**Template I-12: Describing the paper**
```
In this paper, we present ____, a ____ that ____. We evaluate ____ on ____
and demonstrate that ____.
```
> 用法：CS/AI 系统类论文的标准一句话概括。中文："本文提出了...（系统名），一个...。我们在...上评估了...，并证明..."

### 1.4 Contributions

**Template I-13: Listing contributions**
```
Our main contributions are:
(1) We design ____, which ____.
(2) We implement ____ and evaluate it on ____, showing that ____.
(3) We provide ____ that can serve as ____ for future research.
```
> 用法：CS/AI 论文最标准的贡献列举格式。

**Template I-14: Softer contribution statement**
```
This study contributes to the literature on ____ in three ways.
First, it provides empirical evidence on ____. Second, it extends ____
by ____. Third, it offers practical implications for ____.
```
> 用法：社科/管理类论文贡献陈述，比 CS 风格更强调理论和实践贡献。

---

## Part 2: Related Work

### 2.1 Organizing Prior Work

**Template RW-1: Thematic grouping**
```
Research on ____ can be broadly categorized into ____ streams:
(1) ____, which focuses on ____; (2) ____, which examines ____;
and (3) ____, which investigates ____.
```

**Template RW-2: Chronological narrative**
```
The study of ____ has evolved considerably over the past decade.
Early work focused on ____ (e.g., ___, 2018). More recently,
attention has shifted toward ____ (e.g., ___, 2023). Most recently,
researchers have begun to explore ____ (e.g., ___, 2025).
```

### 2.2 Pointing Out Gaps in Prior Work

**Template RW-3: Summarizing gap**
```
In summary, while prior work has made significant progress in ____,
three gaps remain: (1) ____; (2) ____; and (3) ____. Our work
aims to address ____.
```

**Template RW-4: Positioning your work**
```
Our work builds on ____ but differs in the following ways: ____.
Unlike ____, which ____, we ____. Unlike ____, we ____.
```

---

## Part 3: Methods

### 3.1 System / Model Description

**Template M-1: Architecture overview**
```
The overall architecture of ____ is illustrated in Figure X.
It consists of ____ main components: (1) ____, which ____;
(2) ____, which ____; and (3) ____, which ____.
```

**Template M-2: Workflow description**
```
The workflow of ____ proceeds as follows. First, ____. Next, ____.
Then, ____. Finally, ____.
```

**Template M-3: Algorithm description**
```
Algorithm 1 presents the pseudocode of ____. The algorithm takes ____
as input and produces ____ as output. At each iteration, it ____.
The key difference from prior methods is ____.
```

### 3.2 Data Description

**Template M-4: Data source**
```
We collected data from ____ between ____ and ____.
The dataset comprises ____ samples/records, each containing ____.
```

**Template M-5: Preprocessing**
```
Raw data were preprocessed through the following steps:
(1) ____, to remove ____; (2) ____, to normalize ____;
(3) ____, to transform ____. After preprocessing, the dataset
contained ____ valid samples.
```

### 3.3 Experimental Setup

**Template M-6: Implementation details**
```
____ was implemented in ____ (version ____) using the ____ framework.
All experiments were conducted on a machine with ____ CPU,
____ GPU (____ GB memory), and ____ GB RAM.
```

**Template M-7: Training configuration**
```
We trained ____ using the ____ optimizer with an initial learning
rate of ____. We applied a ____ learning rate schedule and a
batch size of ____. Training ran for ____ epochs, taking
approximately ____ minutes per epoch.
```

**Template M-8: Baselines**
```
We compare ____ against the following baselines:
- ____: a classic approach that ____.
- ____: a recent method proposed by ____ (YEAR), which ____.
- ____: the current state-of-the-art on ____.
```

**Template M-9: Evaluation metrics**
```
Performance is assessed using the following metrics:
- ____, defined as ____, which measures ____.
- ____, computed as ____, which reflects ____.
```

**Template M-10: Experimental design**
```
Participants were randomly assigned to either the ____ condition
(n = ____) or the ____ condition (n = ____). The experiment lasted
____ weeks, with assessments at ____ time points.
```

---

## Part 4: Results

### 4.1 Presenting Results

**Template R-1: Introducing a figure**
```
Figure X shows the ____ of ____ on ____. As can be seen, ____
increased/decreased with ____.
```

**Template R-2: Reporting quantitative results**
```
____ achieved a ____ of ____ on ____, outperforming ____
by ____%. Table X summarizes the results across all metrics.
```

**Template R-3: Reporting statistical tests**
```
A ____ test revealed a significant difference between ____
(Mean = ____, SD = ____) and ____ (Mean = ____, SD = ____),
t(__) = ____, p ____ ____.
```

**Template R-4: Describing trends**
```
We observed a ____ trend: as ____ increased from ____ to ____,
____ increased/decreased monotonically/stabilized/fluctuated.
```

**Template R-5: Reporting non-significant results**
```
No significant difference was found between ____ and ____
on ____ (p = ____), suggesting that ____ does not ____.
```
> 用法：不显著的结果也值得报告！这本身就是信息。

### 4.2 Ablation Studies (CS/AI specific)

**Template R-6: Ablation overview**
```
To assess the contribution of each component, we conducted ablation
studies by removing individual modules from the full model.
```

**Template R-7: Ablation results**
```
As shown in Table X, removing ____ caused a ____% drop in ____,
indicating its critical contribution. In contrast, removing ____
had a relatively minor effect (____% drop), suggesting ____.
```

### 4.3 Qualitative Analysis

**Template R-8: Error analysis**
```
We categorized the errors made by ____ into ____ types:
(1) ____ (____% of errors), characterized by ____;
(2) ____ (____%), typically involving ____.
```

**Template R-9: Case study**
```
Figure X presents a representative case where ____.
In this case, ____ was ____, leading to ____.
This illustrates that ____.
```

---

## Part 5: Discussion

### 5.1 Summarizing Key Findings

**Template D-1: Recap**
```
The present study yielded several key findings.
First, ____. Second, ____. Third, ____.
```

### 5.2 Comparing with Literature

**Template D-2: Consistent with prior work**
```
Consistent with ____ (YEAR), our results indicate that ____.
This further supports the view that ____ and suggests that
this effect is robust across ____.
```

**Template D-3: In contrast to prior work**
```
In contrast to ____ (YEAR), who reported ____, we found ____.
A possible explanation for this discrepancy is ____
(e.g., differences in sample characteristics, methodology, or context).
```

**Template D-4: Extending prior work**
```
Our findings extend those of ____ (YEAR) by demonstrating that ____.
While their work established ____, we show that ____ additionally ____.
```

### 5.3 Interpretation

**Template D-5: Explaining findings**
```
One possible interpretation of this finding is that ____.
Alternatively, ____ may account for ____.
```
> 用法：注意用 "possible"、"may"——不要用 "proves" 或 "demonstrates"。

**Template D-6: Mechanism**
```
These findings suggest a potential mechanism: ____ leads to ____,
which in turn ____. This is consistent with ____ theory,
which posits that ____.
```

### 5.4 Implications

**Template D-7: Theoretical implications**
```
This study contributes to the ____ literature by ____.
Theoretically, our findings (1) provide evidence for ____,
(2) extend ____ theory to the context of ____, and
(3) suggest that ____ moderates the relationship between ____ and ____.
```

**Template D-8: Practical implications**
```
These findings have several practical implications.
For ____, we recommend ____. For ____, our results suggest ____.
```

### 5.5 Limitations & Future Work

**Template D-9: Acknowledging limitations**
```
Several limitations of this study should be noted.
First, the sample was ____, which may limit generalizability.
Second, ____ was measured using ____, which may not fully capture ____.
Third, the study duration of ____ may be insufficient to detect ____.
```

**Template D-10: Future directions**
```
Future work could address these limitations by:
(1) replicating this study with ____;
(2) employing ____ to measure ____ more precisely;
(3) conducting a longitudinal study to examine ____.
Additionally, future research could explore ____.
```

**Template D-11: Ending with open possibilities**
```
We hope that our work will inspire further research on ____,
particularly in ____ and ____.
```

---

## Part 6: Abstract (English)

### 6.1 Structured Abstract Template (5 elements)

```
____ is a critical challenge in ____. (Background, 1-2 sentences)
However, ____ remains underexplored. (Gap, 1 sentence)
In this paper, we propose/investigate ____. (Purpose, 1 sentence)
Through ____, we evaluate/demonstrate that ____, achieving ____
on ____. (Methods + Results, 2-3 sentences)
These findings suggest ____. (Conclusion, 1 sentence)
```

### 6.2 CS/AI Abstract Template

```
We present ____, a ____ for ____. ____ addresses the challenge of
____ by ____. We evaluate ____ on ____ benchmark datasets, where it
achieves ____, outperforming ____ by ____%. Ablation studies reveal
that ____ contributes most significantly to the performance gains.
Our results demonstrate that ____. Code and data are available at ____.
```

---

## Part 7: CS/AI Paper Specific Templates

### Algorithm / Model

**Template CS-E-1: Model description**
```
Our proposed ____ consists of ____ modules: ____, ____, and ____.
The ____ module encodes ____, the ____ module processes ____,
and the ____ module decodes ____. The architecture is illustrated
in Figure X.
```

**Template CS-E-2: Complexity**
```
The time complexity of our approach is O(____), compared to O(____)
for ____. The space complexity is O(____). This efficiency gain
comes from ____.
```

### Experiments

**Template CS-E-3: Datasets**
```
We evaluate our method on ____ benchmark datasets:
- ____: ____ samples across ____ classes, used for ____.
- ____: ____ instances, focusing on ____.
For each dataset, we split the data into training (____%),
validation (____%), and test (____%) sets.
```

**Template CS-E-4: Baselines**
```
We compare ____ against the following baselines:
(1) ____ (YEAR): a ____-based method that ____;
(2) ____ (YEAR): a ____ approach using ____;
(3) ____ (YEAR): the current SOTA on ____, based on ____.
```

**Template CS-E-5: Training details**
```
We use the ____ optimizer with β1 = ____, β2 = ____.
The initial learning rate is ____, with a ____ decay schedule.
We use a batch size of ____ and train for ____ epochs.
All experiments run on a single NVIDIA ____ GPU (____ GB).
```

### Results & Analysis

**Template CS-E-6: Main results table**
```
Table X presents the main results. Our method achieves a ____ of ____
on ____, surpassing the strongest baseline (____) by ____%.
Notably, ____ outperforms ____ on ____ of the ____ benchmarks.
```

**Template CS-E-7: Ablation analysis**
```
Table X reports the ablation results. Removing ____ degrades ____
by ____%, confirming its critical role. Removing ____ results in a
____% drop, which is smaller but still notable. The full model
consistently outperforms all ablated variants.
```

**Template CS-E-8: Error / failure analysis**
```
We analyze the failure cases of ____ on ____. The errors fall into
three categories: (1) ____, where ____; (2) ____, where ____;
and (3) ____, where ____. Addressing ____ would likely yield the
largest improvement.
```

**Template CS-E-9: Significance testing**
```
We conduct a paired t-test (or Wilcoxon signed-rank test) to verify
that the improvement of ____ over ____ is statistically significant.
The results confirm significance at the ____ level (p < ____).
```

**Template CS-E-10: Efficiency comparison**
```
We also compare the inference/efficiency of ____ against baselines.
As shown in Table X, ____ achieves ____× speedup over ____,
while maintaining comparable ____.
```

### Positioning & Contribution

**Template CS-E-11: Contribution summary**
```
In summary, this work makes the following contributions:
- We propose ____, a novel ____ for ____.
- We demonstrate through extensive experiments on ____ that ____
  achieves state-of-the-art performance, improving over ____ by ____%.
- We conduct ablation studies and analysis to understand ____,
  revealing that ____.
```

**Template CS-E-12: Distinguishing from prior work**
```
Our work differs from ____ in several key aspects.
First, while ____ uses ____, we adopt ____, which enables ____.
Second, ____ evaluates on ____, whereas we test on ____ datasets
covering ____ scenarios. Third, our method requires ____,
compared to ____ which needs ____.
```

---

## Part 8: Common Transition & Connective Phrases

### 8.1 Adding information
- "Furthermore, ____"
- "In addition, ____"
- "Moreover, ____"
- "Additionally, ____"
- "Notably, ____" (for particularly important additions)

### 8.2 Contrasting
- "However, ____" (most common, versatile)
- "In contrast, ____" (sharp contrast)
- "On the other hand, ____" (different perspective)
- "Nevertheless, ____" (despite the previous point)
- "Conversely, ____" (opposite relationship)

### 8.3 Cause and effect
- "Therefore, ____"
- "As a result, ____"
- "Consequently, ____"
- "This finding suggests that ____" (NOT "proves that")
- "This may be due to ____" (when unsure of exact cause)

### 8.4 Summarizing
- "Taken together, ____"
- "In summary, ____"
- "Overall, ____"
- "Collectively, these results indicate that ____"

### 8.5 Hedging (softening claims — CRITICAL for academic writing)
```
"It is possible that ____"
"This finding suggests that ____"                (NOT "proves")
"____ appears to ____"                           (NOT "is")
"One potential explanation is ____"
"These results may indicate that ____"
"Caution should be exercised in interpreting ____"
```

> ⚠️ **为什么缓和语气很重要？** 中国学生常犯的错误是语气太绝对：用 "prove"（证明）而不是 "suggest"（表明），用 "is" 而不是 "may be"。学术写作中，很少有发现是绝对确定的——承认不确定性是严谨的表现，不是弱点。
