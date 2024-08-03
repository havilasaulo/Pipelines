# Insights_Prouni

![Descrição da Imagem](https://github.com/arlen64/Insights_Prouni/blob/676cb3ded09b08c975b3b7d430ca70a4b4be150f/ImageProject_Prouni.jpeg)

Este é projeto aprensenta um estudo tendo como base dados do Prouni que visa Extrair informações<br />
de uma base de dados do 'Prouni' que se retrata do detalhamento quantitativo de bolsas concedidas pelo Prouni por ano

## Bibliotecas necessárias:

- dash
- ploty
- pandas
- sqlalchemy

## 🧐 Objetivo

Fazer um processo de etl tendo como base de dados do 'Prouni' que se retrata do detalhamento quantitaivo de bolsas concedidas pelo Prouni. <br/>

## ✨ Requisitos do desafio

Esse código pode ser usado como base para projetos mais avançados ou para entender os conceitos básicos e intermediários de processos de ETL. <br/>

Neste desafio, feito em conjunto com o [@arlen64](https://github.com/arlen64), criamos este projeto com a finalidade de realizar processos de "coleta", 'limpeza", "análise" e "visualização" de dados da **Administração Pública brasileira** tendo como requisitos:

-   Este processo poderá estático, isto é, a coleta pode ser feita em apenas uma etapa sem a necessidade de processamento dinâmico de informações;
-   A coleta normalmente será realizada processando-se um arquivo do tipo `CSV` por meio do uso do `Pandas`;
-   Deve-se realizar um tratamento para remover os dados não relevantes para o fim da aplicação ("limpeza").

-   Uso de banco de dados relacional:
    -   Uso do Postgres;
    -   Não há a necessidade de uso de Spark, bastando o uso de Pandas;
    -   Utilizar comandos SQL ou Python para o cruzamento das informações.
-   Implementar e detalhar um processamento segmentado em no mínimo 3 zonas:
    -   raw (dado cru);
    -   curated (dado limpo); e
    -   analytics (dado analisado).

## Como Usar

Para utilizar este projeto, siga os passos abaixo:

baixar o dataset que disponibilizei no link:<br/> https://dadosabertos.mec.gov.br/images/conteudo/prouni/2020/ProuniRelatorioDadosAbertos2020.csv<br/> e em seguida crie três banco de dados de forma manual no postgres. sendo eles: <br/>
raw_data, silver_data, gold_data. Por fim, passe as referências do seu banco de dados e o caminho do arquivo csv que foi baixado para o script python.

## 🛠 Tecnologias

#### **Dependências**

-   **[Python](https://docs.python.org/pt-br/3/tutorial/index.html)**
-   **[Poetry - Python dependency management and packaging made easy](https://python-poetry.org/)**
-   **[Pandas documentation](https://pandas.pydata.org/pandas-docs/stable/index.html)**
-   **[PostgreSQL: The world's most advanced open source database](https://www.postgresql.org/)**
-   **[Plotly Python Graphing Library](https://plotly.com/python/)**
-   **[Dash for Python | Plotly](https://dash.plotly.com/tutorial)**
-   **[jupyter for VsCode | Plotly](https://www.walissonsilva.com/posts/jupyter-notebook-no-visual-studio-code)**

### Resultado:

Carregamento dos dados brutos no banco de dados raw_data do postgres, carregar os dados tratados no banco silver_data e os gráficos escolhidos no banco gold_data <br/>
os dados serão consultados do banco silver_data para sim gerar as tabelas e os gráficos com as bibliotecas dash e plotly. Diante disso, serão gerados 6 gráficos com suas regras de negócios de exemplo <br/>
e ao fim do código a construção de um dashboard com todos os gráficos em uma página local.
