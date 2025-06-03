# PROJETO FOME ZERO
Desenvolvido no curso Analisando Dados com Python da Comunidade DS

# Problema de negócio

A empresa Fome Zero é uma marketplace de restaurantes. Ou seja, seu core business é facilitar o encontro e negociações de clientes e restaurantes. Os restaurantes fazem o cadastro dentro da plataforma da Fome Zero, que disponibiliza informações como endereço, tipo de culinária servida, se possui reservas, se faz entregas e também uma nota de avaliação dos serviços e produtos do restaurante, dentre outras informações.

O CEO pediu que fosse gerado um dashboard que permitisse que ele visualizasse as principais informações das perguntas que ele fez. O CEO precisa dessas informações o mais rápido possível, uma vez que ele também é novo na empresa e irá utilizá-las para entender melhor a empresa Fome Zero para conseguir tomar decisões mais assertivas.

O trabalho é utilizar os dados que a empresa Fome Zero possui e responder as perguntas feitas do CEO e criar o dashboard solicitado.

## Geral
1. Quantos restaurantes únicos estão registrados? 
2. Quantos países únicos estão registrados?
3. Quantas cidades únicas estão registradas?
4. Qual o total de avaliações feitas?
5. Qual o total de tipos de culinária registrados?

## País
1. Qual o nome do país que possui mais cidades registradas?
2. Qual o nome do país que possui mais restaurantes registrados?
3. Qual o nome do país que possui mais restaurantes com o nível de preço igual a 4 registrados?
4. Qual o nome do país que possui a maior quantidade de tipos de culinária distintos?
5. Qual o nome do país que possui a maior quantidade de avaliações feitas?
6. Qual o nome do país que possui a maior quantidade de restaurantes que fazem entrega?
7. Qual o nome do país que possui a maior quantidade de restaurantes que aceitam reservas?
8. Qual o nome do país que possui, na média, a maior quantidade de avaliações registrada?
9. Qual o nome do país que possui, na média, a maior nota média registrada? 
10. Qual o nome do país que possui, na média, a menor nota média registrada? 
11. Qual a média de preço de um prato para dois por país?

## Cidade
1. Qual o nome da cidade que possui mais restaurantes registrados?
2. Qual o nome da cidade que possui mais restaurantes com nota média acima de 4?
3. Qual o nome da cidade que possui mais restaurantes com nota média abaixo de 2.5?
4. Qual o nome da cidade que possui o maior valor médio de um prato para dois?
5. Qual o nome da cidade que possui a maior quantidade de tipos de culinária distintas?
6. Qual o nome da cidade que possui a maior quantidade de restaurantes que fazem reservas?
7. Qual o nome da cidade que possui a maior quantidade de restaurantes que fazem entregas?
8. Qual o nome da cidade que possui a maior quantidade de restaurantes que aceitam pedidos online?

## Restaurantes
1. Qual o nome do restaurante que possui a maior quantidade de avaliações?
2. Qual o nome do restaurante com a maior nota média?
3. Qual o nome do restaurante que possui o maior valor de uma prato para duas pessoas?
4. Qual o nome do restaurante de tipo de culinária brasileira que possui a menor média de avaliação?
5. Qual o nome do restaurante de tipo de culinária brasileira, e que é do Brasil, que possui a maior média de avaliação?
6. Os restaurantes que aceitam pedido online são também, na média, os restaurantes que mais possuem avaliações registradas?
7. Os restaurantes que fazem reservas são também, na média, os restaurantes que possuem o maior valor médio de um prato para duas pessoas?
8. Os restaurantes do tipo de culinária japonesa dos Estados Unidos da América possuem um valor médio de prato para duas pessoas maior que as churrascarias americanas (BBQ)?

