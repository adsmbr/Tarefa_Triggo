# Olist E-Commerce Dataset Analysis

Este projeto realiza uma análise completa do dataset de e-commerce da Olist, desde a preparação e limpeza dos dados, passando pela análise exploratória (EDA), resolução de problemas de negócio, até visualizações interativas e conclusões.

## Estrutura do Projeto

- `analysis.py`: Script principal em Python que executa todo o pipeline de análise.
- `/mnt/data/`: Diretório contendo os arquivos CSV originais do dataset.

## Requisitos

- Python 3.8+
- Bibliotecas Python (instaláveis via pip):
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn plotly sqlite3
  ```

## Como Executar

1. **Clone o repositório**

   ```bash
   git clone https://github.com/adsmbr/Tarefa_Triggo.git
   cd Tarefa_Triggo
   ```

2. **Instale as dependências**

   ```bash
   pip install -r requirements.txt
   ```

3. **Execute o script de análise**

   ```bash
   python analysis.py
   ```

   O script carregará os CSVs, tratará os dados, gerará gráficos estáticos (Matplotlib/Seaborn) e interativos (Plotly), e exibirá as conclusões no terminal.

## Principais Resultados

1. **Sazonalidade de Pedidos**
   - Picos em novembro e dezembro, refletindo eventos como Black Friday e Natal.

2. **Tempo de Entrega e Avaliação**
   - Entregas mais rápidas associadas a notas de avaliação mais altas.

3. **Frete vs Distância**
   - Correlação positiva entre distância percorrida e valor do frete.

4. **Categorias Top por Faturamento**
   - Destaque para Cama, Mesa e Banho; Relógios e Presentes; Beleza e Saúde.

5. **Valor Médio por Estado**
   - SP e RJ lideram em valor médio de pagamento.

6. **Predição de Atrasos**
   - Modelo RandomForest demonstrou boa precisão ao prever atrasos com base em preço e frete.

7. **Segmentação de Clientes**
   - Quatro perfis identificados (Baixo, Médio, Alto e Muito Alto Gasto) para direcionamento de marketing.
