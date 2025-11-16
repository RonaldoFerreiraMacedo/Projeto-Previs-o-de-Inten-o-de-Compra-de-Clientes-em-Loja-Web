# 🛒 Previsão de Intenção de Compra em E-commerce

Modelo de Machine Learning para prever se um cliente irá realizar compras no site com base em dados demográficos e comportamentais.

# 📌 Visão Geral

Este projeto desenvolve um sistema preditivo capaz de antecipar a intenção de compra online de clientes de um e-commerce, analisando padrões de comportamento, visitas ao site, perfil socioeconômico e histórico de compras.

# A solução ajuda empresas a:

direcionar campanhas de marketing com maior precisão

aumenta conversão

reduzir custos de publicidade

compreender seu público com profundidade

É um estudo completo, passando por EDA, pré-processamento, limpeza, visualização, modelagem e avaliação de desempenho.

# 🎯 Objetivos do Projeto

Identificar os fatores que mais influenciam a decisão de compra online.

Modelar variáveis demográficas, financeiras e comportamentais.

Comparar modelos de classificação (Regressão Logística vs Random Forest).

Criar insights acionáveis com storytelling visual.

# 🗂️ Sobre o Dataset

As variáveis incluem dados socioeconômicos, histórico de consumo e comportamento digital:

Variável	Descrição
Year_Birth	Ano de nascimento
Education	Nível educacional
Marital_Status	Estado civil
Income	Renda anual
Kidhome	Número de crianças
Recency	Dias desde a última compra
MntWines, MntFruits, MntMeatProducts	Gastos por categoria
MntFishProducts, MntSweetProducts	Gastos adicionais
NumDealsPurchases	Compras com desconto
NumStorePurchases	Compras em loja física
NumWebVisitsMonth	Visitas ao site no mês
WebPurchases	Variável alvo (0 = não comprou / 1 = comprou)

# 📊 Etapa 1 — Preparação e Análise dos Dados (EDA)
## ✔️ Limpeza e ajuste

Remoção de valores nulos

Correção de estados civis inconsistentes

Tratamento de outliers extremos

Agrupamento de níveis educacionais

## ✔️ Análises realizadas

Distribuições das variáveis

Correlação numérica

Análises por categoria (idade, escolaridade, filhos, etc.)

## 📈Insights encontrados

Clientes sem filhos compram mais online.

Graduados representam a maior parcela dos compradores.

Quanto mais visitas ao site no mês, maior a taxa de compra com pico em 7 visitas.

## ⚙️ Etapa 2 — Pré-processamento

Codificação de variáveis categóricas

Padronização com StandardScaler

Remoção de colunas pouco relevantes (Complain, Recency, Year_Birth, etc.)

Separação em treino e teste (70% / 30%)

## 🤖 Etapa 3 — Modelagem

Foram comparados dois modelos:

### 1️⃣ Regressão Logística

Simples, eficiente e interpretável

Rodou com dados padronizados

Métricas obtidas:

Acurácia: 0.866

F1-score equilibrado para ambas classes

### 2️⃣ Random Forest

Modelo mais robusto

Captura relações não-lineares

Resultados:

Acurácia: 0.914

Melhor precisão e recall

Matriz de confusão com menor taxa de erro

## 🧪 Etapa 4 — Avaliação dos Modelos
✔️ Métricas principais
Modelo	Acurácia	F1-score médio
Regressão Logística	0.866	0.87
Random Forest	0.914	0.91
✔️ Matrizes de confusão

# 🏆 Conclusão

O modelo Random Forest apresentou desempenho superior para prever intenção de compra, com:

maior acurácia

melhor equilíbrio entre precisão e recall

menos erros de classificação

Com melhorias adicionais (como otimização de hiperparâmetros), esse sistema pode ser integrado em campanhas de marketing ou plataformas de CRM para aumentar conversão e reduzir desperdício.
