# Transfer Learning com VGG16 — Classificação de Rostos Star Wars 🛸

Este projeto aplica técnicas de **Transfer Learning** usando a arquitetura **VGG16** para classificar imagens de personagens do universo Star Wars: **Luke Skywalker** e **Obi-Wan Kenobi**.

## 📁 Estrutura do Dataset
O dataset está organizado em duas pastas:
- `Luke_Skywalker/`
- `Obi_Wan_Kenobi/`

Cada pasta contém imagens do respectivo personagem. O dataset foi extraído de um arquivo `.rar` hospedado no Google Drive.

## 🧠 Etapas do Projeto
1. Pré-processamento das imagens com `ImageDataGenerator` e `preprocess_input`
2. Treinamento de uma CNN do zero
3. Aplicação de Transfer Learning com VGG16
4. Comparação de desempenho entre os modelos
5. Avaliação final com imagens novas

## 📊 Resultados
O modelo com Transfer Learning apresentou melhor desempenho em acurácia e generalização, mesmo com um dataset pequeno.

## 📦 Requisitos
- Python 3.10+
- TensorFlow / Keras
- NumPy, Matplotlib, PIL

## 🚀 Como rodar
Basta abrir o notebook `transfer-learning-editado.ipynb` no Google Colab ou em um ambiente com Jupyter Notebook.

---

Que a força esteja com seu classificador!
