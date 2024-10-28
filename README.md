**Fonte dos Dados**

Os dados foram retirados de uma base fictícia gerada pelo Chat GPT, base referente a vendas.
Esses dados oferece uma visão das informações relacionadas a vendas e desempenho em geral de uma empresa fictícia.

O conjunto de dados é composto por 7 colunas e 65535 linhas.
- Data do Pedido 
- Nome do Produto 
- Valor Unitário
- Categoria do Produto
- Fornecedor
- Loja
- UF da Loja

**SQL Server**

O SGBD utilizado para esse projeto foi o Microsoft SQL Server, essa ferramenta é uma excelente opção para manipular dados e oferece recursos avançados, como segurança aprimorada, integração com outras tecnologias e opções de implantação flexíveis. 

**Vendas por Estado (UF da Loja)**

Primeiramente, foram identificados 8 estados com presença de vendas da empresa:
São Paulo (SP), Santa Catarina (SC), Paraná (PR), Rio Grande do Sul (RS), Bahia (BA), Distrito Federal (DF), Minas Gerais (MG) e Rio de Janeiro (RJ).

![image](https://github.com/user-attachments/assets/ff0cffe0-33bb-4fae-8a7f-d59c9abb3413)
![image](https://github.com/user-attachments/assets/8df07972-77ef-4e07-a8da-db7847fcb37a)

Os resultados da análise de vendas por estado (UF da Loja), mostram que o estado de São Paulo (SP) tem o maior percentual de vendas, com 29,89%, seguido por Santa Catarina (SC) com 10,14%. O estado do Rio de Janeiro (RJ) tem o menor percentual de vendas, com 9,87%. Esse resultado é contando todos os anos de 01/2021 à 07/2024.

**Desempenho por Categoria de Produto**

A análise agora foi direcionada para verificar quais categorias de produtos têm o maior volume e vendas, tanto em termos de unidades quanto em valor. 

![image](https://github.com/user-attachments/assets/127d9e66-77b8-47e9-b249-dbc80374a0d4)
![image](https://github.com/user-attachments/assets/abc667aa-c1b1-4a98-9778-f21a1a87cfeb)

Nota-se que em Total_Vendas o produto com maior expressão é o Smartphone com 13228 vendas. E o maior produto em valor vendido é o Laptop com total de R$ 123.785.086,65.

Agora vamos comparar a receita por categoria de produto ao longo do tempo.

![image](https://github.com/user-attachments/assets/6e4517fb-01b9-448b-ab28-f86d1e301cf7)
![image](https://github.com/user-attachments/assets/5dc54487-650d-47a2-b47c-ad6314a6d6db)

Podemos notar que não temos muita diferença na Receita_Total dos produtos entre os anos de 2021 à 2023 e que, apenas em 2024 nota-se um valor menor pois a base só apresenta resultados até 07/2024. Como foi visto na análise de desempenho por categoria, podemos ver que os produtos Smarthpones e Laptops possuem um maior destaque no valor da receita das vendas. 

**Desempenho por Loja**

Agora vamos avaliar quais lojas estão gerando mais receita e volume de vendas.

![image](https://github.com/user-attachments/assets/001feb4e-c690-46ed-a71e-67d3a86603c8)
![image](https://github.com/user-attachments/assets/3c4f738c-d5cd-4bef-b7d5-9a01616e28a3)

O resultado mostra um domínio total pelo estado de São Paulo (SP), onde acumula a maior parte de vendas e, também da receita total.

Podemos ver esse resultado em % do Total de Vendas, segue abaixo:

![image](https://github.com/user-attachments/assets/35c82377-30c8-4001-823a-aa376e27999f)
![image](https://github.com/user-attachments/assets/d2c3ed9d-3056-4657-bbc5-30bc2d3bef29)

São Paulo representa 29,89% de vendas da empresa e com a menor % está Rio de Janeiro (RJ) com 9,87%. Nota-se a região sul com os estados de Santa Catarina (SC), Paraná (PR) e Rio Grande do Sul (RS) com um total de 30,25% das vendas, a empresa é muito forte na região Sul e no estado de São Paulo (SP), pode ser que suas atividades se iniciaram em algum desses estados e está evoluindo para as demais regiões, como Distrito Federal (DF), Minas Gerais (MG) e o Rio de Janeiro (RJ).

Agora comparando o desempenho entre lojas que pertencem à mesma categoria.

![image](https://github.com/user-attachments/assets/38981c1b-b518-4955-a44f-c6f2f2196a0e)
![image](https://github.com/user-attachments/assets/8b2ea82f-22e2-4d0e-aeeb-80063acc59c3)

Notamos que as lojas são homogêneas no quesito de boa performance, todas são bem fortes no ganho com Laptops e Smartphones, não conseguimos ver muita diferença de receita.  

**Análise de Preços**

Verificar a variação dos preços entre diferentes lojas ou estados e identificar possíveis tendências ou disparidades regionais. 

![image](https://github.com/user-attachments/assets/5a6801ff-4756-4ffd-8bf9-5864b30579a1)
![image](https://github.com/user-attachments/assets/62d8b44a-2c0f-47bd-9f32-2887913d5f25)
![image](https://github.com/user-attachments/assets/77ca92df-f8a0-4566-b1ef-f2ea6d5f75b4)

Nota-se que no geral Bahia (BA) apresenta o maior preço médio, porém, esse valor muda no decorrer dos anos: 2021 – Paraná (PR) | 2022 – Santa Catarina (SC) | 2023 – Distrito Federal (DF) | 2024 – Rio Grande do Sul (RS). Por fim, os preços não apresentam tanta disparidade, essas pequenas diferenças podem estar relacionadas com a política de preço de cada região. 

Calculando o ticket médio das vendas por loja e por estado. 

![image](https://github.com/user-attachments/assets/c69d0ab7-eb85-4263-b55b-3713f6ff5832)
![image](https://github.com/user-attachments/assets/f8257c72-064b-4589-b470-8f5df2a4d04c)

A MegaElectro e a ElectroMall frequentemente aparecem com valores de ticket médio mais elevados em comparação com outras lojas, o que pode indicar um posicionamento voltado para produtos de maior valor agregado. A loja Super Tech aparece várias vezes na lista com um ticket médio relativamente mais baixo, sugerindo que essa loja pode estar focada em produtos de menor valor ou em uma estratégia mais acessível ao cliente. 
Em alguns estados, como SP e RJ, há uma variação significativa de ticket médio entre as lojas. Essa variação pode estar ligada ao tipo de produto vendido ou ao público-alvo de cada loja nessas regiões.
O DF apresenta uma tendência regional, com o ticket médio mais alto. Isso pode refletir um mercado mais disposto a adquirir produtos de maior valor agregado. 

**Participação de Mercado por Fornecedor**

Avaliar a participação de mercado de cada fornecedor em termos de quantidade de produtos vendidos e receita gerada.

![image](https://github.com/user-attachments/assets/b0929add-5b6a-4a88-82d8-3bc5f3a09029)
![image](https://github.com/user-attachments/assets/939d17b4-0737-49b7-97d8-27e37a3e0b7c)

O Supplier F lidera em participação na receita total com 13,82% da receita, embora sua quantidade de produtos vendidos seja de apenas 6,72%. Isso sugere que os produtos desse fornecedor possuem um ticket médio mais alto, ou seja, são vendidos a preços mais elevados. 
O Supplier E e D, também têm uma alta participação na receita, mas a participação de ambos na quantidade de produtos vendidos é semelhante (em torno de 6,64%). Isso indica que esses fornecedores estão entre os líderes em vendas.
Os fornecedores J, L e K têm uma participação muito pequena na receita total (cerca de 1,76%). Isso indica que esses fornecedores vendem produtos de ticket médio mais baixo ou produtos mais baratos. 
Com base nessa análise, a empresa pode ajustar o portfólio de fornecedores, favorecendo aqueles que geram maior receita com menor quantidade de vendas, como o Supplier F, e avaliar estratégias de crescimento para fornecedores de produtos mais acessíveis. Também pode ser interessante explorar oportunidades de negociação com fornecedores de alto volume e baixa receita para melhorar as margens ou considerar substituições que possam agregar mais valor. 

**Loja vs. Categoria de Produto**

Verificar quais lojas têm melhor desempenho em diferentes categorias de produtos. Isso pode ajudar a entender o perfil de vendas de cada loja.

![image](https://github.com/user-attachments/assets/92d34f4e-1642-4457-8a07-680a3d7007e3)
![image](https://github.com/user-attachments/assets/037e79a2-ca6f-4ea4-9dad-db2ea65a6b91)

As lojas que vendem Laptops, como a MegaElectro e a Eletrônicos Plus, estão gerando as receitas mais altas, superando os R$ 20 milhões em várias ocasiões. A categoria “Laptops” parece ser a mais rentável, com percentuais de receita entre 16% e 17,5%.
Lojas como Digital World e Super Tech apresentam vendas significativas de smartphones, o que indica uma alta demanda. As receitas dessa categoria também têm uma boa representatividade, ficando em torno de 17%. 
As categorias Smartwatches e Headphones têm as receitas mais baixas entre os produtos analisados, geralmente com percentuais de receita em torno de 16%. Isso sugere que essas categorias podem não ter tanta demanda ou poderiam se beneficiar de promoções ou outras estratégias para aumentar o volume de vendas. 
As lojas MegaElectro, Eletrônicos Plus e Digital World são as lojas com melhores receitas totais. Investir em estoque ou estratégias de marketing nessas lojas para produtos de alto desempenho pode potencializar o crescimento. 

**Muito obrigado por ler meu projeto.**




