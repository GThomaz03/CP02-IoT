# 🧠 Checkpoint 2 – Redes Neurais com Keras

Disciplina: **Disruptive Architectures: IoT, IoB e Generative AI**  
Atividade: **Treinamento de Redes Neurais com Keras (Dados Tabulares)**  
Peso: **40% da nota do CP2**  

---

## 📂 Estrutura do Repositório

```
/redes-neurais-keras
│── exercicio1_classificacao.ipynb # Classificação Multiclasse (Wine Dataset)
│── exercicio2_regressao.ipynb # Regressão (California Housing)
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
git clone https://github.com/SEU_USUARIO/redes-neurais-keras.git
cd redes-neurais-keras
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