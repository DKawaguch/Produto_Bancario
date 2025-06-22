# 🎯 Predição de Subscrição de Depósitos Bancários com CRISP-DM

Este projeto aplica o processo CRISP-DM em um conjunto de dados de marketing bancário para prever se um cliente irá subscrever um depósito a prazo.

## 📌 Objetivo
Utilizar modelos de classificação para prever a resposta do cliente a uma oferta bancária com base em atributos pessoais, históricos de campanhas anteriores e indicadores socioeconômicos.

## 🔍 Conjunto de Dados
- Fonte: [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)
- Amostras: ~41.000
- Target: `y` (binário) - Subscrição (`yes` ou `no`)

## 🔧 Pipeline CRISP-DM

### 1. Entendimento do Negócio
- Reduzir custos com ligações telefônicas e aumentar taxa de conversão em campanhas.

### 2. Entendimento dos Dados
- Dados categóricos, numéricos e contextuais.
- Variáveis relacionadas ao cliente, à campanha e à economia.

### 3. Preparação dos Dados
- Tratamento de nulos, variáveis constantes, codificação de categorias.
- Padronização de variáveis numéricas.
- Aplicação de PCA para redução de dimensionalidade mantendo 98% da variância.

### 4. Modelagem
- Árvore de decisão (com e sem poda).
- Testes com `max_depth`, `min_samples_split`, `min_samples_leaf`.

### 5. Avaliação
- Acurácia, F1-score, Matriz de Confusão.
- AUC-ROC para avaliar capacidade de distinguir classes.
- Comparação entre árvore podada e não podada.

## 📊 Resultados
- Melhor modelo: Árvore de decisão com poda.
- Foco na melhoria da detecção da classe "sim" (clientes que aceitam a oferta).

## 📎 Tecnologias Utilizadas
- Python 3
- pandas, scikit-learn, matplotlib, seaborn
- Jupyter Notebook

## ✍️ Autor
Danilo Kawaguchi – Estudante de Física e Ciência de Dados

---

