# Transfer Learning com VGG16 — Classificação de Rostos Star Wars 🛸

Este projeto é uma adaptação do notebook original de [Transfer Learning com VGG16](https://colab.research.google.com/github/kylemath/ml4a-guides/blob/master/notebooks/transfer-learning.ipynb#scrollTo=XklKIrnaZb3f), que utiliza o dataset **Caltech 101 (101_ObjectCategories)** para demonstrar como aplicar Transfer Learning em tarefas de classificação de imagens.

Neste repositório, substituímos o dataset original por um conjunto de imagens de personagens do universo Star Wars — **Luke Skywalker** e **Obi-Wan Kenobi** — para treinar um classificador binário usando a mesma estrutura de código.

## 📁 Estrutura do Dataset

O dataset está organizado da seguinte forma:

starwars-face-classification/ └── dataset/ ├── Luke_Skywalker/ └── Obi_Wan_Kenobi/


Cada subpasta contém imagens do respectivo personagem. O dataset foi extraído de um arquivo `.rar` hospedado no Google Drive.

## 🧠 Etapas do Projeto

1. **Pré-processamento das imagens** com redimensionamento para 224x224 e normalização.
2. **Treinamento de uma CNN do zero** para servir como baseline.
3. **Aplicação de Transfer Learning** com a arquitetura VGG16 pré-treinada no ImageNet.
4. **Congelamento das camadas da VGG16**, exceto a última, que foi substituída por uma camada `Dense` com 2 neurônios (softmax).
5. **Comparação de desempenho** entre o modelo treinado do zero e o modelo com Transfer Learning.
6. **Predição de novas imagens** com visualização das probabilidades por classe.

## 📊 Resultados

O modelo com Transfer Learning apresentou desempenho superior em acurácia e generalização, mesmo com um número limitado de amostras.

## 📦 Requisitos

- Python 3.10+
- TensorFlow / Keras
- NumPy, Matplotlib, PIL

## 🚀 Como rodar

Basta abrir o notebook `transfer-learning-editado.ipynb` no Google Colab ou em um ambiente com Jupyter Notebook. Certifique-se de que o dataset esteja disponível no caminho correto.

---

Que a força esteja com seu classificador!