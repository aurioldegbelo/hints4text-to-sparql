Experiments on the impact of different types of hints on LLM-based SPARQL query generation on long-tail scientific graphs. The detailed results per experiment are available in the [\experiment folder](/experiments). 

The following conditions were compared across four models (GPT-4.1, GPT-5.4-mini, GPT-5.4-nano, and GPT-5.5) and three datasets (LamaH-CE, CAMELS-GB, and QUADICA).

# 🧪 Conditions

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

# ❓ Questions 

Examples of question types, only for the LamaH-CE Dataset, are shown below. The remaining examples can be accessed from the [\questions folder](/questions) folder as well, both in a human-readable format (Excel) and machine-readable format (YAML).

| Spatial Facets and Core Concepts | Question Pattern / Examples                                                                                                                                                                                                                                                                                                                                                                                                             |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Object - Location                | Where is (What is the location of) geographic feature G?<br>OL1: Where is the gauging station “Hohenems” located?<br>OL2: What are the gauging station locations of the five largest catchments by area?                                                                                                                                                                                                                                |
| Object - Boundary                | What is the boundary of geographic feature G?<br>OB1: What is the boundary of the catchment monitored by sensor 1?<br>                                                                                                                                                                                                                                                                                                                  |
| Object - Spatial Properties      | What is the value of this spatial property for geographic feature G?<br>OS1: What is the area of the largest catchment in the dataset? <br>OS2: What are the areas of all catchments in the dataset?                                                                                                                                                                                                                                    |
| Network - Spatial Relationships  | What is the spatial relationship between feature G1 and feature G2?<br>NS1: What is the distance between the gauging stations with the highest and lowest elevations in the dataset?<br>NS2: What are the gauging stations within a 10 km radius of the Gauging Station nr. 1?<br>NS3: Which catchments share a boundary with the catchment that recorded the highest total precipitation between 2012 and 2015?                        |
| Object - Attribute values        | What is the value of this non-spatial property for geographic feature G?<br>OA1: What is the name of the river-based region connected to the gauging station 'Loruens-Aeule'<br>OA2: Which catchment recorded the highest mean precipitation in 2015?<br>OA3: Which catchments recorded total precipitation above 1000 mm in Austria in 2010?<br>OA4: What are the names and elevations of the upstream gauging stations to station 88? |
| Field - Attribute values         | What are attribute values for a field P (at Location L)?<br>FA1: What are the minimum and maximum river flow observed at the Gauging Station 'Garsella'?<br>FA2: What are the minimum and maximum river flow across all gauging stations?<br>FA3: What is the average annual precipitation in Catchment 1 during the period from 2012 to 2015?                                                                                          |
| Event-based - Occurrence time    | When did event E happen?<br>EO1: Which month experienced the highest flow rate in Austria in 2012?<br>EO2: Which years experienced average precipitation below 1400 mm/year in Austria?                                                                                                                                                                                                                                                 |
| Event-Based - Extreme event      | How often did event E happen?<br>EE1: How many frost days were recorded at the 'Bangs' gauging station between 2010 and 2020? (Frost days are defined as days with temperatures below 0°C) <br>                                                                                                                                                                                                                                         |


# 🗂️ Datasets

- LamaH-CE in RDF: https://doi.org/10.5281/zenodo.16948620 

- CAMELS-GB in RDF: https://doi.org/10.5281/zenodo.16950260 

- QUADICA in RDF: https://doi.org/10.5281/zenodo.17290249

# 📊 Results

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

