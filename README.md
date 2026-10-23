Experiments about the impact of different types of hints on LLM-based SPARQL query generation on long-tail scientific graphs. 

The following conditions were compared for four models across the three datasets: LamaH-CE, CAMELS-GB and QUADICA.

|Preset|Contents|
|-|-|
|`base`|Default small schema and general constraints.|
|`c01`|Baseline graph-hint condition.|
|`c02_ia`|NER schema context and CoT-style instruction.|
|`ca`|Full graph schema with domain/range information.|
|`ca_ia`|Full schema plus the CoT-style instruction.|
|`ca_ib`|Reasoning-path context using the base prompt.|
|`ca_ic`|Reasoning-path context using the graph-specific prompt.|
|`ca_ia_ic`|Reasoning path, CoT instruction, and graph-specific prompt.|
|`ca_cb_ia_ic`|The previous combination plus query, aggregation, function, and unit hints.|
