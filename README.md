# expedia

A Expedia forneceu registros do comportamento do cliente. Isso inclui o que os clientes pesquisaram, como eles interagiram com os resultados da pesquisa (clique/reserva), se o resultado da pesquisa foi ou não um pacote de viagem. Os dados são uma seleção aleatória da Expedia e não são representativos das estatísticas gerais.

A Expedia está interessada em prever qual grupo de hotéis um usuário irá reservar. A Expedia possui algoritmos internos para formar clusters de hotéis, onde hotéis semelhantes para uma pesquisa (com base no preço histórico, classificação por estrelas do cliente, localizações geográficas relativas ao centro da cidade, etc.) são agrupados. Esses clusters de hotéis servem como bons identificadores para quais tipos de hotéis as pessoas vão reservar, evitando valores discrepantes, como novos hotéis que não possuem dados históricos.

Seu objetivo nesta competição é prever o resultado da reserva (grupo de hotéis) para um evento de usuário, com base em sua pesquisa e outros atributos associados a esse evento de usuário.

Os conjuntos de dados de treinamento e teste são divididos com base no tempo: dados de treinamento de 2013 e 2014, enquanto os dados de teste são de 2015. Os dados do placar público/privado também são divididos com base no tempo. Os dados de treinamento incluem todos os usuários nos logs, incluindo eventos de clique e eventos de reserva. Os dados de teste incluem apenas eventos de reserva.

Os dados de destinations.csv consistem em recursos extraídos do texto de avaliações de hotéis.

Observe que alguns srch_destination_id's nos arquivos train/test não existem no arquivo destinations.csv. Isso ocorre porque alguns hotéis são novos e não possuem recursos suficientes no espaço latente. Seu algoritmo deve ser capaz de lidar com essa falta
