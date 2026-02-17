# VFS - Data Analyst Technical Interview

<h2>1. Visão Geral do Projeto</h2>

Este projeto tem como objetivo analisar dados históricos de seguro automotivo para identificar os principais sinais associados a maior risco de sinistros e transformar os achados analíticos em insights acionáveis para o negócio.
A solução contempla análise exploratória de dados (EDA), segmentação de risco e um dashboard em Power BI, com foco em apoiar decisões de precificação, underwriting e retenção.

Nota: O projeto, o notebook e o dashboard foram desenvolvidos em inglês, considerando o contexto de um ambiente corporativo multinacional. Este README foi disponibilizado em português para facilitar a leitura e avaliação do processo.

<h2>2. Estrutura do Repositório</h2>

├── data/  
│   └── Car_Insurance_Claim.csv  
│   └── insurance_dashboard_final.csv  
├── notebooks/  
│   └── VFS - Data Analyst Technical Interview.ipynb  
├── dashboard/  
│   └── VFS - Data Analyst Technical Interview.pbix  
└── README.md  

<h2>3. Preparação e Processamento dos Dados (Python)</h2>

Todas as etapas de preparação e análise dos dados estão implementadas no notebook: VFS - Data Analyst Technical Interview.ipynb

Principais etapas:

Auditoria dos dados (tipos, missing, duplicidades e outliers)  
Engenharia de atributos e criação de faixas (idade, experiência, acidentes, quilometragem)  
Segmentação de risco e cálculo de KPIs  
Exportação de um dataset final, pronto para consumo no Power BI  

Dataset final utilizado no Power BI: insurance_dashboard_final.csv  

<h2>4. Decisões de Tratamento de Dados</h2>

Todas as decisões foram documentadas em etapa específica dentro do notebook e orientadas pela interpretabilidade de negócio e robustez analítica.  

<h2>5. KPIs Definidos</h2>

Total de Clientes  
Total de Sinistros  
Taxa de Sinistro (%)  

A Taxa de Sinistro é definida de forma consistente como: Taxa de Sinistro = Total de Sinistros / Total de Clientes  

A mesma métrica é utilizada em todos os visuais e páginas do dashboard.

<h2>6. Dashboard (Power BI)</h2>

O dashboard em Power BI está estruturado em três níveis analíticos:

P1 – Visão Geral

KPIs principais (clientes, sinistros, taxa de sinistro)  
Distribuição de sinistros por idade, experiência de direção, gênero e estado civil  
Taxa de sinistro por histórico de acidentes  

P2 – Drivers e Interações

Filtros interativos (idade, gênero, estado civil, experiência, renda, tipo e ano do veículo)  
Heatmaps: Experiência de Direção × Acidentes Anteriores e Renda × Escolaridade  
Total de Sinistros por tipo e ano do veículo  

P3 – Recomendações de Negócio

4 recomendações objetivas, orientadas por dados, com foco em precificação, segmentação e enriquecimento de dados  

<h2>7. Como Executar o Projeto</h2>

Análise em Python  

Abra o notebook: notebooks/VFS - Data Analyst Technical Interview.ipynb  
Execute todas as células em sequência.  
O dataset final será exportado automaticamente para uso no Power BI.  

Power BI  

Abra o arquivo: dashboard/VFS - Data Analyst Technical Interview.pbix  
Caso solicitado, atualize o caminho da fonte de dados para: insurance_dashboard_final.csv  

<h2>8. Principais Decisões Analíticas</h2>

Foco em frequência de sinistros, não severidade (informação de severidade indisponível)  
Priorização de segmentações interpretáveis, em vez de modelos complexos  
Alinhamento total entre EDA, visuais do dashboard e recomendações finais  

<h2>9. Limitações do Dataset</h2>

Ausência de dados de severidade dos sinistros  
Valor de mercado dos veículos não disponível  
Exposição assumida uniforme entre clientes  
Algumas variáveis funcionam como proxies (ex.: ano do veículo em vez de preço)  
Resultados refletem padrões históricos e podem não capturar mudanças futuras de comportamento  

<h2>10. Autor</h2>

Guilherme Ruppel  
Data Analyst  
Fevereiro de 2026  
