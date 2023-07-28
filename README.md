# LLM-Dataset Analysis
This records analysis of dataset composition of LLM works.

## Foundation Models
### LLAMA2
#### RLHF Dataset
| Dataset                    | Num. of Comparisons | Num. of Prompt | Avg. # Turns per Dialogue | Avg. # Tokens per Example | Avg. # Tokens in Prompt | Avg. # Tokens in Response |
|----------------------------|---------------------|------------|---------------------------|---------------------------|-------------------------|---------------------------|
| Anthropic Helpful          | 122,387             |122,387     | 3.0                       | 251.5                     | 17.7                    | 88.4                      |
| Anthropic Harmless         | 43,966              |43,966      | 3.0                       | 152.5                     | 15.7                    | 46.4                      |
| OpenAI Summarize           | 176,625             |176,625     | 1.0                       | 371.1                     | 336.0                   | 35.1                      |
| OpenAI WebGPT              | 13,333              |13,333      | 1.0                       | 237.2                     | 48.3                    | 188.9                     |
| StackExchange              | 1,038,480           |1,038,480   | 1.0                       | 440.2                     | 200.1                   | 240.2                     |
| Stanford SHP               | 74,882              |74,882      | 1.0                       | 338.3                     | 199.5                   | 138.8                     |
| Synthetic GPT-J            | 33,139              |33,139      | 1.0                       | 123.3                     | 13.0                    | 110.3                     |
| Meta (Safety & Helpfulness)| 1,418,091           |            | 3.9                       | 798.5                     | 31.4                    | 234.1                     |
| Total                      | 2,919,326           |1,502,135   | 1.6                       | 595.7                     | 108.2                   | 216.9                     |
