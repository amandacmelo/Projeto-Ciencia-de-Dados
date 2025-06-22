# Projeto Ciência de Dados - Um conjunto de dados estatísticos socioeconômicos de cidades brasileiras

  Para a realização do projeto da disciplina de Introdução à Ciência de Dados, será desenvolvido um processamento sobre um conjunto de dados socioeconômicos abrangente dos municípios brasileiros. Além disso, a equipe fará comparações desses dados com diferentes questões de economia, pandemia de Covid-19 e o impacto dos governos no período de coleta. A base de dados provém do BRStats, que inclui dados de várias fontes públicas brasileiras, como IBGE, DataSus e IPEA. Para além desses dados, a equipe optou por utilizar outros datasets para enriquecer e realizar extração de dados, que serão discutidos ao longo do processo.

## ATIVIDADES REALIZADAS

[🟡 QUESTÕES A SEREM VALIDADAS ](#-questões-a-serem-validadas)

[🟢 PREPARAÇÃO DO DADOS](#-preparação-do-dados)

[🔴 ANÁLISE EXPLORATÓRIA DOS DADOS](#-análise-exploratória-dos-dados)

[🟠 INFERÊNCIA ESTATÍSTICA E REGRAS DE ASSOCIAÇÃO](#-inferência-estatística-e-regras-de-associação)

[🟤 REGRESSÃO LINEAR](#-regressão-linear)

[⚪ APRENDIZADO SUPERVISIONADO E NÃO-SUPERVISIONADO](#-aprendizado-supervisionado-e-não-supervisionado)

[🟣 ORGANIZAÇÃO](#-organização)

[🔵 AUTORES](#-autores)


# 🟡 QUESTÕES A SEREM VALIDADAS:
  As perguntas formuladas e discutidas pela equipe são as seguintes, contemplando os seguintes eixos:
  ### 🐮🌱 Produção pecuária e agricola:

   1) Como a pandemia da COVID-19 afetou as cidades em que grande parte da renda era em torno do turismo?
   
   2) Há evidência de que municípios com maior valor de produção pecuária também apresentam maior PIB?
   
   3) Como a pandemia de COVID-19 afetou a relação entre a produção agrícola e pecuária?
   
   4) De que maneira a produção e exportação de tais insumos primários impacta na qualidade de vida da população dos municípios descritos no dataset?
   
   5) Municípios com maior produção agrícola tendem a ter maior área desmatada?
   
   6) Quais fatores e aspectos que mais influenciam a produção agrícola?
      
### 💸🗃 Economia e empregabilidade:

  7) De que maneira o investimento público nos Municípios afeta a empregabilidade destes? Cidades que recebem mais transferências (dinheiro) geram mais empregos?
  
  8) Cidades e regiões com maior população possuem um PIB per capita mais alto em relação aos demais? Como o crescimento enconômico de uma região se relaciona com sua população?

  9) Municípios com maior proporção de pessoal assalariado apresentam um PIB per capita significativamente diferente dos demais?

### 📦💰 Dependência financeira dos municípios, relação das transferências e exportações:

  10)  Existe relação entre maior PIB municipal, maior receita própria e menor dependência de transferências correntes e de capital, e o índice de autonomia financeira nos municípios?
  
  11) Existe uma correlação entre as exportações e a produção agrícola e pecuária? Regiões com maior foco nas exportações também são aquelas com maior concentração de atividades do agronegócio?


# 🟢 PREPARAÇÃO DO DADOS: 
  Após a definição da temática principal que será abordade no projeto, foi realizada a preparação dos dados, buscando entender os atributos dos objetos, a tipagem dos atributos, além de identificar e tratar possíveis ruídos ou ausência de informações. Por fim, realizou-se a limpeza dos dados que foram considerados desnecessários para as futuras análises.
  
  Desse modo, para o tratamento de dados a equipe realizou:
  
  
  1)   Verificação dos atributos
  2)   Verificação do período de análise
  3)   Ajuste nos tipos de atributos e valores de ponto flutuante: realizou-se a transformação dos atributos para seus tipos corretos, uma vez que a grande maioria estava definida como 'object' no conjunto de dados analisado.
  4)  Tratamento dos dados referentes receita, exportação e importação: retirada dos objetos com valores vazios.
  5)  Transformação de todos os valores 'nan' em 0.
  6)  Preenchimento de valores ausentes
  7)  Retirada de atributos
  8)  Criação de novos atributos: utilizando os dados fornecidos por esse dataset, também construímos novos atributos para facilitar futuras análises.
  9)  Análises dos dados em busca de ruidos/outliers.
     
  A visualização dos tratamentos realizados pode ser acessada em: [Preparacao_dos_dados.ipynb](Preparacao_dos_dados.ipynb)

