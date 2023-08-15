<!-- Imagem redimensionada -->
<img src="https://digitalcollege.com.br/wp-content/webp-express/webp-images/uploads/2022/05/logo-digital.png.webp" alt="texto alt" width="300">



# Projeto: Criando um Banco de Locação de Veículos com PostgreSQL - Usando o PENTAHO

O projeto tem como desafio criar um Banco de Dados Dimensional, usando a transformação ETL de um arquivo CSV no Pentaho, criando tabelas de dimensão e fato, e obtendo com sucesso um output para o banco de dados Postgres. 💼🔗


## 🚀 Começando

Neste projeto, realizamos a criação de um banco de dados db_locacao_nayara, sendo essa a basse de todo o projeto.

> **Foi dividida a análise em 4 etapas:**

1. **Análise do Arquivo CSV**: Nesta etapa, analisamos o arquivo CSV recebido, para entender os dados a serem análisados e fazer a separação das dimensões e fato.

2. **Modelagem, Tratamento e Criação das Tabelas no Pentaho**: Nesta etapa, criamos 6 modelagens para tratamento e criação das tabelas no Postgres:
dim_cliente, dim_combustivel, dim_carro, dim_vendedor, dim_data, fato_locacao.

Na modelagem utilizamos:

-**Value Mapper:** O "Value Mapper" é uma etapa do fluxo de trabalho no Pentaho que permite mapear valores de uma coluna para outros valores específicos. Isso é útil para transformar dados em categorias ou codificar valores de acordo com um padrão desejado. Nesse projeto utilizamos para tratar o id_carro, id_vendedor e criar a descrição da semana e do mês.

-**Select Values:** A etapa "Select Values" é usada para selecionar colunas específicas de um conjunto de dados. Ela permite que você escolha quais colunas deseja manter no fluxo de trabalho, descartando as que não são necessárias para a análise ou transformação. Além da escolha das colunas usamos meta-data para alterar o tipo de algumas colunas.

-**Sort Rows:** A etapa "Sort Rows" é usada para ordenar os registros de um conjunto de dados com base nos valores de uma ou mais colunas. Isso é útil quando você deseja ter os dados organizados em uma ordem específica antes de realizar outras operações ou análises.

-**Unique Rows:** A etapa "Unique Rows" é usada para eliminar registros duplicados de um conjunto de dados. Ela garante que apenas uma instância de cada combinação única de valores nas colunas selecionadas seja mantida, reduzindo redundâncias nos dados.

-**Table Output:** A etapa "Table Output" é usada para enviar os resultados do fluxo de trabalho do Pentaho para uma tabela de banco de dados. Isso permite que os dados transformados ou processados sejam inseridos, atualizados ou substituídos em uma tabela específica do banco de dados. Nesse projeto inserimos as tabelas em um banco de dados dimensional no Postgres.


## 🚀 INSIGHTS

> Nessa etapa usamos o POWERBI para apresentar alguns insights das locações, clientes e vendedores.

-**Total de Locações por Cidade Cliente**.

-**Receita por Cliente**.

-**Faturamento por Estado** (Bolha Mapa).

-**Total de Faturamento por Marca de Carro**.

-**Total de Faturamento por Modelo de Carro**.

-**Media de Quilometragem por Modelo de Carro**.

-**Media de Quilometragem por Tipo de Combustivel**.

-**Total de Vendas por Vendedor**.

-**Total de Locações por Vendedor**.

-**Total de Faturamento por Carro e Vendedor**.

-**Quantidade de Vendedor**.

-**Quantidade de Carros**.

-**Quantidade de Clientes**.

-**Quantidade de Locações**.

-**Total Faturamento**.

-**Filtros por Data**.

-**Filtros por Vendedor**.

-**Filtros por Estado**.

-**Filtros por Sexo Vendedor**.

-**Filtros por Modelo Carro**.

-**Filtros por Estado**.

-**Filtros por Cidade**.

-**Filtros por Cliente**.



## 🚀 **Resultado de Algumas Análises**


-Rio Branco é a Cidade com Menor Faturamento.

-Nissan é a marca mais escolhida pelos clientes.

-Combustivel mais utilizado é a Gasolina.

-Fiat 147 foi o carro que teve o maior deslocamento (quilometragem).

-Vendedor Dezesseis é o que tem o maior número de vendas.

-Ano de 2019 e 2021 não teve faturamento ou não teve a coleta correta dos dados.


> **Para visualizar o dashboard do projeto, acessar o link abaixo:**

https://app.powerbi.com/view?r=eyJrIjoiYjUwOGQ0MzctYTI0My00MjU5LWI2M2EtOTQwOGFjM2IwM2NiIiwidCI6ImJkMWMxZTAzLTU2MDMtNDUzNy04ODY5LWQ5ZGQyYzRiMjc2MiJ9


## ⚙️ Arquivos no Repositório:

-**Pbix com os Insights**.

-**Arquivo .ktr do Pentaho**.

-**Arquivo CSV da base de Dados**.



## 🎁 Expressões de gratidão

* Compartilhe com outras pessoas esse projeto 📢;
* Quer saber mais sobre o projeto? Entre em contato para tomarmos um :coffee:;

---
⌨️ com ❤️ por [Nayara Vakevskii](https://github.com/NayaraWakewski) 😊
