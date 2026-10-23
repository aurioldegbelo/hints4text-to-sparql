Experiments about the impact of different types of hints on LLM-based SPARQL query generation on long-tail scientific graphs. 

The following conditions were compared for four models () across the three datasets (LamaH-CE, CAMELS-GB, and QUADICA).

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