## Tipos de Culinária
1. Dos restaurantes que possuem o tipo de culinária italiana, qual o nome do restaurante com a maior média de avaliação?
2. Dos restaurantes que possuem o tipo de culinária italiana, qual o nome do restaurante com a menor média de avaliação?
3. Dos restaurantes que possuem o tipo de culinária americana, qual o nome do restaurante com a maior média de avaliação?
4. Dos restaurantes que possuem o tipo de culinária americana, qual o nome do restaurante com a menor média de avaliação?
5. Dos restaurantes que possuem o tipo de culinária árabe, qual o nome do restaurante com a maior média de avaliação?
6. Dos restaurantes que possuem o tipo de culinária árabe, qual o nome do restaurante com a menor média de avaliação?
7. Dos restaurantes que possuem o tipo de culinária japonesa, qual o nome do restaurante com a maior média de avaliação?
8. Dos restaurantes que possuem o tipo de culinária japonesa, qual o nome do restaurante com a menor média de avaliação?
9. Dos restaurantes que possuem o tipo de culinária caseira, qual o nome do restaurante com a maior média de avaliação?
10. Dos restaurantes que possuem o tipo de culinária caseira, qual o nome do restaurante com a menor média de avaliação?
11. Qual o tipo de culinária que possui o maior valor médio de um prato para duas pessoas?
12. Qual o tipo de culinária que possui a maior nota média?
13. Qual o tipo de culinária que possui mais restaurantes que aceitam pedidos online e fazem entregas?

# Premissas do negócio
A análise foi realizada com dados contendo informações dos restaurantes, entregadores e avaliações dos clientes.

Marketplace de restaurantes foi o modelo de negócio assumido.

Não foi levada em consideração a variação cambial, na comparação dos valores dos restaurantes entre os países.

As 4 principais visões do negócio foram: 
- Mapa com a localização dos restaurantes cadastrados
- Visão Países
- Visão Cidades
- Visão Cozinhas

# Estratégia da solução
A abordagem envolveu a análise de dados em um Jupyter Notebook para responder às questões levantadas pelo CEO.
Com base nas informações consideradas mais relevantes, desenvolvemos um dashboard interativo usando Streamlit.
O painel estratégico foi desenvolvido utilizando as métricas que refletem as 4 principais visões do modelo de negócio da empresa:
1. Mapa com a localização dos restaurantes
2. Visão dos restaurantes por parís
3. Visão dis restaurantes por cidade
4. Visão por Tipo de Cozinhas

Cada visão é representada pelo seguinte conjunto de métricas.

## 1. Mapa
1. Localização dos restaurantes
2. Nome do restaurante
3. Preço da refeição para 2 pessoas
4. Tipo de culinária
5. Nota de avaliação

## 2. Visão dos restaurantes por parís
1. Quantidade de restaurantes registrados por país
2. Quantidade de cidades registrados por país
3. Média de avaliação feita por país
4. Média de preço de prato para duas pessoas por país

## 3. Visão dis restaurantes por cidade
1. Top 10 cidades com mais restaurantes na base por país
2. Top 7 Cidades com mais Restaurantes com Média de Avaliação acima de 4
3. Top 7 Cidades com mais Restaurantes com Média de Avaliação abaixo de 2.5
4. Top 10 Cidades mais restaurantes com tipos culinários distintos

## 4. Visão por Tipo de Cozinhas
1. Melhores Restaurantes dos Principais tipos Culinários com a maior nota de avaliação
2. Top 10 Restaurantes
3. Top 10 melhores tipos de culinárias
4. Top 10 piores tipos de culinárias

# 4. Top 3 Insights de dados 
1. A Índia é o país que mais se sobressai na maioria dos indicadores analisados. Ela lidera em quantidade de cidades e restaurantes cadastrados, diversidade de culinárias e número de avaliações, entre outros.
2. Já o Brasil se diferencia por apresentar a menor média de avaliações.
3. Entre as três cidades brasileiras no conjunto de dados (São Paulo, Brasília e Rio de Janeiro), o Rio de Janeiro se destaca nas avaliações. A cidade carioca possui mais restaurantes com notas acima de 4 do que São Paulo e Brasília.


# 5. O produto final do projeto 
Painel online, hospedado em um Cloud e disponível para acesso em
qualquer dispositivo conectado à internet.
O painel pode ser acessado através desse link: [Projeto Fome Zero](https://ale-cds-ftc-projeto-do-aluno.streamlit.app)

# 6. Conclusão

O objetivo desse projeto é criar um conjunto de gráficos e/ou tabelas que exibam essas métricas da melhor forma possível para o CEO.

Da visão Países, podemos concluir que o número de restaurantes registrados é maior na Índia e a Indonesia possui, na média, a maior nota média registrada.

# 7. Próximo passos
1. Implementar filtros adicionais: Isso permitirá análises mais detalhadas, atendendo às necessidades específicas do CEO.
2, Investigar a baixa média de avaliação: É importante aprofundar a análise para entender as causas da baixa pontuação dos restaurantes brasileiros.
3. Incluir um botão de download: Adicionar uma funcionalidade para que o CEO possa baixar os dados já processados e utilizados na análise.