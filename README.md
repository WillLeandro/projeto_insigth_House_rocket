<div align="center">
<img src="https://user-images.githubusercontent.com/92799101/155856910-c5ac35e9-d220-4533-9bad-ce47699450e6.png" width="800px" />
</div>

<!--- <img width="1360" alt="b8301210-f45f-11ea-8507-71ed316973d3-How-to-Find-Out-How-Much-a-House-Sold-For" src="https://user-images.githubusercontent.com/92799101/155856910-c5ac35e9-d220-4533-9bad-ce47699450e6.png"> --->
<br>
<br>
Este é um projeto fictício com a finalidade de expor minhas habilidades e competências de um analista e cientista de dados, a empresa e perguntas de negócios não são reais.
Este projeto segue as recomendações do blog <a href="https://sejaumdatascientist.com/os-5-projetos-de-data-science-que-fara-o-recrutador-olhar-para-voce">Seja um datascientist</a>.
<br><br><br>


O objetivo deste projeto é o cientista de dados fornecer ao time de negócio da house Rocket, uma seleção de imóveis, para que possam aplicar seu modelo de 
monetização que, para House Rocket a melhor estratégia de negócio é comprar imoveis de menor valor em boas condições com ótima localização e revende-los por um valor
mais alto.
Os insigths aqui encontrados visam trazer um valor de lucro máximo a empresa, dentro do portifólio de imóveis a venda.
<br><br>

### 1 - Questão de negócio
<br>
O CEO da House Rocket me procurou para ajudá-lo a encontrar bons imóveis para comprar, como isso me apresentou as seguintes perguntas:<br><br>

**1.** Quais imóveis a House Rocket deveria comprar e por qual preço de compra?<br>
**2.** Uma vex o imóvel em posse da empresa, qual o melhor momento para vendê-lo e qual seria o preço da venda?
<br><br>
### 2 - Sobre os dados

Os dados para este projeto podem ser encontrados no Kaggle clicando [aqui](https://www.kaggle.com/harlfoxem/housesalesprediction/discussion/207885).<br>
Abaixo segue a definição para cada um dos 21 atributos:<br><br><br>
| **Atributos** |  **Significado**  |
| ------------------- | ------------------- |
|  id | Numeração única de identificação de cada imóvel |
|  date |  Data de venda do imóvel |
|  price |  Preço que a casa está sendo vendida pelo proprietário |
|  bedrooms |  Número de quartos |
|  bathrooms |  Número de banheiros (0.5 = banheiro em um quarto, mas sem chuveiro) |
|  sqft_living |  Medida (em pés quadrado) do espaço interior dos apartamentos |
|  sqft_lot |  Medida (em pés quadrado)quadrada do espaço terrestre |
|  floors |  Número de andares do imóvel |
|  waterfront |  Variável que indica a presença ou não de vista para água (0 = não e 1 = sim) |
|  view |  Um índice de 0 a 4 que indica a qualidade da vista da propriedade. Varia de 0 a 4, onde: 0 = baixa 4 = alta |
|  condition |  Um índice de 1 a 5 que indica a condição da casa. Varia de 1 a 5, onde: 1 = baixo |-| 5 = alta |
|  grade |  Um índice de 1 a 13 que indica a construção e o design do edifício. Varia de 1 a 13, onde: 1-3 = baixo, 7 = médio e 11-13 = alta |
|  sqft_basement |  A metragem quadrada do espaço habitacional interior acima do nível do solo |
|  yr_built |  Ano de construção de cada imóvel |
|  yr_renovated |  Ano de reforma de cada imóvel |
|  zipcode |  CEP da casa |
|  lat |  Latitude |
|  long |  Longitude |
|  sqft_livining15 |  Medida (em pés quadrado) do espaço interno de habitação para os 15 vizinhos mais próximo |
|  sqft_lot15 |  Medida (em pés quadrado) dos lotes de terra dos 15 vizinhos mais próximo |

### 3 - Premissas do negócio

As premissas adotadas para este projeto:
- O valor igual a zero em **yr_renovated** são casas que não foram reformadas.
- O valor igual a 33 em **bathroom** foi considerado um erro de digitação e foi exclído da análise.
- A coluna **price** indica o preço que o imóvel foi ou será comprado pela House Rocket
- Valores duplicados em **id** foram excluídos da análise
- Condições do imóvel e sua localização foram os faotres decisivos na compra ou não do imóvel.
- A estação do ano foi o padrão decisivo para venda do imóvel.

### 4 - Estratégia para solução do CEO

1. Coleta dos dados do site Keggale
2. Entendimento do negócio da House Rocket
3. Tratamento dos Dados
4. Transformação das variáveis
5. Limpeza dos dados
6. Exploração dos dados
7. Levantamento de hipóteses
8. Validação das hipóteses e insights gerados
9. Conclusão
10. Data viz através do Streamlit

### 5 - Hipóteses relevantes para o negócio

 **Hipóteses** |  **Resultado**  | **Indicação para o negócio**  |
| ------------------- | ------------------- | ------------------- |
|  **H1** - Imóveis com vista para a água são em média 30% mais caros | Verdadeira | Investir em imóveis com vista para água |
|  **H2** - Imóveis com data de construção menor que 1955 são em média 50% mais baratos | Falsa | Investir em imóveis independente da data de construção |
|  **H3** - Imóveis sem porão com maior área total são 40% mais caros | VErdadeira | Investir em imóveis sem porão|
|  **H4** - Imóveis que nunca foram reformados são em média 20% mais baratos | Verdadeira | Investir em imóveis não reformados e reformá-los para venda |
|  **H5** - Imóveis em más condições, mas com boa vista são 10% mais caros | Verdadeira | Não investir em imóveis em más condições| 

O total de lucro onde ( lucro = preço de compra - preço d e venda ) dos imóveis é de **$22.623.548,20**



### 6 - Dashbord entregue ao CEO

Segue o link: 