# 🔴 ANÁLISE EXPLORATÓRIA DOS DADOS: 
  Após a preparação dos dados, nesta etapa foram geradas estatísticas descritivas, gráficos e tabelas a fim de conhecer os dados. Cada integrante, responsável pela formulação das perguntas em sua respectiva área, trabalhou com os dados e análises correspondentes às perguntas que elaborou. Desse modo, os notebooks estão separados de acordo com as áreas trabalhadas, sendo elas: produção pecuária e agrícola, economia e empregabilidade, e dependência financeira dos municípios, relação das transferências e exportações. Os arquivos estão disponíveis na pasta Análise Exploratória dos Dados ou podem ser acessados individualmente nos seguintes documentos:
  
  🔸  [ Atividade Agrícola e Impacto do Covid-19](Análise%20Exploratória%20dos%20Dados/Análise_exploratória_dos_dados_Atividade_agrícola_e_Impacto_do_Covid_19.ipynb)
  
  🔸  [Atividade Agrícola, Pecuária e Qualidade da Água](Análise%20Exploratória%20dos%20Dados/Análise_exploratória_dos_dados_Atividade_agrícolas_e_pecuarias.ipynb)
  
  🔸  [Economia e Empregabilidade](Análise%20Exploratória%20dos%20Dados/Análise_exploratória_dos_dados_Economia.ipynb)
  
  🔸  [Dependência Financeira, Transferências e Exportações](Análise%20Exploratória%20dos%20Dados/Análise_exploratória_dos_dados_Dependência_financeira,_transferências_e_exportaçõesipynb.ipynb)

# 🟠 INFERÊNCIA ESTATÍSTICA E REGRAS DE ASSOCIAÇÃO     

Nesta etapa, o grupo deu continuidade à análise dos dados por meio da aplicação de técnicas de inferência estatística e algoritmos de regras de associação, com o objetivo de aprofundar a investigação de aspectos relevantes identificados na fase exploratória. A partir de novas indagações surgidas durante a análise, foi elaborada uma nova pergunta de pesquisa voltada à investigação de possíveis relações entre variáveis. Com isso, foram aplicados testes estatísticos para avaliar a significância dos padrões observados e, em paralelo, utilizou-se um algoritmo de regras de associação para extrair combinações de variáveis com maior ocorrência conjunta nos dados. Os resultados dessas análises foram interpretados e discutidos, contribuindo para uma compreensão mais robusta dos fenômenos observados. As análises estão organizadas na pasta:
[**Inferência Estatística e Regras de Associação**](./Infer%C3%AAncia%20Estat%C3%ADstica%20e%20Regras%20de%20Associa%C3%A7%C3%A3o)

# 🟤 REGRESSÃO LINEAR 
Após a realização da inferência estatística e da aplicação das regras de associação, a equipe deu continuidade ao processo de resposta às perguntas formuladas por meio da utilização da regressão linear, com o objetivo de investigar as relações entre as variáveis envolvidas, aprofundando a compreensão dessas relações e avaliando a significância estatística das variáveis explicativas e seu impacto. Para isso, foram realizados testes e análises que permitiram identificar quais fatores exercem maior influência e contribuem para explicar as indagações levantadas, possibilitando, assim, a formulação de conclusões fundamentadas a partir dos dados disponíveis. Os resultados foram interpretados e discutidos, e podem ser acessados na pasta:
[**Regressão Linear**](./Regress%C3%A3o%20Linear/)


# ⚪ APRENDIZADO SUPERVISIONADO E NÃO-SUPERVISIONADO

