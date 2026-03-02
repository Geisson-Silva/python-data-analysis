# 🌍 Global Sales Analysis — Python (Pandas & Data Visualization)

## 📌 Visão Geral

Este projeto consiste em uma análise completa de vendas de uma empresa que atua globalmente, comercializando produtos tanto em lojas físicas quanto online.

O objetivo principal foi realizar o ciclo completo de análise de dados:

* entendimento e integração de múltiplas fontes
* limpeza e padronização dos dados
* criação de métricas de negócio
* análises exploratórias
* visualizações para identificação de padrões e insights

O projeto foi desenvolvido em **Python (Google Colab)** utilizando bibliotecas de análise e visualização de dados.

---

## 🎯 Objetivos do Projeto

* Realizar limpeza e tratamento dos dados.
* Integrar três tabelas em um único DataFrame analítico.
* Criar métricas financeiras e operacionais.
* Analisar vendas por:

  * categorias de produtos
  * países e regiões
  * canais de venda (online/offline)
* Avaliar o impacto do tempo de envio.
* Identificar tendências temporais e padrões sazonais.
* Extrair conclusões sob a perspectiva de negócio.

---

## 🗂️ Estrutura dos Dados

O conjunto de dados é composto por:

* **events.csv** — vendas ao longo de vários anos
* **products.csv** — categorias e códigos de produtos
* **countries.csv** — países, regiões e sub-regiões

As tabelas foram conectadas utilizando:

* `product_id`
* `country_code`

---

## 🧹 Limpeza e Preparação dos Dados

Principais etapas executadas:

* remoção de registros com valores ausentes relevantes;
* tratamento de códigos de país ausentes (categoria **UNK / Desconhecido**);
* conversão de datas para formato correto;
* criação da variável de tempo de entrega;
* remoção de duplicatas;
* padronização de colunas e valores textuais;
* normalização de canais de venda.

Após o tratamento, os dados foram integrados em um único DataFrame consolidado para análise. 

---

## 📊 Métricas Criadas

Foram construídos indicadores financeiros e operacionais:

* **Revenue (Receita)**
* **Total Cost (Custo Total)**
* **Profit (Lucro)**
* **Delivery Time (Tempo de envio)**

Além de variáveis temporais:

* ano
* mês
* mês/ano
* dia da semana

---

## 📈 Principais Análises Realizadas

### 🔹 KPIs Gerais

* total de pedidos
* receita total
* lucro total
* unidades vendidas
* abrangência geográfica (países, regiões e sub-regiões)

---

### 🔹 Análise de Vendas

Visualizações e análises por:

* categoria de produtos
* regiões geográficas
* canais de venda (online vs offline)

Objetivo: identificar concentração de receita e desempenho por segmento.

---

### 🔹 Tempo entre Pedido e Envio

Análises realizadas por:

* categoria de produto
* regiões
* países

Também foi investigada a relação entre tempo de envio e lucro médio.

Resultado principal: não foi observada relação forte entre prazo de envio e lucratividade.

---

### 🔹 Dinâmica Temporal das Vendas

Análise da evolução da receita:

* ao longo do tempo
* por categoria
* por região

Objetivo: identificar tendências, ciclos e oscilações.

---

### 🔹 Análise por Dia da Semana

Avaliação do comportamento das vendas por dia para identificar possíveis padrões operacionais e comerciais.

---

### 🔹 Sazonalidade

Análise de:

* unidades vendidas por mês
* média mensal por categoria

Permitindo observar variações sazonais nas vendas.

---

### 🔹 Análise Geográfica

* Top 10 países por receita
* países com maior tempo médio de envio

Identificação de concentração geográfica de desempenho.

---

## 📊 Visualizações

O projeto utiliza gráficos para apoiar a interpretação dos dados:

* bar plots
* line plots
* regressão (profit vs delivery time)
* análises temporais e geográficas

As visualizações foram desenvolvidas com:

* Matplotlib
* Seaborn

---

## 🛠️ Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab

---

## 💼 Principais Insights de Negócio

* concentração de receita em categorias específicas;
* forte influência de determinados mercados geográficos;
* canais online e offline relevantes para o resultado;
* ausência de impacto significativo do tempo de envio no lucro;
* presença de padrões temporais e sazonais nas vendas.

---

## 📄 Estrutura do Repositório

```
python-data-analysis/
│
├── notebooks/
│   └── customer_behavior_analysis.ipynb
│
└── README.md
```

---

## 📌 Observação

Este projeto foi desenvolvido como estudo prático de Análise de Dados, aplicando o processo completo de preparação, análise e visualização com foco em geração de insights de negócio.
