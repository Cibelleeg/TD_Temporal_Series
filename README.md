# README - Análise de Séries Temporais


Este repositório realiza uma análise de séries temporais sobre a variável `vendas`, explorando componentes de tendência, sazonalidade e ruído. Também investiga o impacto de feriados e campanhas ativas e compara modelos aditivo e multiplicativo para identificar o mais adequado.

## Estrutura do Notebook

### Carregamento e Preparação dos Dados

 - Importação das bibliotecas.
 - Leitura do dataset e limpeza de colunas inúteis.
 - Conversão de datas e definição do índice.
 - Cálculo da tendência por média móvel centrada.
 - Extração do componente sazonal aditivo e multiplicativo.
 - Decomposição Automática
 - Visualização dos Componentes
 - Comparação de Modelos
 - Cálculo de métricas (desvio padrão dos resíduos e RMSE).
 - Análise de Impacto de Feriados e Campanhas
 - Boxplots comparando vendas em feriados vs dias normais.
 - Boxplots de vendas com e sem campanhas ativas.

### Dependências

 - pandas
 - numpy
 - matplotlib
 - seaborn
 - statsmodels

Instale via:
`pip install pandas numpy matplotlib seaborn statsmodels`

## Discussão e resultados

### Principais Resultados

 - Modelo Multiplicativo mostrou-se superior, apresentando resíduos muito menores.
 - Sazonalidade e tendência *crescentes* ao longo do tempo, validando o uso de abordagem multiplicativa.
 - Feriados tendem a elevar levemente o volume médio de vendas.
 - Campanhas ativas apresentam impacto com picos mais dispersos.

### Recomendações

Com base nos resultados da análise feita acima, sugiro as seguintes recomendações:

 - Planejar campanhas alinhadas aos picos sazonais
 - Aproveitar feriados para ações específicas
 - Modelagem e previsão contínua com modelo multiplicativo
 - Análise contínua de séries temporais
