# Desafio Alura Store

## 🎯 Objetivo
Ajudar o Senhor João a decidir qual loja da rede Alura Store vender para iniciar um novo empreendimento.  
Analisar dados de vendas, desempenho e avaliações das 4 lojas fictícias e recomendar a loja com menor eficiência.

---

## 🗂️ Etapas da Análise
1. Importação de dados  
2. Verificação e limpeza de valores nulos  
3. Análise e gráfico de faturamento   
4. Análise e gráficos das Vendas por categoria  
5. Análise e gráfico das Médias de Avaliações das lojas  
6. Produtos mais vendidos  
7. Produtos menos vendidos  
8. Análise e gráfico do Custo Médio do Frete por loja  
9. Gráfico do frete  
10. Relatório final  

---

## 📊 Faturamento
Para a análise do Faturamento são importadas as listas ***lojas e nomes***, também é criada uma lista chamada ***faturamentos*** para armazenar os dados obtidos e um dicionário chamado ***dfs_faturamento***.

O programa se dá por um laço *for* que percorre o banco de dados de cada loja e realiza a soma da coluna **'Preço'**, retornando a ***soma*** de todos os itens da coluna. É criado um data frame com a lista completa chamado ***df_faturamento***, que é exibido na tela, e um individualizado chamado ***dfs_faturamento[(nome da loja)]***, onde será retornado a qualquer momento o resultado individualizado de cada loja.

Gráfico: barras verticais comparando faturamento.

---

## 🛍️ Vendas por Categoria
Para a análise das Vendas por Categoria são importadas as listas ***lojas e nomes*** e também é criado um dicionário chamado ***dfs_categorias***.

O programa se dá por um laço *for* que percorre o banco de dados de cada loja, realiza a consulta na coluna ***'Categoria de Produtos'***, armazena cada nome exclusivo e sua respectiva quantidade em forma de tabela além da quantidade total de vendas. É criado um data frame com a lista completa indicando cada categoria de produto chamado ***df_categorias***, que é exibido na tela, e um individualizado chamado ***dfs_categorias[(nome da loja)]***, onde será retornado a qualquer momento a lista individualizada de cada loja.

Gráfico: pizza indicando a porcentagem de vendas de cada categoria.

---

## ⭐ Média de Avaliação das Lojas
Para a análise da Média de Avaliação das Lojas são importadas as listas ***lojas e nomes***, também é criada uma lista chamada ***medias*** para armazenar os dados obtidos e um dicionário chamado ***dfs_medias***.

O programa se dá por um laço *for* que percorre o banco de dados de cada loja, realiza a soma da coluna ***'Avaliação da compra'*** e depois a divisão pela quantidade de itens totais da coluna, retornando a ***média*** da coluna. É criado um data frame com a lista completa chamado ***df_medias*** e um individualizado chamado ***dfs_medias[(nome da loja)]***, onde será retornado a qualquer momento o resultado individualizado de cada loja.

Gráfico: linha comparando média de avaliação.

---

## 🔝 Produtos Mais Vendidos
Para a análise dos Produtos Mais Vendidos são importadas as listas ***lojas e nomes*** e também é criado um dicionário chamado ***dfs_mais_vendidos***.

O programa se dá por um laço *for* que percorre o banco de dados de cada loja e realiza a consulta na coluna ***'Produto'*** parametrizado a 10 ***(head(10))***, retornando os ***10 itens que mais aparecem na coluna***. É criado um data frame com a lista completa, chamado ***df_mais_vendidos*** e um individualizado chamado ***dfs_mais_vendidos[(nome da loja)]***, onde será retornado a qualquer momento a lista individualizada de cada loja.

---

## 🔽 Produtos Menos Vendidos
Para a análise dos Produtos Menos Vendidos são importadas as listas ***lojas e nomes*** e também criado um dicionário chamado ***dfs_menos_vendidos***.

O programa se dá por um laço *for* que percorre o banco de dados de cada loja e realiza a consulta na coluna ***'Produto'*** parametrizado a 10 ***(nsmallest(10))***, retornando os ***10 itens que menos aparecem na coluna***. É criado um data frame com a lista completa, chamado ***df_menos_vendidos*** e um individualizado chamado ***dfs_menos_vendidos[(nome da loja)]***, onde será retornado a qualquer momento a lista individualizada de cada loja.

---

### 🚚 Frete Médio
Para a análise do Valor Médio do Frete por Loja são importadas as listas ***lojas e nomes***, também é criada uma lista chamada ***fretes*** para armazenar os dados obtidos e um dicionário chamado ***dfs_fretes***.

O programa se dá por um laço *for* que percorre o banco de dados de cada loja e realiza a soma da coluna ***'Frete'*** e depois a divisão pela quantidade de itens totais da coluna, retornando a ***média da coluna***. É criado um data frame com a lista completa, chamado ***df_fretes*** e um individualizado chamado ***dfs_fretes[(nome da loja)]***, onde será retornado a qualquer momento o resultado individualizado de cada loja.

Gráfico: barras horizontais comparando frete médio.

---

## 📝 Relatório Final
Após a coleta dos dados obtidos, é feita uma análise referente aos resultados obtidos em cada tópico do projeto e feita a sugestão de escolha da venda de uma das 4 lojas.
