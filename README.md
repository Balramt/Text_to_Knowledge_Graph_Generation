# LLM Triple Extraction Pipeline (LLaMA 3)

This repository runs a pipeline to generate (subject, relation, object) triples from natural language prompts using the **Meta-LLaMA-3-8B** model. The generated triples are later evaluated using ontology-based or contrastive reasoning tools.

---

## 📁 Data

The `data` folder contains benchmark datasets and prompt files. There are two primary datasets:

* **wikidata\_tekgen**: A subset of TekGen adapted to Wikidata-style triples.
* **dbpedia\_webnlg**: A version of WebNLG adapted for DBpedia-style entities.

---

## 📂 Prompt Files

Each dataset has associated prompt files in `.jsonl` format, located here:

* **Prompts**: [`data/wikidata`](https://github.com/Balramt/Text_to_Knowledge_Graph_Generation/tree/main/data/wikidata/prompts)
* Sample File: [`ont_1_movie_prompts_improved.jsonl`](data/wikidata/input_prompts/cot_prompts/ont_1_movie_prompts_improved.jsonl)

---

## 📤 Output

Model outputs (triples) are saved in JSONL format with the following structure:

```json
{"id": "example_1", "triples": [{"sub": "Titanic", "rel": "directed", "obj": "James Cameron"}]}
```

* Output folder: [`data/wikidata/response_run4/Llama3`](data/wikidata/response_run4/Llama3)

---

## ▶️ Running the Script

Edit the paths and run:

```bash
python generate_llama3_triples.py
```

Script is located at:

* [`generate_llama3_triples.py`](generate_llama3_triples.py)

---

Let me know if you'd like help generating links dynamically (for GitHub Pages, Colab, or external sources), or want to add a section for evaluation notebooks (`.ipynb`).
