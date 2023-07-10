# Full Cycle 3 - Observability

## Observabilidade

Na teoria de controle, a observabilidade eh definida como u ma medida de quao bem os estados
internos de um sistema podem ser definidos a partir do conhecimento das saidas externas desse sistema. Simplificando,
obsevabilidade e quao bem voce entender do seu sistema complexo.

## Observabilidade x Monitoriamento

- Monitoriamento nos mostra que ha algo de errado

- Monitoriamento se baseia em saber com antecedencia quais sinais voce deseja monitorar

- Observabilidade nos permite perguntar o porque (porque a memoria esta tao alta)

## Os 3 pilares da observabilidade

- Metricas (CPU esta em 90%)

- Logs

- Tracing (ordem de como o evento foi gerado)

## Elastic Stack

### Visao geral

- Elasticsearch
  - Search engine e analytics
- Logstash
  - Processador de dados atraves de pipelines que consegue receber, transformar e enviar simultaneamente
- Kibana
  - Permite usuarios a visualizarem os dados do elasticsearch em diversas perspectivas

### Elastic

- Search engine e analytics
- Apache Lucene
- 2010 - Elasticsearch N.V (Elastic)
- Rapido
- Escalavel
- API Rest
- Analise e visualizacao geoespacial
- Application, website e enterprise search
- Logging e analytics
- Trabalha de forma distribuida atraves de shards que possuem redundancia de dados
- Pode escalar milhares de servidores e manipular petabyte de dados

### Logstash

- Engine coletora de dados em tempo real
- Iniciou como manipulador de logs
- Trabalha com pipelines
- Recebe dados de multiplas fontes
- Normaliza e transforma dados
- Envia dados para multiplas fontes
- Plugins

### Kibana

- Ferramenta de visualizacao e exploracao de dados
- Usada com: Logs, analise de series, monitoriamento de aplicacoes e inteligencia operacional
- Integrado com Elasticsearch
- Agregadores e filtragem de dados
- Dashboards
- Graficos interativos
- Mapas

## Qual a diferenca entre ELK Stack e Elastic Stack?

### Beats

- Beats foi anunciado em 2015
- "Lightweight data shipper"
- Agente coletor de dados
- Logs, metricas, network data, audit data, uptime monitoring
- Voce pode construir seu proprio Beat
- Quando falamos de Elastic Stack, falamos de: Kibana, Elasticsearch, Beats e Logstash

### Elastic

- Empresa por tras das solucoes
- Cloud Solution
- Oferece plugins e recursos licenciados
- Produtos
  - APM
  - Maps
  - Site search
  - Enterprise search
  - App search
  - Infrastructure

### Iniciando com Elasticsearch e Kibana

- usuarios linux comandos:
  ```
  docker network create observability
  ```
  ```
  mkdir elasticsearch_data
  ```
  ```
  sudo sysctl -w vm.max_map_count=262144
  ```
  ```
  docker-compose up -d
  ```
