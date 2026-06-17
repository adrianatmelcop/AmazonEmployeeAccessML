# Predição de Aprovação de Acesso a Recursos
## Projeto AM - Tema 2

## Descrição
Este projeto desenvolve modelos de classificação binária para prever se uma solicitação de acesso a recurso será aprovada ou negada, utilizando o dataset Amazon Employee Access Challenge.

## Dataset
O dataset utilizado é o `train.csv`, contendo registros de solicitações de acesso. A variável alvo é `ACTION`, em que:
- `1`: acesso concedido
- `0`: acesso negado

## Técnicas utilizadas
- Análise Exploratória de Dados
- Tratamento de variáveis categóricas
- OneHotEncoder
- Agrupamento de categorias raras
- RandomUnderSampler parcial
- Regressão Logística
- Random Forest
- Extra Trees
- Bernoulli Naive Bayes
- Ajuste de hiperparâmetros
- Ajuste de threshold
- Avaliação com métricas para dados desbalanceados

## Como executar
1. Abrir o notebook no Google Colab.
2. Fazer upload do arquivo `train.csv`.
3. Executar todas as células em ordem.

## Principais resultados
O melhor modelo final foi selecionado com base no desempenho na classe minoritária, considerando métricas como F1 da classe 0, AUC-ROC, PR-AUC e taxa de concessão indevida.

## Autores
Adriana Theil Melcop de Castro
Marcela Pereira Raposo
Thawan Ribeiro Silva
