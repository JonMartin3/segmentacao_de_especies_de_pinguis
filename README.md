# 🐧 Penguin Species Clustering with K-Means
## 📌 Visão Geral

Este projeto aplica o algoritmo de Clusterização K-Means para segmentar espécies de pinguins com base em características físicas.

O objetivo é demonstrar a versatilidade de técnicas de aprendizado não supervisionado em um contexto biológico, explorando padrões naturais presentes nos dados.

A metodologia utilizada foi o CRISP-DM, garantindo uma abordagem estruturada e alinhada às boas práticas de projetos de ciência de dados.


## 1️⃣ Business Understanding
🎯 Problema

Identificar agrupamentos naturais em dados biológicos de pinguins, utilizando variáveis físicas como:

* Comprimento do bico
* Profundidade do bico
* Comprimento da nadadeira
* Massa corporal

🎯 Objetivo

Aplicar o algoritmo K-Means para identificar automaticamente padrões e agrupamentos que representem as diferentes espécies de pinguins.

Embora o dataset possua a variável species, ela foi removida durante o treinamento para simular um cenário real de clusterização não supervisionada.

## 2️⃣ Data Understanding
📊 Dataset

Dataset: penguins (Seaborn)

Espécies presentes:

* Adelie
* Chinstrap
* Gentoo

Principais variáveis numéricas utilizadas:

* bill_length_mm
* bill_depth_mm
* flipper_length_mm
* body_mass_g

🔎 Análises realizadas

* Verificação de valores nulos
* Remoção de registros incompletos
* Análise descritiva
* Visualização com pairplot
* Observação inicial de possíveis agrupamentos

A análise exploratória já indicava a presença de aproximadamente 3 agrupamentos naturais, coerentes com o número de espécies.

## 3️⃣ Data Preparation
🔧 Tratamentos aplicados

* Remoção de valores faltantes
* Exclusão de variáveis categóricas (species, island, sex)
* Padronização das variáveis com StandardScaler

A padronização foi essencial porque o K-Means é sensível à escala das variáveis.

## 4️⃣ Modeling
🤖 Algoritmo utilizado

* K-Means
* Número de clusters definido como 3
* random_state=42 para reprodutibilidade

⚙️ Processo

* Ajuste do modelo nos dados padronizados
* Extração dos centroides
* Conversão dos centroides para escala original
* Geração dos labels de cluster

## 5️⃣ Evaluation
📊 Visualizações realizadas

Foram construídas múltiplas matrizes de dispersão com:

* bill_length_mm × bill_depth_mm
* flipper_length_mm × body_mass_g
* bill_length_mm × body_mass_g
* bill_length_mm × flipper_length_mm

Incluindo:

* Pontos coloridos por cluster
* Centroides destacados

📌 Principais Insights

* O comprimento do bico (bill_length_mm) demonstrou forte poder discriminativo.
* A massa corporal também contribuiu significativamente para a separação.
* Os clusters formados apresentaram coerência visual com as espécies reais.

## 🛠️ Tecnologias Utilizadas

* Python
* Pandas
* Seaborn
* Plotly
* Scikit-learn
* StandardScaler
* KMeans


👨‍💻 Autor

Jonathan Martins
Data Science | Machine Learning | Analytics
### Projeto para fins academicos
