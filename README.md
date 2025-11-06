# Descrição do projeto "Alura Store"

### Visão Geral
Este é um projeto de análise de dados de vendas de 4 lojas que constituem a rede Alura Store: uma das lojas deverá ser vendida e as análises possibilitarão concluir qual deve ser indicada. 

Desenvolvido por Lúcia Helena Aparecida Rissi Salvi  - Módulo I Data Science Oracle Next Education | G9.

### Dados
Foram recebidos quatro links de arquivos. Cada arquivo, referente à uma das lojas, tras os dados de vendas no período de 2020-2022 e o primeiro trimestre de 2023. 

Cada arquivo contém 12 colunas, a saber:
1. **Produto**: nome do produto disponível para venda, como "Mesa de jantar", do tipo String (object).
2. **Categoria do Produto**: nome das categorias de produtos, tais como: móveis, eletrônicos, brinquedos, eletrodomésticos, esporte e lazer, instrumentos musicais, livros e utilidades domésticas, do tipo String. 
3. **Preço**: preço do produto, em ponto flutuante (float).
4. **Frete**: frete do produto, em ponto flutuante (float)
5. **Data da compra**: data da aquisição do produto, em string, no formato dd/mm/aaaa. 
6. **Vendedor**: nome do vendedor, em string.
7. **Local da compra**: Unidade federativa do local da compra, tais como SP, PR, string.
8. **Avaliação da compra**: nota do cliente para a compra, numero inteiro.
9. **Tipo de pagamento**: opções de pagamento que a rede de lojas oferece, cartão de crédito, boletos, cupom e cartão de débito. string.
10. **Quantidade de parcelas**: número de parcelas, numero inteiro.
11. **lat**: Latitude - medidas geolocalização float
12. **lon**: Longitude

#### Formato dos arquivos
A loja 1 possui uma base de dados com 12 colunas e 2359 vendas (linhas)
A loja 2 possui uma base de dados com 12 colunas e 2359 vendas (linhas)
A loja 3 possui uma base de dados com 12 colunas e 2359 vendas (linhas)
A loja 4 possui uma base de dados com 12 colunas e 2358 vendas (linhas)



## Métricas
Foram solicitadas a análises das métricas: 

*   Faturamento total das lojas
*   Categorias de produtos mais e menos vendidas
*   Média das avaliações de clientes por loja
*   Produtos mais e menos vendidos
*   Frete médio de cada loja

## Procedimentos aplicados
O desenvolvimento do notebook (Google Colab) foi realizado na linguagem Python, utilizando a biblioteca Pandas - para análise -  e Matplotlib - para criação de gráficos. 

*Passos iniciais*: 
* Importação e leitura dos dados
* Visualização de amostra dos dados (funções head/tail)

*Reconhecimento dos dados*
* Número de linhas e colunas (funçõesshape/len)
* Avaliação de nulos (função info): Pela interferência negativa que podem causar, é preciso fazer o tratamento de dados nulos
* Verificações da frequencia de cada valor por coluna (função value_counts); contagem, número de valores únicos, mais frequentes, frequencia do mais frequente (função describe)
* Verificação do meses de 2023 (set : identifica valores únicos)
* Frequencia, média, desvio padrão, valor mínimo e máximo e quartis (função describe aplicada ao dataframe)
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





