# ANTT-Amostra-Estratificada

Exemplo de análise de dados com amostra aleatória estratificada. Feito para o desafio data glow up #18

Este repositório contém dados de 2019 e 2020 da ANTT, obtidos em https://www.kaggle.com/danlessa/brazil-interstate-bus-travels ;

O repositório contém mais de nove milhões de observações;

Pensando nisso, minha proposta foi fazer um teste de análise de dados com amostra aleatória estratificada e verificar os resultados;

Usei aprox. 15% do conjunto de dados (aprox. 1,6 milhão de registros) para a amostra, estratificando-os por ano e por UF.

No final, comparei os resultados com o de outros colegas do desafio.

O faturamento teve um resultado surpreendentemente positivo, com precisão proporcional de 95,6% (1,4 bi do dataset total x 148 mi da amostra, variação de 10.4%)
Todos os maiores valores das análises qualitativas foram correspondentes (100%) aos resultados das outras dashboards, mas valeria a pena aprofundar mais nos números e averiguar a diferença entre eles.
O ticket médio não correspondeu ao valor apresentado pelos outros participantes do desafio, então vale averiguar a existência de um método mais confiável para esse caso.

## Sobre o dashboard

O dashboard foi construído em três partes:

### Visão geral

* Página com principais estatísticas, como faturamento total, ticket médio, principal empresa de transporte;
* Mapa com o número de viagens e o ticket médio por cada um dos pontos de origem (agrupados por UFs)

### Frequências

* Página com principais gráficos de frequências (mapa de calor) com os meses, dias e horários (drill down) para emissão dos bilhetes e para as viagens
* Análises das principais variáveis qualitativas (Principal linha de ônibus, serviço mais contratado, serviço menos contratado etc)
* Algumas estatísticas (viagens, ticket médio, faturamento) que podem ser analisadas com filtragem por variável qualitativa ou por alguma frequência ou período de tempo específico.

### Estadual

* Gráfico de mapa com filtro por estado, onde é possível ver os 5 maiores destinos de qualquer estado. Também é possível filtrar por mais de uma variável para ver os 5 maiores destinos das regiões filtradas.
* Estatística com a principal linha dos filtros ativados.
