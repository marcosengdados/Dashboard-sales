# 📊 Dashboard de Análise de Vendas — Power BI
 
> Painel interativo de inteligência comercial com análise de receita, lucro, desempenho por região, segmento de cliente e gerentes de vendas.
 
---
 
## 🖼️ Preview do Dashboard
 
<!-- Adicione abaixo o print do seu dashboard -->
> 📌 **Para adicionar a imagem:** faça o upload do screenshot na pasta `/assets/` do repositório e substitua o bloco abaixo:
 
```md
![Dashboard de Vendas](/assets/[Dashboard-Vendas.png])
```
 
<!-- Descomente a linha abaixo após adicionar a imagem:
![Dashboard de Vendas](assets/[Dashboard-Vendas.png]
-->
 
<div align="center">
  <i>🔜 Imagem do dashboard será exibida aqui — adicione o arquivo em <code>assets/dashboard-preview.png</code></i>
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
---
 
## 🗂️ Estrutura do Relatório
 
O arquivo `.pbix` contém **3 páginas**:
 
| Página | Descrição |
|--------|-----------|
| `Página 1` | Painel principal com todos os KPIs e visualizações |
| `Página 2` | Rascunho / dados auxiliares (oculta no modo de visualização) |
| `Duplicata de Página 1` | Variação do painel principal para análise comparativa |
 
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
| Lucro por Região | Gráfico de Barras Horizontal | Região |
| Lucro por Segmento de Cliente | Gráfico de Barras Horizontal | Segmento do Cliente |
| Evolução do Lucro vs. Meta | Gráfico de Linhas | Mês / Ano |
| Receita por Gerente | Gráfico de Rosca (Donut) | Gerente |
| Mapa Geográfico de Vendas | Mapa Interativo | Estado |
 
### 🎛️ Filtros (Slicers)
 
- **Ano** — filtra todo o relatório por período anual
- **Estado** — filtra por unidade federativa
---
 
## 🧱 Modelo de Dados
 
O modelo segue o padrão **Star Schema** com as seguintes tabelas identificadas:
 
```
📁 Vendas          → tabela fato principal (Valor da Venda, Estado, Região, Segmento)
📅 dCalendario     → dimensão de tempo (Ano, Mês, Hierarquia)
👔 Gerentes        → dimensão de gestores (Gerente, Receita por Gerente)
📐 RECEITA         → medidas de receita (Receita Líquida)
💰 LUCROS          → medidas de lucro (Lucro Líquido, Ticket Médio, Meta)
🏷️ CMV             → custo das mercadorias vendidas
📊 Ranking         → métricas de participação percentual
```
 
---
 
## 🛠️ Tecnologias Utilizadas
 
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Data Modeling](https://img.shields.io/badge/Star%20Schema-4CAF50?style=for-the-badge&logo=databricks&logoColor=white)
 
- **Power BI Desktop** — construção do relatório
- **DAX** — criação de medidas calculadas (Lucro Líquido, Ticket Médio, Meta, % Participação)
- **Power Query (M)** — transformação e modelagem dos dados
- **Tema Fluent 2** — identidade visual moderna (Microsoft Design System)
---
 
## 🚀 Como Utilizar
 
### Pré-requisitos
 
- [Power BI Desktop](https://powerbi.microsoft.com/pt-br/desktop/)
### Passos
 

## 💡 Insights com Este Dashboard
 
- Identificar **regiões com maior margem de lucro** para priorizar investimentos
- Detectar **segmentos de clientes mais rentáveis** e concentrar esforços de vendas
- Comparar **desempenho mensal vs. meta** para acionar planos de contingência
- Avaliar a **contribuição individual de cada gerente** para a receita total
- Mapear **estados com maior volume de vendas** para expansão geográfica
---

## 📜 Licença
 
Distribuído sob a licença MIT. Veja [`LICENSE`](LICENSE) para mais informações.
 
---
 
## 👤 Autor
 
Feito com 💙 por **[Marcos Vinicius Lima]**
 
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/seu-perfil)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/seu-usuario)
 
---
 
<div align="center">
  <sub>⭐ Se este projeto te ajudou, deixa uma estrela no repositório!</sub>
</div>
