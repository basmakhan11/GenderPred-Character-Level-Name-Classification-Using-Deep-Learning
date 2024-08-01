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






## References
This repository builds upon significant academic research in the field of name-based gender classification:

Rego, R. C., Silva, V. M. & Fernandes, V. M. (2021). Predicting Gender by First Name Using Character-level Machine Learning. arXiv preprint arXiv:2106.10156 v2.
Rego, R. C., & Silva, V. M. (2021). Predicting gender of Brazilian names using deep learning. arXiv preprint arXiv:2106.10156 v1.

R. C. B. Rego, G. d. S. Nascimento, D. E. d. L. Rodrigues, S. M. Nascimento, & V. M. L. Silva (2023). "Brazilian scientific productivity from a gender perspective during the Covid-19 pandemic: classification and analysis via machine learning," IEEE Latin America Transactions, vol. 21, no. 2, pp. 302-309, doi: 10.1109/TLA.2023.10015223.


## Conclusion
This repository offers a comprehensive toolkit for predicting gender based on first names using advanced machine learning techniques. Whether you are interested in exploring the intricacies of character-level models or need a robust solution for name-based gender prediction, this repository provides everything you need to get started.
