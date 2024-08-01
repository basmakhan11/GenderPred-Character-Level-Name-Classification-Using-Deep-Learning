# GenderPred-Character-Level-Name-Classification-Using-Deep-Learning


This project uses deep learning and machine learning techniques to classify the gender of Brazilian names based on their character sequences. The models are trained on a large dataset of names and can predict whether a given name is typically male or female with high accuracy. The project demonstrates the power of character-level processing in natural language tasks.

## Key Features
- **Character-Level Input**: The model processes names as sequences of characters rather than treating them as whole words, allowing it to capture subtle patterns in name structures.
- **Multiple Deep Learning Models**: The project includes several models—CNN, MLP, RNN, BiLSTM, and GRU—to compare performance and robustness across different neural network architectures.
- **Open Dataset**: The dataset used is publicly available, allowing for easy reproduction of results and further experimentation.
- **Pre-trained Models**: Links to pre-trained models are provided for quick deployment and testing without needing to train from scratch.

## Dataset
The dataset consists of Brazilian names labeled with gender. It can be downloaded directly using the following Python code:

```python
import requests

url = "https://data.brasil.io/dataset/genero-nomes/nomes.csv.gz"
filename = url.split("/")[-1]
with open(filename, "wb") as f:
    r = requests.get(url)
    f.write(r.content)
