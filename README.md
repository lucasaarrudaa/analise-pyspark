# analise-pyspark
 
Objetivos:
O objetivo do projeto foi explorar os dados de amostra disponíveis no IMDB usando o Apache Spark e a API de Dataframes do Spark. Foi realizada uma análise exploratória dos dados para responder a algumas perguntas sobre os filmes, como gênero de títulos mais frequente, quantidade de títulos de filmes diferentes, duração média dos filmes com conteúdo adulto, quantidade de filmes com título atual diferente do título original, nome mais longo de filme, filme com a maior quantidade de votos e a menor nota média de um filme.

Análise:
Para realizar a análise dos dados, os arquivos "title_basics.tsv" e "title_ratings.tsv" foram lidos usando a API de Dataframes do Spark. Em seguida, foram realizadas as seguintes análises:

Qual o gênero de títulos mais frequente?
Para responder a essa pergunta, foi criado um novo dataframe agrupando os dados por gênero e contando o número de títulos em cada gênero. Em seguida, os dados foram ordenados em ordem decrescente para encontrar o gênero mais frequente.

Quantos títulos de filmes diferentes existem?
Foi criado um novo dataframe contendo apenas os títulos únicos dos filmes e, em seguida, foi contado o número de títulos no dataframe.

Qual a duração média dos filmes com conteúdo adulto?
Foi criado um novo dataframe contendo apenas os filmes com classificação etária de "adulto" e, em seguida, foi calculada a duração média desses filmes.

Quantos filmes têm o título atual (“primary”) diferente do título original?
Foi criado um novo dataframe contendo apenas os filmes cujo título atual é diferente do título original e, em seguida, foi contado o número de filmes no dataframe.

Qual o filme que tem o nome mais longo?
Foi criado um novo dataframe ordenando os dados por comprimento do título em ordem decrescente e, em seguida, o primeiro registro no dataframe foi selecionado para obter o nome do filme mais longo.

Qual filme tem a maior quantidade de votos?
Foi criado um novo dataframe ordenando os dados por quantidade de votos em ordem decrescente e, em seguida, o primeiro registro no dataframe foi selecionado para obter o filme com a maior quantidade de votos.

Qual é a menor nota média de um filme?
Foi criado um novo dataframe contendo apenas os filmes com nota média atribuída e, em seguida, foi calculada a nota média mínima desses filmes.

Conclusão:
O projeto usou a API de Dataframes do Spark para explorar os dados de amostra disponíveis no IMDB. A análise dos dados permitiu responder às perguntas sobre os filmes e extrair informações relevantes sobre o conjunto de dados. A utilização do Spark permitiu que a análise fosse executada de forma rápida e escalável, mesmo para arquivos de tamanho grande, como os utilizados neste projeto.
