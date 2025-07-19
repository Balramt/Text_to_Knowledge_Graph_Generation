# 🧠 Text to RDF Triple Generator and Knowledge Graph using LLMs (LLaMA 3 / Mistral)

This project provides an **interactive web interface** built with **Dash** for generating RDF-like triples from user-uploaded text prompts using large language models (**LLaMA 3** and **Mistral**). It also offers a **dynamic knowledge graph visualization** of the extracted triples using **Cytoscape**.

---

## 🚀 Features

* **File Upload and Model Selection**: Upload a `.jsonl` prompt file and choose between **LLaMA 3** or **Mistral** for triple generation.
* **Triple Extraction**: Extracts (subject, relation, object) triples from the model's generated output using pattern-based parsing.
* **Knowledge Graph Visualization**: Displays an interactive graph with entities and relationships using `dash_cytoscape`.
* **Table View**: Optionally view the extracted triples in a paginated table.
* **Interactive Elements**: Click nodes and edges to explore details of entities and relationships.

---

## 📦 Requirements

Install dependencies using pip:

```bash
pip install torch transformers dash dash-bootstrap-components dash-cytoscape nltk jsonlines
```

---

## ⚙️ How It Works

### 1. Model Setup

The app allows users to select between:

* `meta-llama/Meta-Llama-3-8B`
* `mistralai/Mistral-7B-Instruct-v0.3`

The models are loaded via HuggingFace’s `transformers` with `torch_dtype=torch.float16` and `device_map="auto"` for GPU acceleration.

### 2. Prompt Processing and Triple Extraction

* Prompts are read from a `.jsonl` file.

* For each prompt, the model generates **two text completions**.

* The completions are parsed using regular expressions to extract triples in the format:

  ```
  relation(subject, object)
  ```

* Outputs are **normalized** using tokenization and lemmatization (`nltk`), and **deduplicated** per prompt.

### 3. Knowledge Graph Construction

* Uses `dash_cytoscape` to generate a **directed, interactive graph**:

  * Nodes represent entities (subjects or objects).
  * Edges represent relations.
  * **Bidirectional edges** are merged and highlighted for clarity.
* Nodes and edges are color-coded using consistent hashing.

---

## 💡 How to Use

1. **Upload Prompt File**:

   * Format: `.jsonl`
   * Each line should look like:

     ```json
     {"id": "sample_001", "prompt": "The movie Titanic was directed by James Cameron."}
     ```

2. **Select a Model**:

   * LLaMA 3 or Mistral 7B

3. **Click "Run Extraction"**:

   * Extracts triples from the first 10 prompts for faster UI response.

4. **Choose Output View**:

   * **Table View**: Shows all extracted triples in a table.
   * **Graph View**: Renders an interactive RDF-style knowledge graph.

5. **Interact with the Graph**:

   * Click nodes and edges to view semantic details in the sidebar.

---

## 🧬 Code Overview

### Core Logic

* `setup_llama_model()` / `setup_mistral_model()`: Loads the selected model with device optimization.
* `extract_test_outputs()`: Retrieves the `Test Output:` block from the LLM response.
* `parse_model_output()`: Uses regex to parse triples in `(rel, sub, obj)` format.
* `clean_triple_component()`: Normalizes and lemmatizes entity/relation strings.
* `triples_to_cytoscape_elements()`: Converts triple list into Cytoscape graph elements.

### Dash Interface

* **Upload Component**: Accepts `.jsonl` files for prompts and optional `.json` ontologies.
* **Model Selector**: Dropdown to pick LLaMA or Mistral.
* **View Switch**: Toggle between Table and Graph modes.
* **Graph Panel**: Interactive knowledge graph with node/edge click handling.
* **Status Panel**: Displays process summary and errors.

---

## ▶️ Launching the App

To run the Dash app locally:

```bash
python app.py
```

Then open your browser at:

```
http://0.0.0.0:8070/
```

> You can modify `app.run()` if needed for deployment or external hosting.

---

## 📌 Notes

* This demo processes **only the first 10 prompts** for performance reasons.
* Extend the logic if you want to process larger files or full batches.
* Requires **GPU** for real-time LLM inference. Quantized models can be used if needed.

---

## 📊 Sample Output

### 📋 Table View

| ID          | Subject | Relation | Object        |
| ----------- | ------- | -------- | ------------- |
| sample\_001 | titanic | directed | james cameron |

### 🧠 Graph View (Interactive)

* Nodes = entities
* Edges = relationships
* Double arrows = bidirectional relations
* Clickable for detailed info

---

## 📜 License

This project is for **research and educational purposes only**.
Please ensure compliance with individual model licenses (e.g., Meta’s LLaMA, Mistral AI).

---

## 🙏 Acknowledgements

* [HuggingFace Transformers](https://huggingface.co/docs/transformers)
* [Meta AI – LLaMA](https://ai.meta.com/llama/)
* [Mistral AI](https://mistral.ai/)
* [Dash by Plotly](https://dash.plotly.com/)

---

Let me know if you want image previews or `requirements.txt` included!
