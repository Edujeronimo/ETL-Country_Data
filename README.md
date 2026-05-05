# Country Data 

Projeto de engenharia de dados baseado em um ETL (Extract, Transform, Load) para processamento de um arquivo JSON contendo informações sobre países e continentes.

Desenvolvido utilizando o conceito de arquitetura Medallion (Bronze, Silver, Gold) no Databricks, com foco em organização, qualidade e consumo dos dados.

#Bronze (Ingestão - ING)
Responsável pela ingestão dos dados brutos

Dados armazenados exatamente como foram recebidos (JSON)

Nenhum tratamento é aplicado nesta camada


Objetivo: garantir rastreabilidade e histórico

# Silver (Refined / Trusted)
Camada de tratamento e padronização dos dados

Aplicação de:
Limpeza de dados,
Normalização de colunas,
Tratamento de nulos e
Estruturação dos dados

# Gold (Consumption / UCS)
Camada final para consumo analítico

Dados preparados para BI e visualização

Estrutura otimizada para consultas

Possíveis usos:
Dashboards no Power BI,
Consultas analíticas,
Agregações (ex: países por continente)