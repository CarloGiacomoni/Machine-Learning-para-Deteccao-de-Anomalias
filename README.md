# Machine Learning para Detecção de Anomalias
Este repositório contém um projeto de **Machine Learning para detecção de anomalias** utilizando a **linguagem R** para o apresentação em Dashboard no Power BI. O projeto foi desenvolvido como parte do **Lab 08 - Machine Learning no Power BI com Linguagem R para Detecção de Anomalias**, que faz parte do capítulo 17 do curso de **Microsoft Power BI para Business Intelligence e Data Science** da **Data Science Academy**. O foco principal do projeto é aplicar técnicas de aprendizado não supervisionado para identificar anomalias em conjuntos de dados de uma empresa (ficticia) do ramo financeiro.

# Técnica Utilizada
A técnica empregada neste projeto é o **aprendizado não supervisionado**.  
O objetivo é identificar padrões incomuns ou atípicos nos dados sem a necessidade de rótulos pré-existentes.

# Pacotes Utilizados
Os seguintes pacotes **R** foram instalados e utilizados neste projeto:

- tidyverse
- dplyr
- solitude
- ggplot2
- readr

# Gráficos Utilizados
Os gráficos empregados para visualização e análise dos resultados, foram:

- Gráfico de densidade
- Gráfico de dispersão (geom_point) com destaque para pontos anômalos (em vermelho)
- Box plot (geom_boxplot) para análise da distribuição dos dados

# Fluxo do Projeto
O projeto segue os seguintes passos:

1. Carregamento dos dados históricos.
2. Criação do modelo de Machine Learning utilizando o algoritmo Isolation Forest.
3. Treinamento do modelo com os dados históricos.
4. Realização de previsões utilizando o modelo treinado e os dados históricos.
5. Criação de um Density Plot para visualizar os scores de anomalia.

![Density Plot](https://github.com/CarloGiacomoni/Machine-Learning-para-Deteccao-de-Anomalias/blob/main/Density%20Plot.png)


6. Definição de um limiar para identificação de anomalias (anomaly score acima de 0.62).
7. Aplicação do filtro para identificar registros considerados anomalias.
8. Geração e visualização de gráfico com os resultados obtidos.

![geom_point01](https://github.com/CarloGiacomoni/Machine-Learning-para-Deteccao-de-Anomalias/blob/main/geom_point01.png)

Além disso, o projeto também contempla a aplicação do modelo treinado em novos dados:

1. Carregamento dos novos dados.
2. Realização de previsões com o modelo treinado nos novos dados.
3. Aplicação do limiar de anomalia (0.62) para filtrar anomalias nos novos dados.

![geom_point02](https://github.com/CarloGiacomoni/Machine-Learning-para-Deteccao-de-Anomalias/blob/main/geom_point02.png)

4. Visualização dos resultados em um gráfico.

![geom_boxplot](https://github.com/CarloGiacomoni/Machine-Learning-para-Deteccao-de-Anomalias/blob/main/geom_boxplot.png)

![Dashboard](https://github.com/CarloGiacomoni/Machine-Learning-para-Deteccao-de-Anomalias/blob/main/PB.png)

[Power BI](https://app.powerbi.com/view?r=eyJrIjoiMjFiYjYyM2QtMmY0NS00NjcyLWE3MzctOTU2YjZmYjRlZjczIiwidCI6ImQ2YjQ0ZTk0LWJiMDktNGE1Ni05ZjMxLWJlYmVjYmFhMmQ0ZCJ9)
##### Obs: Os visuais R são um recurso do Power BI Pro. Somente usuários com uma licença do Power BI Pro podem criar, exibir ou interagir com visuais R
--------

# Autor:

**Carlo Giacomoni** sob orientação de **Data Science Academy** para o curso de **Microsoft Power BI para Business Intelligence e Data Science**
[Linkedin](https://www.linkedin.com/in/carlo-giacomoni/)

---------

**Observação:** As imagens dos gráficos gerados durante a execução do projeto foram incluídas neste README para melhor ilustração.  

**Nota:** Este README fornece uma visão geral do projeto de detecção de anomalias utilizando Machine Learning e a linguagem R. Detalhes específicos sobre a implementação, código-fonte e resultados podem ser encontrados nos arquivos e códigos contidos neste repositório.
