Explorando Dados de Vendas e Clientes: Criando KPIs Essenciais para o Varejo 

Objetivos:
Departamentos mais vendidos
Média de preço com frete por departamento
Quantidade de vendas por mês
Média de renda por canal de vendas
Média de idade dos clientes por bandeira
Premissas:
Erro de sistema: para compras sem UF, atribuir MS.
Validação de preços: O preço sem frete não pode ser maior que o preço com frete.

Etapas do Processo
1. Carregamento e Visualização dos Dados
O primeiro passo foi carregar as bases de dados de vendas e clientes usando Pandas. As funções head() e info() foram utilizadas para inspecionar a estrutura dos dados e garantir que as colunas estavam corretamente formatadas. Dados ausentes e inconsistências também foram identificados nesta etapa.

2. Limpeza e Tratamento dos Dados
Em seguida, foi feita a limpeza e tratamento das duas bases. As colunas que continham valores nulos, como o estado das compras, foram preenchidas com o valor padrão "MS", conforme as premissas do projeto. Além disso, corrigimos erros onde o preço do produto era maior que o preço com frete, e as colunas de preços passaram por tratamento para garantir que estavam prontas para análise.

3. Criação de Métricas e KPIs
Com os dados tratados, várias métricas foram geradas:

Departamentos mais vendidos: O agrupamento foi feito por departamento para identificar os mais vendidos.
Média de preço com frete por departamento: Calculamos a média de preços para cada departamento após o tratamento dos dados.
Vendas por mês: Extraímos a informação de mês a partir da data de venda para analisar o comportamento ao longo do tempo.
Renda média por canal de vendas: Unimos as bases de vendas e clientes para calcular a média de renda por canal de vendas.
Idade média dos clientes por bandeira de vendas: Realizamos o mesmo processo para identificar a média de idade dos clientes por bandeira de venda.
4. Visualização dos Resultados
Utilizamos as bibliotecas Matplotlib e Plotly para criar gráficos de barras e linhas que facilitam a interpretação dos KPIs gerados. Por exemplo, gráficos que mostram a média de idade por bandeira de vendas, a renda média por canal de vendas e a quantidade de vendas por mês foram essenciais para visualizar tendências e padrões nos dados.

5. Análise Final
Finalmente, fizemos uma análise das correlações entre as variáveis de vendas e clientes, verificando se os departamentos mais vendidos estavam alinhados com os canais de vendas mais lucrativos. Essa análise foi crucial para a tomada de decisões estratégicas, ajudando a identificar quais departamentos e canais merecem mais atenção para maximizar as vendas.

Ferramentas e Bibliotecas Utilizadas
Pandas: Manipulação e tratamento de dados.
NumPy: Cálculos numéricos eficientes.
Matplotlib: Criação de gráficos e visualizações estáticas.
Seaborn: Visualizações avançadas para análise de dados.
Plotly: Gráficos interativos e dinâmicos para facilitar a exploração dos dados.
