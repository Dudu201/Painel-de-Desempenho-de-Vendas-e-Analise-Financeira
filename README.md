# Documentação da Base de Dados
## 1. Descrição Geral
Esta base de dados é utilizada para analisar dados de vendas e desempenho financeiro, permitindo gerar insights sobre diferentes segmentos, países e produtos. Os dados incluem informações como quantidade de unidades vendidas, preços, vendas brutas, descontos, custo de mercadorias vendidas (COGS) e lucros, além de dados temporais para análises sazonais.

![Dashboard de Vendas](https://raw.githubusercontent.com/Dudu201/Painel-de-Desempenho-de-Vendas-e-Analise-Financeira/refs/heads/main/Dashboard%20Reporte%20FInanceiro.png)
---

## 2. Estrutura dos Dados
A tabela contém as seguintes colunas:

- **Segment**: Segmento de mercado (ex.: `Government`, `Midmarket`).
- **Country**: País onde a venda foi realizada (ex.: `Canada`, `Germany`).
- **Product**: Produto vendido (ex.: `Carretera`).
- **Discount Band**: Faixa de desconto aplicada (ex.: `None`).
- **Units Sold**: Quantidade de unidades vendidas.
- **Manufacturing Price**: Preço de fabricação por unidade.
- **Sale Price**: Preço de venda por unidade.
- **Gross Sales**: Receita bruta (calculada como `Units Sold x Sale Price`).
- **Discounts**: Valor dos descontos aplicados.
- **Sales**: Receita líquida após descontos (`Gross Sales - Discounts`).
- **COGS**: Custo das mercadorias vendidas (`Units Sold x Manufacturing Price`).
- **Profit**: Lucro líquido (`Sales - COGS`).
- **Date**: Data da venda.
- **Month Number**: Número do mês (ex.: `1` para Janeiro).
- **Month Name**: Nome do mês (ex.: `January`).
- **Year**: Ano (ex.: `2014`).

---

## 3. Exemplos de Registros
| Segment     | Country  | Product   | Discount Band | Units Sold | Manufacturing Price | Sale Price | Gross Sales | Discounts | Sales      | COGS       | Profit     | Date       | Month Number | Month Name | Year |
|-------------|----------|-----------|---------------|------------|----------------------|------------|-------------|-----------|------------|------------|------------|------------|--------------|------------|------|
| Government  | Canada   | Carretera | None          | 1,618.50   | 3.00                 | 20.00      | 32,370.00   | 0         | 32,370.00  | 16,185.00  | 16,185.00  | 01/01/2014 | 1            | January    | 2014 |
| Government  | Germany  | Carretera | None          | 1,321.00   | 3.00                 | 20.00      | 26,420.00   | 0         | 26,420.00  | 13,210.00  | 13,210.00  | 01/01/2014 | 1            | January    | 2014 |
| Midmarket   | France   | Carretera | None          | 2,178.00   | 3.00                 | 15.00      | 32,670.00   | 0         | 32,670.00  | 21,780.00  | 10,890.00  | 01/06/2014 | 6            | June       | 2014 |
| Midmarket   | Germany  | Carretera | None          | 888.00     | 3.00                 | 15.00      | 13,320.00   | 0         | 13,320.00  | 8,880.00   | 4,440.00   | 01/06/2014 | 6            | June       | 2014 |

---

## 4. Aplicações no Dashboard
Os dados desta base são usados no dashboard para:
- Visualizar as vendas por segmento, país e produto.
- Analisar o desempenho financeiro com métricas como lucro e receita líquida.
- Identificar tendências sazonais por mês e ano.
- Avaliar o impacto de descontos no faturamento.

---

## 5. Considerações
O **dashboard de vendas** é uma ferramenta essencial para a tomada de decisões estratégicas, fornecendo uma visão clara e detalhada do desempenho comercial. Ele permite que as empresas monitorem suas **métricas chave**, como vendas brutas, lucros, unidades vendidas e descontos, em tempo real. Essa análise facilita a identificação de tendências, oportunidades de melhoria e áreas que precisam de atenção.

Com o uso de gráficos e tabelas dinâmicas, o dashboard ajuda a **visualizar dados complexos**, tornando-os mais acessíveis e compreensíveis para diferentes stakeholders, como gerentes e executivos. Ele também permite a **comparação de desempenho entre diferentes segmentos de mercado**, países e produtos, promovendo uma análise mais precisa sobre o que está funcionando e o que não está.

Além disso, o dashboard contribui para **otimizar a estratégia de vendas**, ajustando campanhas, políticas de preços e descontos com base em dados concretos. Ele facilita a detecção de padrões sazonais, ajudando as empresas a se prepararem para picos de demanda ou períodos de baixo desempenho.

Em resumo, o dashboard de vendas é fundamental para melhorar a **eficiência operacional**, aumentar as vendas e maximizar o lucro, proporcionando uma visão estratégica e detalhada do negócio.

