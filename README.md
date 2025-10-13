# 🧠 Checkpoint 2 – Redes Neurais com Keras

Disciplina: **Disruptive Architectures: IoT, IoB e Generative AI**  
Atividade: **Treinamento de Redes Neurais com Keras (Dados Tabulares)**  
Peso: **40% da nota do CP2**  

---

## 📂 Estrutura do Repositório

```
/redes-neurais-keras
│── CP02-1.ipynb # Classificação Multiclasse (Wine Dataset)
│── CP02-2.ipynb # Regressão (California Housing)
│── teachable-machine-1
│── teachable-machine-2
│── README.md # Instruções e resultados
```


---

## 📌 Exercício 1 – Classificação Multiclasse
- **Dataset**: [Wine Dataset (UCI)](https://archive.ics.uci.edu/dataset/109/wine) – carregado via `sklearn.datasets.load_wine`.
- **Rede Neural (Keras)**:
  - 2 camadas ocultas (32 neurônios cada), ativação **ReLU**
  - Camada de saída com 3 neurônios (softmax)
  - Função de perda: `categorical_crossentropy`
  - Otimizador: `Adam`
- **Comparação**:
  - `LogisticRegression`
  - `RandomForestClassifier`
- **Métrica**: Acurácia

---

## 📌 Exercício 2 – Regressão
- **Dataset**: [California Housing Dataset](https://scikit-learn.org/stable/datasets/real_world.html#california-housing-dataset) – carregado via `sklearn.datasets.fetch_california_housing`.
- **Rede Neural (Keras)**:
  - 3 camadas ocultas (64, 32, 16 neurônios), ativação **ReLU**
  - Saída com 1 neurônio (linear)
  - Função de perda: `mse`
  - Otimizador: `Adam`
- **Comparação**:
  - `LinearRegression`
  - `RandomForestRegressor`
- **Métricas**: RMSE e MAE

---

## ▶️ Como Executar os Experimentos

### 1. Clonar o repositório
```bash
git clone https://github.com/GThomaz03/CP02-IoT.git
cd CP02-IoT
```
### 2. Criar ambiente virtual (opcional, mas recomendado)
```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```
### 3. Instalar dependências
```bash
pip install tensorflow scikit-learn pandas numpy matplotlib
```
### 4. Abrir os notebooks
```bash
jupyter notebook
```

E executar:
- exercicio1_classificacao.ipynb
- exercicio2_regressao.ipynb

---
📊 Resultados Esperados

- Exercício 1 (Wine Dataset):
    Comparar a acurácia da rede neural com Logistic Regression e Random Forest.
        Normalmente, Random Forest tende a se sair melhor em datasets tabulares pequenos.

- Exercício 2 (California Housing):
    Comparar RMSE/MAE entre rede neural, Linear Regression e Random Forest.
        Em geral, Random Forest atinge melhor desempenho, enquanto a rede neural precisa de mais ajustes de hiperparâmetros.

---

📌 Conclusão

- Random Forest geralmente apresenta maior robustez em dados tabulares.
- Redes neurais podem alcançar desempenho competitivo, mas são mais sensíveis a hiperparâmetros.
- Linear Regression serve como baseline simples para comparação.

---
Integarntes:

- Gabriel Alves Thomaz - RM558637

---
# Parte 2

links dos datasets:
- https://app.roboflow.com/teste-atffo/coco128-iugjx-c5qje/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true
- https://universe.roboflow.com/new-workspace-s0sid/bus-yqkys/dataset/2
- https://universe.roboflow.com/yu-cttti/motorcycle-a1sts/dataset/2

---
Teachable machine foi treinado com duas classes, ônibus e motos utilizando os datasest citados acima e testado comuma imagem que não foi utilizada no treinamento 
