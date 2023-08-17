# Blue and Gray in Palette: 
What Can We Learn from Orca

* **Important note**: Although Orca is good, we should not ignore the fact Orca is a 4.2M dataset, which is 10x larger than other existing datasets. We should always remember this number when we admire the benchmark performance of Orca compared to models trained with other *mediocre* datasets with only hundred thousands samples.



## **Challenges with Existing Methods**

>a *lack of rigorous evaluation resulting in overestimating the small model’s capability as they tend to learn to imitate the style, **but not the reasoning process of LFMs*****.** 



* Simple instructions with limited diversity →  WizardLM’ s complexity + Vicuna’s human-like style
* Limited imitation signals → system prompt
    * System prompt is the key to trigger **Teacher(ChatGPT, GPT4)**, not student model

>The **system message**, placed at the start of the prompt, provides the **LFM** with essential context, guidelines, and other pertinent details.

Not directly related:

* GPT-4 prefers long answers: GPT-4 responses are on an average 1*.*5*×* longer than that of ChatGPT

## Orca **Construction**

* No edge-cutting sampling method. Just sample tasks and samples query in each task
    * Contradict to [Instruction Mining](https://arxiv.org/abs/2307.06290)?
* 5M from Chatgpt, 1M from gpt-4

## Evaluation

>**Replication Note:** We observe that there is a positive bias in GPT-4 evaluation towards the response of the first model in the comparison set

### When a Model Lose: **AGIEval**

* Domain knowledge: tie
* Complex reasoning: tie
* Long context: **ChatGPT has an edge over Orca**
* Geometric reasoning: tie
* LaTeX reasoning: tie

### When a Model Lose: **Big-Bench Hard**

* Entailment and Semantic Understanding: Orca performs better
* Temporal and Spatial Reasoning: Orca performs better
* Causal Judgment: Orca performs better
* Multilingual Understanding: tie
* World Knowledge: Orca performs better (**Why?**)
* Logical and Geometric Reasoning: ChatGPT better
* Table Understanding: ChatGPT better