Nesta etapa, o grupo aplicou algoritmos de aprendizado supervisionado e não-supervisionado com o objetivo de compreender certas relações e avaliar a possibilidade de prever atributos específicos. Para isso, foram utilizados algoritmos não-supervisionados para a geração de agrupamentos (clusterização) e algoritmos supervisionados para realizar previsões e classificações. O estudo concentrou-se na área socioeconômica, empregando atributos dessa natureza para prever o PIB de um município em determinado ano, assim como o número de nascimentos. Os resultados obtidos foram analisados e discutidos, e podem ser encontrados na pasta:[**Aprendizado Supervisionado e Não Supervisionado**](./Aprendizado%20Supervisionado%20e%20N%C3%A3o%20Supervisionado/)

  
# 🟣 ORGANIZAÇÃO

### ◽ENTREGA 1: 
  Para a elaboração das perguntas e preparação dos dados, a equipe se reuniu em horários extraclasse e durante as aulas práticas. Dessa forma, as tarefas da primeira etapa foram divididas da seguinte maneira:
  
  1) Caio: Elaboração de três perguntas relacionadas à agropecuaria e análises dos dados em busca de ruidos/outliers.

  2) Leticia: Elaboração de duas perguntas relacionadas à agropecuaria, ajuste nos tipos de atributos e valores de ponto flutuante.

  3) Melissa: Elaboração de três perguntas relacionadas à economia e empregabilidade e criação de novos atributos, com objetivo de auxiliar em análises futuras.

  4) Amanda: Elaboração de duas perguntas relacionadas à transferências aos municípios e suas relações, além de exportações e analise e tratamento dos dados referentes receita, exportação e importação.

### ◽ENTREGA 2:
  Para a etapa de Análise Exploratória de Dados, as tarefas foram divididas da seguinte maneira:

1) Caio: Responsável pela análise exploratória da área de produção pecuária e agrícola.

2) Letícia: Atuou na mesma área de produção pecuária e agrícola, utilizando um dataset externo.

3) Melissa: Responsável pela análise exploratória dos dados relacionados à economia e empregabilidade.

4) Amanda: Responsável pela análise exploratória dos dados da área de dependência financeira dos municípios, com foco em transferências governamentais, exportações e receitas municipais.

### ◽ENTREGA 3:
  Para a entrega referente à Inferência Estatística e Regras de Associação, as tarefas foram designadas da seguinte forma:

1) Caio: Responsável pela Inferência Estatística e Regra de Associação da área de Turismo, para a pergunta 1

2) Letícia: Responsável pela Inferência Estatística e Regra de Associação da área de Agropecuária, por meio da criação de duas novas perguntas

3) Melissa: Responsável pela criação de uma Regra de Associação para a pergunta 7.

4) Amanda: Responsável pela Inferência Estatística da área de Economia e Empregabilidade a partir da criação de uma nova pergunta

### ◽ENTREGA 4:
  Para a entrega referente à Regressão Linear, as tarefas foram dividas da seguinte maneira:

1) Caio: Responsável pela aplicação da Regressão na área Agrícola, como em em análises multivariaveis para análises de Valor de produção Agrícola

2) Letícia:  Responsável pela aplicação da Regressão na área Agrícola,com foco em desmatamento

3) Melissa: Responsável pela aplicação da Regressão na área da Economia, como em Transferências de Capital vs Empregabilidade, além do Produto Interno Bruto (PIB) vs População

4) Amanda: Responsável pela Regressão da área de Economia e Empregabilidade e da Dependência Financeira dos municípios

### ◽ENTREGA 5:
  Para a entrega referente à aplicação de algoritmos de aprendizando supervisionado e não-supervisionado, as tarefas foram dividas desse modo:

1) Caio:

2) Letícia:  

3) Melissa: 

4) Amanda: Responsável pela criação de um modelo supervisionado na área da economia


# 🔵 AUTORES:

  Amanda Caroline Melo Assunção - 5366

  Caio Menezes Oliveira - 5784

  Letícia Cristina Almeida da Silva - 5781

  Melissa Alanis Santos Oliveira - 5384
