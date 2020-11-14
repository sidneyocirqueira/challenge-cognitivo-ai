# challenge-cognitivo-ai

Nesse repositório apresento a resolução do challenge de engenharia de dados que tem como objetivo realizar a leitura de um arquivo no formato csv, converter para um formato colunar otimizado para big data, além de realizar uma etapa de definição de tipos de dados e exportação de um dataset final conforme solicitado no arquivo [requirements](https://github.com/sidneyocirqueira/challenge-cognitivo-ai/tree/main/requirements).


## Integrantes
1. [Sidney Cirqueira](https://www.linkedin.com/in/sidneyoliveiracirqueira/)

## Pré-Requisitos:
Conhecimento basico em Azure, Big Data,Data Lake, Databricks e Spark.

* [Conta Microsoft Azure](https://azure.microsoft.com/en-us/free/); 
* [Dataset de usuários]();
* [Azure Databricks](https://azure.microsoft.com/en-us/services/databricks/);
* [Storage Account](https://docs.microsoft.com/en-us/azure/storage/common/storage-account-overview); 
* [PySpark](https://databricks.com/glossary/pyspark);

## Etapas:

# Conversão de dados
* [Notebook](https://github.com/sidneyocirqueira/challenge-cognitivo-ai/tree/main/notebooks)

Recebendo os dados da aplicação ou de qualquer outra fonte de dados e
convertendo para o tipo de arquivo mais otimizado para se trabalhar com Spark
o apache parquet é um tipo de arquivo colunar que acelera e otimiza varios formatos de arquivos,
esse modelo colunar faz integração com quase todas os frameworks de processamento de dados de big data
é extremamente utilizado juntamente com o apache spark.

Como explicado anteriormente para que você possa ganhar em otimização
é extremamente importante que você sempre realize a conversão dos tipos de dados, se estiver trabalhando com spark então definitivamente
utilize apache parquet

o Apache Spark possibilita diversos tipos de leituras diferentes, segue opções disponíveis utilizando = (spark.read.)
Parquet, JSON, CSV, ORC e JDBC

convertendo os dataframes para o apache parquet  obtemos algumas vantagens:

**1** - aceita estrutura complexas para arquivo  
**2** - eficiente para compressão e encoding de schema  
**3** - permite menos acesso ao disco e consultas mais rápidas no arquivo  
**4** - menos overhead de I/O  
**5** - aumento na velocidade de scan  

* [Notebook](https://github.com/sidneyocirqueira/challenge-cognitivo-ai/tree/main/notebooks)
* [Output](https://github.com/sidneyocirqueira/challenge-cognitivo-ai/tree/main/data/output/load.parquet)

## Conversão, deduplicação dos dados convertivos e exportação dataset final 

* [Notebook](https://github.com/sidneyocirqueira/challenge-cognitivo-ai/tree/main/notebooks)
* [Output](https://github.com/sidneyocirqueira/challenge-cognitivo-ai/tree/main/data/usersFinal.parquet)

## Notas Gerais 

O serviço escolhido foi o Azure Databricks hospedado na nuvem [Microsoft Azure](https://azure.microsoft.com/en-us/) devido minha maior expertize técnica, facilidade de deployment, integração com o datalake (storage account) e possibilidade de utilização de Pyspark para manipulação dos dados.

## Contribuição
Se você quiser contribuir, leia mais sobre tags markdown para editar o arquivo README, [Guia markdown](https://docs.microsoft.com/en-us/azure/devops/project/wiki/markdown-guidance?view=azure-devops&viewFallbackFrom=vsts) 

