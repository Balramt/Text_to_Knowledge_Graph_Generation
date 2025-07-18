# Evaluation Metrics Table

The following table presents the evaluation metrics for three different language models: **Alpaca-LoRA-13B**, **LLAMA3**, **Mistral** and **Vicuna-13B**. These metrics provide insights into the performance of each model across various categories, such as Movie, Music, Sport, Book, Military, Computer, Space, Politics, Nature, and Culture. The evaluation metrics include average precision, average recall, average F1 score, average ontological confidence, and various types of hallucinations (subjective and objective).


| LLM Name           | Evaluation Metrics | avg_precision | avg_recall | avg_f1 | avg_onto_conf | avg_rel_halluc | avg_sub_halluc | avg_obj_halluc |
|--------------------|--------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
| LLAMA3             | Movie              | 0.45          | 0.21       | 0.27   | 0.55          | 0.45           | 0.28           | 0.28           |
|                    | Music              | 0.48          | 0.27       | 0.32   | 0.67          | 0.33           | 0.13           | 0.22           |
|                    | Sport              | 0.68          | 0.56       | 0.60   | 0.82          | 0.18           | 0.15           | 0.10           |
|                    | Book               | 0.43          | 0.30       | 0.34   | 0.67          | 0.33           | 0.11           | 0.21           |
|                    | Military           | 0.38          | 0.37       | 0.37   | 0.68          | 0.32           | 0.15           | 0.24           |
|                    | Computer           | 0.48          | 0.34       | 0.37   | 0.52          | 0.48           | 0.14           | 0.06           |
|                    | Space              | 0.76          | 0.69       | 0.70   | 0.70          | 0.30           | 0.15           | 0.05           |
|                    | Politics           | 0.56          | 0.53       | 0.53   | 0.69          | 0.31           | 0.13           | 0.13           |
|                    | Nature             | 0.51          | 0.46       | 0.47   | 0.74          | 0.26           | 0.12           | 0.12           |
|                    | Culture            | 0.63          | 0.64       | 0.63   | 0.68          | 0.32           | 0.15           | 0.40           |
|--------------------|--------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
|                    | **Average**        | 0.54          | 0.44       | 0.46   | 0.67          | 0.33           | 0.15           | 0.18           |
|--------------------|--------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
| Mistral            | Movie              | 0.37          | 0.27       | 0.29   | 0.77          | 0.23           | 0.19           | 0.10           |
|                    | Music              | 0.41          | 0.32       | 0.34   | 0.82          | 0.18           | 0.13           | 0.12           |
|                    | Sport              | 0.53          | 0.46       | 0.47   | 0.83          | 0.17           | 0.14           | 0.10           |
|                    | Book               | 0.37          | 0.31       | 0.32   | 0.78          | 0.22           | 0.08           | 0.12           |
|                    | Military           | 0.40          | 0.41       | 0.40   | 0.86          | 0.14           | 0.11           | 0.16           |
|                    | Computer           | 0.39          | 0.32       | 0.33   | 0.72          | 0.28           | 0.08           | 0.02           |
|                    | Space              | 0.73          | 0.70       | 0.70   | 0.88          | 0.12           | 0.10           | 0.04           |
|                    | Politics           | 0.40          | 0.41       | 0.40   | 0.80          | 0.20           | 0.09           | 0.11           |
|                    | Nature             | 0.42          | 0.39       | 0.39   | 0.86          | 0.15           | 0.08           | 0.09           |
|                    | Culture            | 0.45          | 0.47       | 0.45   | 0.73          | 0.27           | 0.14           | 0.35           |
|--------------------|--------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
|                    | **Average**        | 0.45          | 0.41       | 0.41   | 0.81          | 0.20           | 0.11           | 0.12           |
|--------------------|--------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
| Alpaca-LoRA-13B    | Movie              | 0.28          | 0.14       | 0.17   | 0.92          | 0.08           | 0.25           | 0.24           |
|                    | Music              | 0.33          | 0.19       | 0.22   | 0.91          | 0.09           | 0.18           | 0.24           |
|                    | Sport              | 0.51          | 0.44       | 0.45   | 0.96          | 0.04           | 0.18           | 0.11           |
|                    | Book               | 0.25          | 0.17       | 0.19   | 0.94          | 0.06           | 0.17           | 0.19           |
|                    | Military           | 0.21          | 0.21       | 0.21   | 0.93          | 0.07           | 0.21           | 0.26           |
|                    | Computer           | 0.39          | 0.27       | 0.29   | 0.83          | 0.17           | 0.17           | 0.13           |
|                    | Space              | 0.58          | 0.55       | 0.55   | 0.90          | 0.10           | 0.14           | 0.10           |
|                    | Politics           | 0.22          | 0.21       | 0.21   | 0.90          | 0.10           | 0.19           | 0.15           |
|                    | Nature             | 0.28          | 0.26       | 0.27   | 0.93          | 0.07           | 0.22           | 0.20           |
|                    | Culture            | 0.15          | 0.16       | 0.15   | 0.54          | 0.46           | 0.16           | 0.14           |
|--------------------|--------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
|                    | **Average**        | 0.32          | 0.26       | 0.27   | 0.88          | 0.12           | 0.19           | 0.18           |
|--------------------|--------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
| Vicuna-13B         | Movie              | 0.33          | 0.23       | 0.25   | 0.89          | 0.11           | 0.26           | 0.26           |
|                    | Music              | 0.42          | 0.28       | 0.32   | 0.94          | 0.06           | 0.16           | 0.22           |
|                    | Sport              | 0.57          | 0.52       | 0.52   | 0.85          | 0.15           | 0.22           | 0.13           |
|                    | Book               | 0.31          | 0.25       | 0.26   | 0.92          | 0.08           | 0.16           | 0.23           |
|                    | Military           | 0.24          | 0.25       | 0.24   | 0.80          | 0.20           | 0.19           | 0.26           |
|                    | Computer           | 0.38          | 0.35       | 0.35   | 0.85          | 0.15           | 0.15           | 0.11           |
|                    | Space              | 0.68          | 0.67       | 0.66   | 0.93          | 0.07           | 0.15           | 0.08           |
|                    | Politics           | 0.34          | 0.32       | 0.33   | 0.92          | 0.08           | 0.17           | 0.15           |
|                    | Nature             | 0.25          | 0.27       | 0.25   | 0.68          | 0.04           | 0.10           | 0.14           |
|                    | Culture            | 0.31          | 0.32       | 0.31   | 0.59          | 0.39           | 0.15           | 0.12           |
|--------------------|--------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
|                    | **Average**        | 0.38          | 0.35       | 0.35   | 0.84          | 0.13           | 0.17           | 0.17           |
|--------------------|--------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|

