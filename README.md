# Projeto Ciência de Dados - Um conjunto de dados estatísticos socioeconômicos de cidades brasileiras

# -> Descrição:
  Para a realização do projeto da disciplina de Introdução à Ciência de Dados, será desenvolvido um processamento sobre um conjunto de dados socioeconômicos abrangente dos municípios brasileiros. Além disso, a equipe fará comparações desses dados com diferentes questões de economia, pandemia de Covid-19 e o impacto dos governos no período de coleta. A base de dados provém do BRStats, que inclui dados de várias fontes públicas brasileiras, como IBGE, DataSus e IPEA. Para além desses dados, a equipe optou por utilizar outros datasets para enriquecer e realizar extração de dados, que serão discutidos ao longo do processo.

# -> Participantes:

  Amanda Caroline Melo Assunção - 5366

  Caio Menezes Oliveira - 5784

  Letícia Cristina Almeida da Silva - 5781

  Melissa Alanis Santos Oliveira - 5384

# -> Divisão de tarefas:
  Para a elaboração das perguntas e preparação dos dados, a equipe se reuniu em horários extraclasse e durante as aulas práticas. Dessa forma, as tarefas da primeira etapa foram divididas da seguinte maneira:
  
  1) Caio: Elaboração de três perguntas relacionadas à agropecuaria e análises dos dados em busca de ruidos/outliers.

  2) Leticia: Elaboração de duas perguntas relacionadas à agropecuaria, ajuste nos tipos de atributos e valores de ponto flutuante.

  3) Melissa: Elaboração de três perguntas relacionadas à economia e empregabilidade e criação de novos atributos, com objetivo de auxiliar em análises futuras.

  4) Amanda: Elaboração de duas perguntas relacionadas à transferências aos municípios e suas relações, além de exportações e analise e tratamento dos dados referentes receita, exportação e importação.

# -> Preparação dos Dados: 
  Após a definição da temática principal que abordaremos em nosso projeto, realizamos a preparação dos dados, buscando entender os atributos dos objetos, a tipagem dos atributos, além de identificar e tratar possíveis ruídos ou ausência de informações. Por fim, realizamos a limpeza dos dados que consideramos desnecessários para nossas futuras análises.
  
  Desse modo, para o tratamento de dados realizamos:
  
  1)  Ajuste nos tipos de atributos e valores de ponto flutuante: realizamos a transformação dos atributos para seus tipos corretos, uma vez que a grande maioria estava definida como 'object' no conjunto de dados analisado.
  2)  Tratamento dos dados referentes receita, exportação e importação: retirada dos objetos com valores vazios.
  3)  Transformação de todos os valores 'nan' em 0.
  4)  Criação de novos atributos: utilizando os dados fornecidos por esse dataset, também construímos novos atributos para facilitar futuras análises.
  5)  Análises dos dados em busca de ruidos/outliers.
     
  A visualização dos tratamentos realizados pode ser acessada pelo link: https://colab.research.google.com/drive/1ztOUOMFKtLA2Oix2uHLVwv6P7I3TrAyu?usp=sharing ou pelo arquivo Preparacao_dos_dados.ipynb.
  
# -> Perguntas:
  As perguntas formuladas e discutidas pela equipe são as seguintes, contemplando os seguintes eixos:
  # Produção pecuária e agricola:

   1) Como a pandemia da COVID-19 afetou as cidades em que grande parte da renda era em torno do turismo?

  2) Como a mudança da presidência e de outros poderes do governo federal no ano de 2018 afetou a produção pecuária e agricula nos anos seguintes?

  3) De que maneira a produção e exportação de tais insumos primários impacta na qualidade de vida da população dos municípios descritos no dataset?

  4) Estados com maior volume de atividades agropecuárias tendem a ter piores índices de perda e qualidade da água? (Usar o dataset do Diagnóstico dos Serviços de Água e Esgotos do Ministério das Cidades)
  
  5) Como a pandemia de COVID-19 afetou a relação entre a produção agrícola e pecuária?

# Economia e empregabilidade:

  6) De que maneira o investimento público nos Municípios afeta a empregabilidade destes? Cidades que recebem mais transferências (dinheiro) geram mais empregos?
  
  7) O crescimento econômico de uma cidade/região possui relação com o seu povoamento? Cidades e regiões mais densamente povoadas possuem um PIB maior? Além disso, elas geram mais empregos?

   8) Como a pandemia da COVID-19 afetou as cidades em que grande parte da renda era em torno do turismo?

# Dependência financeira dos municípios, relação das transferências e exportações:

  9) Existe uma relação entre o PIB municipal e a receita tributária, com uma menor dependência de transferências e um maior índice de autonomia financeira nos municípios? (Utilizar dados do Siconfi para análise)
  
  10) Como funciona o processo de exportação no Brasil? O que é exportado dentro dos limites federais e o que é destinado a outros países? Quais setores dominam as exportações brasileiras e como eles se relacionam com a produção agrícola e pecuária? (Utilizar dados externos, possivelmente de COMEX STAT - MDIC)
