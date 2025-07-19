# 🧠 Text-to-Triple Dataset and Evaluation Resources

This repository contains benchmark datasets, ontology files, LLM-generated responses, and evaluation results used for extracting and evaluating RDF triples from text using large language models.

---

## 📦 Data Structure Overview

---

### 🗂️ `wikidata_tekgen` – Wikidata-TekGen Dataset

* **Ontologies (10)**: [ontologies](data/wikidata/ontologies) – Ontology files used for triple validation.
* **Ground Truth**: [ground\_truth](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/ground_truth) – Gold standard triples for evaluation.
* **Prompts**: [prompts](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/prompts)) – Natural language prompts generated for test samples.

#### 📊 Baselines – Evaluation Results and LLM Responses

##### 🔹 Alpaca-LoRA-13B

* [Alpaca Data](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Alpaca-LoRA-13B))

  * [llm\_responses](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Alpaca-LoRA-13B/llm_response)) – Raw responses + extracted triples
  * [eval\_metrics](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Alpaca-LoRA-13B/evaluation_statistics/baseline_statistics)) – Ontology-level + aggregated results

##### 🔹 Vicuna-13B

* [Vicuna Data](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Vicuna-13B))

  * [llm\_responses](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Vicuna-13B/llm_response)) – Raw responses + extracted triples
  * [eval\_metrics](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Vicuna-13B/evaluation_statistics/baseline_statistics)) – Ontology-level + aggregated results

##### 🔹 Llama-8B

* [Llama Data](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Llama-8B))

  * [llm\_responses](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Llama-8B/llm_response)) – Raw responses + extracted triples
  * [eval\_metrics](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Llama-8B/evaluation_statistics)) – Ontology-level + aggregated results

##### 🔹 Mistral-7B

* [Mistral Data](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Mistral-7B))

  * [llm\_responses](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Mistral-7B/llm_response)) – Raw responses + extracted triples
  * [eval\_metrics](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/baselines/Mistral-7B/evaluation_statistics)) – Ontology-level + aggregated results

---

### 🗂️ `dbpedia_webnlg` – [DBpedia Dataset](data/dbpedia)

* **Ontologies (19)**: [ontologies](data/dbpedia/ontologies) – DBpedia ontologies for triple evaluation.
* **Ground Truth**: [ground\_truth](data/dbpedia/ground_truth) – Gold standard triple data.
* **Prompts**: [prompts](data/dbpedia/input_prompts/cot_prompts) – Prompt files for LLM-based triple generation.

#### 📊 Baselines – Evaluation Results and LLM Responses

##### 🔹 Alpaca-LoRA-13B

* [Alpaca Data](data/dbpedia/baselines/Alpaca-LoRA-13B)

  * [llm\_responses](data/dbpedia/baselines/Alpaca-LoRA-13B/llm_responses)
  * [eval\_metrics](data/dbpedia/baselines/Alpaca-LoRA-13B/eval_metrics)

##### 🔹 Vicuna-13B

* [Vicuna Data](data/dbpedia/baselines/Vicuna-13B)

  * [llm\_responses](data/dbpedia/baselines/Vicuna-13B/llm_responses)
  * [eval\_metrics](data/dbpedia/baselines/Vicuna-13B/eval_metrics)

---

## 🧪 How to Use

This structure supports:

* Reproducing experiments using the provided prompts and ground truths.
* Comparing LLM outputs against baseline evaluations.
* Loading ontologies and results into custom tools or visualizers.

---

## 📁 Folder Tree (Example)

```
data/
├── dbpedia/
│   ├── ontologies/
│   ├── ground_truth/
│   ├── input_prompts/
│   └── baselines/
│       ├── Alpaca-LoRA-13B/
│       └── Vicuna-13B/
└── wikidata/
    ├── ontologies/
    ├── ground_truth/
    ├── input_prompts/
    └── baselines/
        ├── Alpaca-LoRA-13B/
        └── Vicuna-13B/
```
