# Evaluation Metrics Table

The following table presents the evaluation metrics for three different language models: **Alpaca-LoRA-13B**, **LLAMA3**, and **Vicuna-13B**. These metrics provide insights into the performance of each model across various categories, such as University, Musical Work, Airport, Building, Athlete, Politician, Company, Celestial Body, Astronaut, Comics Character, Means of Transportation, Monument, Food, Written Work, Sports Team, City, Artist, Scientist, and Film. The evaluation metrics include average precision, average recall, average F1 score, average ontological confidence, and various types of hallucinations (subjective, relational, and objective).

### Combined Performance Metrics for LLM Models
| LLM Name           | Evaluation Metrics | avg_precision | avg_recall | avg_f1 | avg_onto_conf| avg_rel_halluc | avg_sub_halluc | avg_obj_halluc |
|--------------------|--------------------|---------------|------------|--------|--------------|----------------|----------------|----------------|
|LLama 3-8B          | University         | 0.77          | 0.55       | 0.62   | 0.92         | 0.08           | 0.00           | 0.03           |
|                    | Musicalwork        | 0.42          | 0.39       | 0.40   | 0.97         | 0.03           | 0.43           | 0.26           |
|                    | Airport            | 0.53          | 0.40       | 0.44   | 0.96         | 0.04           | 0.00           | 0.11           |
|                    | Building           | 0.62          | 0.55       | 0.57   | 0.99         | 0.01           | 0.00           | 0.05           |
|                    | Athlete            | 0.66          | 0.60       | 0.62   | 1.00         | 0.00           | 0.00           | 0.10           |
|                    | Politician         | 0.63          | 0.59       | 0.60   | 0.98         | 0.02           | 0.03           | 0.10           |
|                    | Company            | 0.69          | 0.58       | 0.61   | 0.99         | 0.01           | 0.10           | 0.20           |
|                    | Celestialbody      | 0.81          | 0.80       | 0.80   | 1.00         | 0.00           | 0.01           | 0.31           |
|                    | Astronaut          | 0.71          | 0.64       | 0.67   | 0.96         | 0.04           | 0.01           | 0.22           |
|                    | Comicscharacter    | 0.52          | 0.51       | 0.50   | 1.00         | 0.00           | 0.42           | 0.07           |
|                    | Meanoftransportation | 0.58        | 0.45       | 0.49   | 0.98         | 0.02           | 0.00           | 0.11           |
|                    | Monument           | 0.39          | 0.38       | 0.38   | 1.00         | 0.00           | 0.00           | 0.14           |
|                    | Food               | 0.68          | 0.64       | 0.65   | 0.99         | 0.01           | 0.02           | 0.06           |
|                    | Writtenwork        | 0.81          | 0.78       | 0.78   | 0.99         | 0.01           | 0.06           | 0.14           |
|                    | Sportsteam         | 0.71          | 0.68       | 0.69   | 1.00         | 0.00           | 0.03           | 0.02           |
|                    | City               | 0.19          | 0.20       | 0.19   | 1.00         | 0.00           | 0.03           | 0.62           |
|                    | Artist             | 0.44          | 0.36       | 0.38   | 0.98         | 0.02           | 0.00           | 0.04           |
|                    | Scientist          | 0.74          | 0.70       | 0.71   | 0.98         | 0.02           | 0.01           | 0.20           |
|                    | Film               | 0.46          | 0.42       | 0.43   | 0.99         | 0.01           | 0.00           | 0.14           |
|--------------------|--------------------|---------------|------------|--------|--------------|----------------|----------------|----------------|
|                    | **Average**        | 0.58          | 0.52       | 0.55   | 0.97         | 0.02           | 0.07           | 0.15           |
| -------------------- | -------------------- | --------------- | ------------ | -------- | --------------- | ---------------- | ---------------- | ---------------- |
| Mistral              | University           | 0.75            | 0.59         | 0.65     | 0.95            | 0.05             | 0.00             | 0.02             |
|                      | Musicalwork          | 0.36            | 0.33         | 0.34     | 0.96            | 0.04             | 0.46             | 0.22             |
|                      | Airport              | 0.57            | 0.47         | 0.50     | 0.98            | 0.02             | 0.01             | 0.12             |
|                      | Building             | 0.66            | 0.58         | 0.61     | 0.99            | 0.01             | 0.00             | 0.06             |
|                      | Athlete              | 0.62            | 0.52         | 0.55     | 0.97            | 0.03             | 0.00             | 0.11             |
|                      | Politician           | 0.66            | 0.56         | 0.59     | 0.91            | 0.09             | 0.02             | 0.12             |
|                      | Company              | 0.62            | 0.50         | 0.54     | 0.93            | 0.07             | 0.11             | 0.16             |
|                      | Celestialbody        | 0.78            | 0.78         | 0.77     | 0.99            | 0.01             | 0.00             | 0.29             |
|                      | Astronaut            | 0.71            | 0.67         | 0.68     | 0.99            | 0.01             | 0.00             | 0.21             |
|                      | Comicscharacter      | 0.54            | 0.56         | 0.55     | 0.99            | 0.01             | 0.58             | 0.15             |
|                      | Meanoftransportation | 0.51            | 0.40         | 0.44     | 0.97            | 0.03             | 0.01             | 0.09             |
|                      | Monument             | 0.34            | 0.35         | 0.34     | 1.00            | 0.00             | 0.00             | 0.05             |
|                      | Food                 | 0.68            | 0.65         | 0.66     | 0.98            | 0.02             | 0.00             | 0.06             |
|                      | Writtenwork          | 0.75            | 0.70         | 0.71     | 1.00            | 0.00             | 0.05             | 0.15             |
|                      | Sportsteam           | 0.73            | 0.65         | 0.68     | 0.97            | 0.03             | 0.03             | 0.02             |
|                      | City                 | 0.20            | 0.18         | 0.19     | 0.99            | 0.01             | 0.02             | 0.49             |
|                      | Artist               | 0.43            | 0.31         | 0.34     | 0.95            | 0.05             | 0.00             | 0.06             |
|                      | Scientist            | 0.77            | 0.73         | 0.74     | 0.99            | 0.01             | 0.00             | 0.19             |
|                      | Film                 | 0.44            | 0.40         | 0.42     | 0.99            | 0.01             | 0.01             | 0.12             |
| -------------------- | -------------------- | --------------- | ------------ | -------- | --------------  | ---------------- | ---------------- | ---------------- |
|                      | **Average**          | 0.55            | 0.49         | 0.51     | 0.97            | 0.03             | 0.10             | 0.14             |
|--------------------|--------------------|---------------|------------|--------|--------------|----------------|----------------|---------------|
| Alpaca-LoRA-13B    | University         | 0.29          | 0.16       | 0.20   | 0.89         | 0.11           | 0.13           | 0.26          |
|                    | Musicalwork        | 0.18          | 0.15       | 0.15   | 0.85         | 0.15           | 0.32           | 0.33          |
|                    | Airport            | 0.28          | 0.18       | 0.20   | 0.94         | 0.06           | 0.12           | 0.45          |
|                    | Building           | 0.35          | 0.27       | 0.29   | 0.93         | 0.07           | 0.17           | 0.32          |
|                    | Athlete            | 0.38          | 0.30       | 0.32   | 0.94         | 0.06           | 0.11           | 0.27          |
|                    | Politician         | 0.39          | 0.27       | 0.30   | 0.92         | 0.08           | 0.15           | 0.38          |
|                    | Company            | 0.35          | 0.21       | 0.25   | 0.95         | 0.05           | 0.17           | 0.44          |
|                    | Celestialbody      | 0.52          | 0.44       | 0.47   | 0.96         | 0.04           | 0.12           | 0.49          |
|                    | Astronaut          | 0.34          | 0.21       | 0.25   | 0.87         | 0.13           | 0.08           | 0.58          |
|                    | Comicscharacter    | 0.52          | 0.41       | 0.45   | 0.93         | 0.07           | 0.62           | 0.42          |
|                    | Meanoftransportation | 0.13        | 0.09       | 0.10   | 0.97         | 0.03           | 0.18           | 0.36          |
|                    | Monument           | 0.11          | 0.07       | 0.08   | 0.97         | 0.03           | 0.13           | 0.31          |
|                    | Food               | 0.38          | 0.30       | 0.31   | 0.92         | 0.08           | 0.12           | 0.26          |
|                    | Writtenwork        | 0.39          | 0.35       | 0.36   | 0.90         | 0.10           | 0.20           | 0.50          |
|                    | Sportsteam         | 0.41          | 0.28       | 0.31   | 0.90         | 0.10           | 0.11           | 0.24          |
|                    | City               | 0.10          | 0.09       | 0.09   | 0.96         | 0.04           | 0.07           | 0.68          |
|                    | Artist             | 0.35          | 0.22       | 0.26   | 0.83         | 0.17           | 0.07           | 0.26          |
|                    | Scientist          | 0.42          | 0.33       | 0.34   | 0.92         | 0.08           | 0.14           | 0.43          |
|                    | Film               | 0.18          | 0.14       | 0.15   | 0.82         | 0.18           | 0.08           | 0.33          |
|--------------------|--------------------|---------------|------------|--------|--------------|----------------|----------------|---------------|
|                    | **Average**        | 0.27          | 0.23       | 0.25   | 0.91         | 0.09           | 0.16           | 0.38          |
|--------------------|------------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
| Vicuna             | University             | 0.31          | 0.19       | 0.23   | 0.92          | 0.08           | 0.11           | 0.21           |
|                    | Musicalwork            | 0.20          | 0.18       | 0.18   | 0.89          | 0.11           | 0.32           | 0.27           |
|                    | Airport                | 0.33          | 0.24       | 0.27   | 0.92          | 0.08           | 0.03           | 0.27           |
|                    | Building               | 0.48          | 0.33       | 0.38   | 0.98          | 0.02           | 0.02           | 0.22           |
|                    | Athlete                | 0.33          | 0.26       | 0.29   | 0.92          | 0.08           | 0.01           | 0.13           |
|                    | Politician             | 0.39          | 0.28       | 0.32   | 0.89          | 0.11           | 0.11           | 0.29           |
|                    | Company                | 0.49          | 0.37       | 0.41   | 1.00          | 0.00           | 0.09           | 0.36           |
|                    | Celestialbody          | 0.48          | 0.46       | 0.46   | 0.97          | 0.03           | 0.05           | 0.46           |
|                    | Astronaut              | 0.40          | 0.28       | 0.32   | 0.87          | 0.13           | 0.06           | 0.28           |
|                    | Comicscharacter        | 0.41          | 0.41       | 0.40   | 0.97          | 0.03           | 0.64           | 0.28           |
|                    | Meanoftransportation   | 0.22          | 0.17       | 0.18   | 0.94          | 0.06           | 0.14           | 0.41           |
|                    | Monument               | 0.04          | 0.05       | 0.05   | 0.94          | 0.06           | 0.18           | 0.31           |
|                    | Food                   | 0.43          | 0.39       | 0.39   | 0.94          | 0.06           | 0.05           | 0.20           |
|                    | Writtenwork            | 0.40          | 0.34       | 0.36   | 0.92          | 0.08           | 0.12           | 0.33           |
|                    | Sportsteam             | 0.52          | 0.38       | 0.42   | 0.91          | 0.09           | 0.04           | 0.11           |
|                    | City                   | 0.12          | 0.12       | 0.12   | 0.98          | 0.02           | 0.04           | 0.67           |
|                    | Artist                 | 0.30          | 0.21       | 0.23   | 0.89          | 0.11           | 0.03           | 0.13           |
|                    | Scientist              | 0.52          | 0.43       | 0.46   | 0.95          | 0.05           | 0.05           | 0.30           |
|                    | Film                   | 0.23          | 0.19       | 0.20   | 0.94          | 0.06           | 0.30           | 0.19           |
|--------------------|------------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
|                    | **Average**            | 0.34          | 0.27       | 0.30   | 0.93          | 0.07           | 0.12           | 0.28           |
|--------------------|------------------------|---------------|------------|--------|---------------|----------------|----------------|----------------|
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
