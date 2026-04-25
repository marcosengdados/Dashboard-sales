# 📊 Dashboard de Análise de Vendas — Power BI

> Painel interativo de inteligência comercial com análise de receita, lucro, desempenho por região, segmento de cliente e gerentes de vendas.

---

## 🖼️ Preview do Dashboard

![Dashboard de Vendas](Dashboard-Vendas.png)

<div align="center">

</div>

---

## 🎯 Objetivo do Projeto

Este projeto tem como finalidade construir uma **visão analítica completa do desempenho comercial**, permitindo que gestores e analistas tomem decisões baseadas em dados com agilidade e precisão.

O dashboard responde a perguntas estratégicas como:

- Qual foi a **receita líquida** e o **lucro líquido** no período?  
- Quais **regiões e estados** geram mais resultado?  
- Qual o desempenho por **segmento de cliente**?  
- Como está a performance de cada **gerente de vendas**?  
- O lucro está acima ou abaixo da **meta**?  
- Qual é o **ticket médio** das vendas?  

---

## 🗂️ Estrutura do Relatório

O arquivo `.pbix` contém **1 página**:

| Página | Descrição |
|--------|-----------|
| `Página 1` | Painel principal com todos os KPIs e visualizações |

---

## 📈 Visuais e Indicadores

### 🔢 KPIs (Cards de Resumo)

| Indicador | Descrição |
|-----------|-----------|
| **Receita Líquida** | Total de vendas após deduções |
| **Lucro Líquido** | Resultado após custos e despesas |
| **CMV** | Custo das Mercadorias Vendidas |
| **Ticket Médio** | Valor médio por venda |
| **% Participação Receita** | Share de receita no ranking de segmentos |

### 📊 Gráficos e Mapas

| Visual | Tipo | Dimensão Analisada |
|--------|------|-------------------|
| Lucro por Região | Barras Horizontais | Região |
| Lucro por Segmento de Cliente | Barras Horizontais | Segmento do Cliente |
| Evolução do Lucro vs. Meta | Linhas | Mês / Ano |
| Receita por Gerente | Rosca (Donut) | Gerente |
| Mapa Geográfico de Vendas | Mapa Interativo | Estado |

### 🎛️ Filtros (Slicers)

- **Ano** — filtra todo o relatório por período anual  
- **Estado** — filtra por unidade federativa  

---

## 🧱 Modelo de Dados

O modelo segue o padrão **Star Schema** com as seguintes tabelas identificadas:

- 📁 Vendas          → tabela fato principal (Valor da Venda, Estado, Região, Segmento)
- 📅 dCalendario     → dimensão de tempo (Ano, Mês, Hierarquia)
- 👔 Gerentes        → dimensão de gestores (Gerente, Receita por Gerente)
- 📐 RECEITA         → medidas de receita (Receita Líquida)
- 💰 LUCROS          → medidas de lucro (Lucro Líquido, Ticket Médio, Meta)
- 🏷️ CMV             → custo das mercadorias vendidas
- 📊 Ranking         → métricas de participação percentual

---

## 🛠️ Tecnologias Utilizadas

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Data Modeling](https://img.shields.io/badge/Star%20Schema-4CAF50?style=for-the-badge&logo=databricks&logoColor=white)

- **Power BI Desktop** — construção do relatório  
- **DAX** — criação de medidas calculadas (Lucro Líquido, Ticket Médio, Meta, % Participação)  
- **Power Query (M)** — transformação e modelagem dos dados  

---
## 💡 Insights com Este Dashboard

- Identificar **regiões com maior margem de lucro** para priorizar investimentos  
- Detectar **segmentos de clientes mais rentáveis** e concentrar esforços de vendas  
- Comparar **desempenho mensal vs. meta** para acionar planos de contingência  
- Avaliar a **contribuição individual de cada gerente** para a receita total  
- Mapear **estados com maior volume de vendas** para expansão geográfica  
- Monitorar o **ticket médio** para avaliar eficiência comercial  

---

## 📜 Licença

Distribuído sob a licença MIT [`LICENSE`](LICENSE).

---

## 👤 Autor

Feito por **Marcos Vinicius Lima**
