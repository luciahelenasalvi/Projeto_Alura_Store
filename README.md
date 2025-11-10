# Descrição do projeto "Alura Store"

### Visão Geral
Trata-se de um projeto de análise de dados. A Alura Store é uma rede com 4 lojas de propriedade do Sr. João. A partir das análises dos dados fornecidos, será recomendada a venda de uma das unidades. 

### Dados
Foram fornecidos quatro arquivos, via link, referentes às vendas de cada loja. Os dados abarcam o período de 2020-2022 e o primeiro trimestre de 2023. 

Cada arquivo contém 12 colunas, a saber:

| Nome da Coluna | Conteúdo | Tipo de dado |
| ---------------------- | ---------------------- | ---------------------- |
|  **Produto**   | Nome do produto disponível para venda [Ex. Mesa de Jantar]   | String[Texto]  |
|  **Categoria do Produto**   | Nome das categorias dos produtos disponíveis para venda [Móveis, Eletrônicos]   | String[Texto]  |
|  **Preço**   | Preço dos produtos disponíveis para venda    | Float[Decimal]  |
|  **Frete**   | Frete dos produtos disponíveis para venda   | Float[Decimal]  |
|  **Vendedor**   | Nome do vendedor responsável pela venda | String[Texto]  |
|  **Local da compra**   | Sigla da Unidade Federativa do local de compra [SP, PR]   | String[Texto]  |
|  **Avaliação da compra**   | Nota do cliente para a compra [1, 2, 3, 4, 5]   | Int[Número inteiro]  |
|  **Tipo de pagamento**   | Nome das opções de pagamento que a rede aceita [cartão de crédito, boletos, cupom, cartão de débito]   | String[Texto]  |
|  **Quantidade de parcelas**   | Número de parcelas disponíveis para pagamento [1 - 24]   | Int[Número inteiro]  |
|  **lat**   | Latitude do local de compra    | Float[Decimal]  |
|  **lon**   | Longitude do local de compra   | Float[Decimal]  |

#### Formato dos arquivos

| Unidade | Colunas | Linhas|
| ---------------------- | ---------------------- | ---------------------- |
| **Loja 1**| 12 | 2359 |
| **Loja 2**| 12 | 2359 |
| **Loja 3**| 12 | 2359 |
| **Loja 4**| 12 | 2358 |
| **Total**| - | 9435 |

## Métricas
A análise considerará as seguintes métricas:
*   Faturamento total das lojas
*   Categorias de produtos mais e menos vendidas
*   Média das avaliações de clientes por loja
*   Produtos mais e menos vendidos
*   Frete médio de cada loja

## Procedimentos iniciais
Desenvolvimento realizado na linguagem Python, utilizando a biblioteca Pandas e Matplotlib. Os códigos foram escritos e executados na plataforma online Google Colab, assim como o relatório final. 

*Passos iniciais*: 
* Importação e leitura dos dados
* Visualização de amostra dos dados (funções head/tail)

*Reconhecimento dos dados*
* Número de linhas e colunas (funçõesshape/len)
* Avaliação de nulos (função info): Pela interferência negativa que podem causar, é preciso fazer o tratamento de dados nulos
* Verificações da frequência de cada valor por coluna (função value_counts); contagem, número de valores únicos, mais frequentes, frequência do mais frequente (função describe)
* Verificação do meses de 2023 (set : identifica valores únicos)
* Frequência, média, desvio padrão, valor mínimo e máximo e quartis (função describe aplicada ao dataframe)
* Agrupamentos (groupby) e seleções (query)

## Análises ##
⦁	Faturamento total
⦁	Faturamento por loja e ano
⦁	Número de vendas por loja e ano
⦁	Ticket médio por loja e ano
* Categorias de produtos
* Vendas por categoria
* Faturamento por loja das categorias mais vendidas
* Percentual das categorias mais vendidas 
* Média de avaliação das lojas
* Média geral
* Distribuição das notas
* 10 produtos mais vendidos
* 10 produtos menos vendidos
* Frete médio por loja
* Frete máximo por loja
* Frete mínimo por loja
* Frete mínimo sem casos de frete gratuito por loja
* Frequência do frete gratuito
* Percentual do frete gratuito
* Frete médio sem frete gratuito por loja

### Como executar o notebook
* Faça o download do arquivo. 
* Abra o Google Colab. 
* Faça o upload do arquivo. 
No menu "Ambiente de Execução" >> Executar tudo ou Ctrl + F9

Neste repositório há dois arquivos notebook: AluraStoreBr.ipynb e Relatorio_AluraStoreBr.ipynb. O primeiro arquivo contém as verificações e, ao final, o relatório. No intuito de facilitar a visualização do relatório, foi criado o segundo arquivo, que é dedicado à ele. 

### Insights
O primeiro passo para ter ideias sobre os padrões, é preciso conhecer os dados. Por isso, na exploração inicial, foi possível descobrir a amplitude temporal (por exemplo, que o ano de 2023 continha dados apenas do primeiro trimestre), correlação de preço e frete, e como se comportaram as vendas, o faturamento e o ticket médio durante os anos. 

Foram criados gráficos utilizando a biblioteca Matplotlib: Gráficos de barras, gráficos de linhas, gráfico de pizza, violin plot, mapa de calor.

Desenvolvido por Lúcia Helena Aparecida Rissi Salvi  - Módulo I Data Science Oracle Next Education | G9.