## Models Description

### Alpaca-LoRA-13B
Alpaca-LoRA-13B is a 13 billion parameter language model fine-tuned with the LoRA (Low-Rank Adaptation) technique. This model is designed to perform well on a variety of natural language processing tasks by leveraging a large-scale dataset and fine-tuning to adapt to specific domains and use cases.

### LLAMA3
LLAMA3 is an advanced language model that has been trained to understand and generate human-like text. It has been evaluated across multiple categories to benchmark its performance in terms of precision, recall, F1 score, ontological confidence, and hallucination rates.

### Vicuna-13B
Vicuna-13B is a robust language model evaluated on various domains. It aims to achieve a balance between high performance and low hallucination rates, ensuring reliable and accurate text generation across different contexts.

## Evaluation Metrics
The evaluation metrics used for these models are as follows:
- **avg_precision**: The average precision score across different categories.
- **avg_recall**: The average recall score across different categories.
- **avg_f1**: The average F1 score, which is the harmonic mean of precision and recall.
- **avg_onto_conf**: The average ontological confidence score, indicating the model's confidence in its predictions.
- **avg_sub_halluc**: The average subjective hallucination rate, measuring the frequency of subjective errors.
- **avg_rel_halluc**: The average relational hallucination rate, measuring the frequency of relational errors.
- **avg_obj_halluc**: The average objective hallucination rate, measuring the frequency of objective errors.
