
# Olist E-Commerce Dataset Analysis

Análise completa e visualmente aprimorada do dataset público da Olist, uma plataforma de e-commerce brasileira que conecta pequenos vendedores a grandes marketplaces.

## Sobre o Projeto

Este projeto tem como objetivo realizar uma **análise exploratória**, desenvolver **modelos preditivos**, aplicar **técnicas de segmentação de clientes** e criar **visualizações interativas** com base no conjunto de dados da Olist. A análise considera aspectos como logística, comportamento de compra, avaliação de clientes e desempenho de vendedores.

---

## Tecnologias Utilizadas

- Python 3.x  
- Pandas & NumPy  
- Matplotlib & Seaborn  
- Plotly (express e graph_objects)  
- SQLite (via `sqlite3`)  
- Scikit-learn  

---

## Estrutura dos Dados

O projeto utiliza os seguintes arquivos CSV:

- `olist_customers_dataset.csv`
- `olist_geolocation_dataset.csv`
- `olist_orders_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_order_payments_dataset.csv`
- `olist_order_reviews_dataset.csv`
- `olist_products_dataset.csv`
- `olist_sellers_dataset.csv`
- `product_category_name_translation.csv`

Todos os arquivos são carregados, tratados e integrados em um modelo relacional SQLite em memória para facilitar consultas SQL durante a análise.

---

## Etapas do Projeto

### 1. Preparação dos Dados
- Importação de bibliotecas
- Carregamento dos CSVs
- Limpeza: remoção de duplicatas, padronização de colunas
- Tradução das categorias de produtos
- Verificação de dados ausentes

### 2. Análise Exploratória
- Evolução dos pedidos por mês
- Distribuição do tempo de entrega
- Relação entre frete e distância
- Top 10 categorias por faturamento
- Valor médio de pedidos por estado

### 3. Problemas de Negócio
- **Retenção de clientes:** análise de recorrência
- **Predição de atraso:** usando Random Forest
- **Segmentação de clientes:** via K-Means e visualização com boxplot
- **Satisfação vs Entrega:** análise de impacto do prazo na avaliação

### 4. Visualizações Interativas
- Linha do tempo de pedidos
- Mapa de calor por estado com Plotly Choropleth
- Dispersão interativa: Avaliação vs Tempo de entrega
- Dashboard de vendedores: pedidos, avaliação média e distância

### 5. Conclusões

```
- Picos de pedidos em Nov/Dez indicam datas sazonais.
- Entregas rápidas geram melhores notas.
- Correlação entre distância e frete reforça impacto logístico.
- Segmentação revela perfis valiosos para marketing.
- SP e RJ lideram em faturamento médio.
- Categorias com maior faturamento: Beleza e Saúde; Relógios e Presentes; Cama, Mesa e Banho.
- Modelo RandomForest mostrou boa performance na predição de atrasos.
```

---

## Insights Relevantes

- A logística influencia diretamente o valor do frete e a satisfação do cliente.
- A maior parte dos clientes realiza apenas uma compra — há potencial para estratégias de fidelização.
- A segmentação baseada em valor gasto pode ser usada em campanhas direcionadas.
- Atrasos impactam negativamente as avaliações, o que pode prejudicar a reputação da marca.

---

## Como Executar

1. Clone o repositório.
2. Certifique-se de ter os arquivos CSV na pasta apropriada.
3. Instale as dependências com:
   ```bash
   pip install scikit-learn plotly pandas matplotlib seaborn
   ```
4. Execute o script `.py` ou o notebook Jupyter.

---

## Requisitos

- Python 3.7+
- Navegador para visualizações Plotly
- Ambiente compatível com gráficos interativos (como Jupyter Notebook ou Google Colab)

