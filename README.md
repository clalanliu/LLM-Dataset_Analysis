# LLM-Dataset Analysis
This records analysis of dataset composition of LLM works.

## Foundation Models
### Orca (2023/08)
[ORCA](Orca.md)
### Hermes (2023/07)
#### SFT Dataset
| Dataset                   | Num. of Prompt |
| ------------------------- | -------------- |
| GPTeacher                 | 89.3k          |
| GPT4-LLM-Cleaned          | 54.6k          |
| WizardLM-evol-instruct-v2 | 196k           |
| airoboros                 | 9k             |
| unnatural-instruction     | 66k            |
| Code-alpaca               | 20k            |
| Camel-AI math             | 50k            |
| Camel-AI biology          | 20k            |
| Camel-AI physics          | 20k            |
| Camel-AI chemistry        | 20k            |


### LLAMA2 (2023/07)
#### Pretraining Dataset
2T
#### SFT Dataset
27.5k 
#### RLHF Dataset
| Dataset                     | Num. of Comparisons | Num. of Prompt | Avg. # Turns per Dialogue | Avg. # Tokens per Example | Avg. # Tokens in Prompt | Avg. # Tokens in Response |
| --------------------------- | ------------------- | -------------- | ------------------------- | ------------------------- | ----------------------- | ------------------------- |
| Anthropic Helpful           | 122,387             | 122,387        | 3.0                       | 251.5                     | 17.7                    | 88.4                      |
| Anthropic Harmless          | 43,966              | 43,966         | 3.0                       | 152.5                     | 15.7                    | 46.4                      |
| OpenAI Summarize            | 176,625             | 176,625        | 1.0                       | 371.1                     | 336.0                   | 35.1                      |
| OpenAI WebGPT               | 13,333              | 13,333         | 1.0                       | 237.2                     | 48.3                    | 188.9                     |
| StackExchange               | 1,038,480           | 1,038,480      | 1.0                       | 440.2                     | 200.1                   | 240.2                     |
| Stanford SHP                | 74,882              | 74,882         | 1.0                       | 338.3                     | 199.5                   | 138.8                     |
| Synthetic GPT-J             | 33,139              | 33,139         | 1.0                       | 123.3                     | 13.0                    | 110.3                     |
| Meta (Safety & Helpfulness) | 1,418,091           |                | 3.9                       | 798.5                     | 31.4                    | 234.1                     |
| Total                       | 2,919,326           | 1,502,135      | 1.6                       | 595.7                     | 108.2                   | 216.9                     |

### LLAMA
#### Pretraining Dataset
| Dataset       | Sampling Prop. | Epochs | Disk Size |
| ------------- | -------------- | ------ | --------- |
| CommonCrawl   | 67.0%          | 1.10   | 3.3 TB    |
| C4            | 15.0%          | 1.06   | 783 GB    |
| Github        | 4.5%           | 0.64   | 328 GB    |
| Wikipedia     | 4.5%           | 2.45   | 83 GB     |
| Books         | 4.5%           | 2.23   | 85 GB     |
| ArXiv         | 2.5%           | 1.06   | 92 GB     |
| StackExchange | 2.0%           | 1.03   | 78 GB     |
