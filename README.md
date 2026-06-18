# Predição de Aprovação de Acesso a Recursos
## Projeto AM - Tema 2

## Descrição

Este projeto desenvolve modelos de classificação binária para prever se uma solicitação de acesso a recurso será aprovada ou negada, utilizando o dataset Amazon Employee Access Challenge.

O objetivo é comparar diferentes abordagens de classificação para dados categóricos altamente desbalanceados, aplicando técnicas de pré-processamento, balanceamento de classes, ajuste de hiperparâmetros e otimização de threshold.

---

## Dataset

O dataset utilizado é o `train.csv`, contendo registros de solicitações de acesso.

A variável alvo é `ACTION`, em que:

- `1`: acesso concedido
- `0`: acesso negado

O conjunto de dados faz parte do desafio Amazon Employee Access Challenge.

---

## Técnicas utilizadas

- Análise Exploratória de Dados (EDA)
- Tratamento de variáveis categóricas
- Agrupamento de categorias raras
- One-Hot Encoding
- RandomUnderSampler parcial
- Regressão Logística
- Random Forest
- Extra Trees
- Bernoulli Naive Bayes
- Ajuste de hiperparâmetros
- Ajuste de threshold de decisão
- Avaliação para dados desbalanceados

---

## Tecnologias

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- SciPy
- Scikit-Learn
- Imbalanced-Learn
- Jupyter Notebook

---

## Pré-requisitos

- Python 3.10 ou superior

---

## Instalação

### 1. Clone o repositório

```bash
git clone <url-do-repositorio>
cd <nome-do-repositorio>
```

### 2. Crie um ambiente virtual (opcional, mas recomendado)

#### Linux/macOS

```bash
python -m venv .venv
source .venv/bin/activate
```

#### Windows

```powershell
python -m venv .venv
.venv\Scripts\activate
```

### 3. Instale as dependências

```bash
pip install -r requirements.txt
```

---

## Estrutura do projeto

```text
AmazonEmployeeAccessML/
│
├── data/
│   └── train.csv
│
└── docs/
│   ├── Predição_de_Aprovação_de_Acesso_a_Recursos.pdf
│
├── results/
│   ├── figures
│       ├── ...
│   ├── results
│       ├── ...
│
├── .gitignore
├── AmazonEmployeeAccess.ipynb
├── README.md
├── requirements.txt
```

---

## Execução

### Google Colab

1. Abra o notebook `AmazonEmployeeAccess.ipynb` no Google Colab.
2. Execute todas as células em ordem.

### Execução local

Inicie o Jupyter Notebook:

```bash
jupyter notebook
```

ou o Jupyter Lab:

```bash
jupyter lab
```

Depois abra o arquivo:

```text
AmazonEmployeeAccess.ipynb
```

e execute todas as células em ordem.

---

## Métricas avaliadas

Os modelos foram avaliados utilizando métricas adequadas para problemas com classes desbalanceadas:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- PR-AUC
- Matriz de Confusão
- Taxa de concessão indevida de acesso

---

## Principais resultados

O melhor modelo final foi selecionado considerando principalmente o desempenho na classe minoritária (acessos negados), utilizando métricas como:

- F1 da classe 0
- ROC-AUC
- PR-AUC
- Taxa de concessão indevida

Além da comparação entre algoritmos, foram avaliados os impactos do balanceamento parcial dos dados e do ajuste do threshold de classificação.

---

## Autores

- Adriana Theil Melcop de Castro
- Marcela Pereira Raposo
- Thawan Ribeiro da Silva