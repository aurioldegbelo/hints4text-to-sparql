Experiments on the impact of different types of hints on LLM-based SPARQL query generation on long-tail scientific graphs. The detailed results per experiment are available in the [\experiment folder](/experiments). The structured questions can be accessed in the [\questions folder](/questions).

The following conditions were compared across four models (GPT-4.1, GPT-5.4-mini, GPT-5.4-nano, and GPT-5.5) and three datasets (LamaH-CE, CAMELS-GB, and QUADICA).

# Conditions

|Preset|Schema mode|Contents|
|-|-|-|
|`base`|`small`|Default small schema and general constraints.|
|`c01`|`small`|Baseline graph-hint condition.|
|`c02_ia`|`ner`|NER schema context and CoT-style instruction.|
|`ca`|`full`|Full graph schema with domain/range information.|
|`ca_ia`|`full`|Full schema plus the CoT-style instruction.|
|`ca_ib`|`reasoning_path`|Reasoning-path context using the base prompt.|
|`ca_ic`|`reasoning_path`|Reasoning-path context using the graph-specific prompt.|
|`ca_ia_ic`|`reasoning_path`|Reasoning path, CoT instruction, and graph-specific prompt.|
|`ca_cb_ia_ic`|`reasoning_path`|The previous combination plus query, aggregation, function, and unit hints.|

Schema refers to the extent to which the knowledge graph schema (i.e. its classes and relationships) is exposed to the LLM during the SPARQL generation process. The available schema modes are `full`, `small`, `ner`, `reasoning_path`, and `none`.

# Questions 

to be added

# Results

## Execution time

<img width="3562" height="1763" alt="plot_ET_LamaH_CE" src="https://github.com/user-attachments/assets/c03bf723-0581-4f57-8a5d-e55cab9b947f" />
<img width="3562" height="1763" alt="plot_ET_CAMELS_GB" src="https://github.com/user-attachments/assets/51e1d3d1-ee74-4a37-a794-c56b563f0852" />
<img width="3563" height="1763" alt="plot_ET_QUADICA" src="https://github.com/user-attachments/assets/3350df14-f382-4c2d-901f-36d8370612f1" />

## Syntactic validity


<img width="3560" height="1763" alt="plot_VS_LamaH_CE" src="https://github.com/user-attachments/assets/10259683-d426-4fe5-a3f9-c6b002778a6e" />
<img width="3560" height="1763" alt="plot_VS_CAMELS_GB" src="https://github.com/user-attachments/assets/be234bca-fccb-4f4c-8ffa-f5d28e85859c" />
<img width="3560" height="1763" alt="plot_VS_QUADICA" src="https://github.com/user-attachments/assets/6f3d516b-72d1-448d-9628-d00b385402a3" />

## Query correctness


<img width="3560" height="1763" alt="plot_AAF_LamaH_CE" src="https://github.com/user-attachments/assets/9a496692-47dc-401f-9f25-c05890d203e3" />
<img width="3560" height="1763" alt="plot_AAF_CAMELS_GB" src="https://github.com/user-attachments/assets/bd1468cd-373b-4ab2-bdeb-d1449ae3a170" />
<img width="3560" height="1763" alt="plot_AAF_QUADICA" src="https://github.com/user-attachments/assets/6cf8d6c8-23af-4439-9b28-ef38aeb70b78" />

