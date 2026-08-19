# REVISÃO DE SQL

## FUNDAMENTOS DE SQL

### O que é SQL?

- **SQL (Structured Query Language)** é a linguagem padrão para interagir, acessar e manipular bancos de dados relacionais.
- É uma linguagem declarativa: você descreve qual resultado deseja.

### O que é PostgreSQL?
O **PostgreSQL** é o **SGBD (Sistema Gerenciador de Banco de Dados)**, responsável por decidir o como e por elaborar o plano físico de execução mais eficiente para sua consulta.

### DDL - Data Definition Language

O **DDL** é o conjunto de comandos SQL responsável por criar, modificar e remover estruturas do banco de dados. 
Ele não interage diretamente com os dados, apenas com a sua organização, definindo as estruturas.

| Comandos | Descrição | Sintaxe |
|:---:|---|:---:|
| CREATE TABLE | Cria uma nova tabela | CREATE TABLE table_name(column1 data_type, column2 data_type) |
| ALTER TABLE | Modifica uma tabela existente | ALTER TABLE table_name ADD COLUMN column_name data_type; |
| DROP TABLE | Remove uma tabela | DROP TABLE table_name; |
| CREATE INDEX | Cria índices para performance | CREATE INDEX idx_name ON table_name(column_name); |
| TRUNCATE | Remove todos os registros da tabela | TRUNCATE TABLE table_name; |
| COMMENT | Adiciona comentários ao dicionário de dados | COMMENT ON TABLE table_name IS 'comment_text'; |
| RENAME | Renomeia um objeto existente no banco de dados | RENAME TABLE old_table_name TO new_table_name; |

### DML - Data Manipulation Language

O **DML** é um conjunto de comandos que inserem, alteram e removem registros dentro das estruturas definidas pelo DDL. Aqui os dados de fato existem e são modificados.

| Comandos | Descrição | Sintaxe |
|:---:|---|:---:|
| INSERT INTO | Insere novos registros | INSERT INTO table_name (column1, column2,...) VALUES (value1, value2,…) |
| UPDATE | Altera registros existentes | ALTER TABLE table_name ADD COLUMN column_name data_type; |
| DELETE | Remove registros | DROP TABLE table_name; |

### DQL - Data Query Language

O **DQL** é um conjunto de comandos de consulta de dados.

| Comandos | Descrição | Sintaxe |
|:---:|---|:---:|
| SELECT | Define quais colunas serão exibidas | SELECT column1, column2… FROM table_name WHERE condition; |
| FROM | Indica qual a tabela dos registros a serem exibidos | SELECT column1, column2… FROM table_name; |
| WHERE | Filtra quais linhas antes de qualquer agrupamento ou agregação | SELECT column1 FROM table_name WHERE condition; |
| GROUP BY | Grupo de linhas com os mesmos valores nas colunas especificadas | SELECT column1, column2 FROM table_name GROUP BY column2; |
| HAVING | Filtra os resultados de GROUP BY | SELECT column1, column2 FROM table_name GROUP BY column2 HAVING condition; |
| DISTINCT | Remove registros duplicados | SELECT DISTINCT column1, column2,... FROM table_name; |
| ORDER BY | Ordena os resultados | SELECT column1 FROM table_name ORDER BY column1 [ASC | DESC]; |
| LIMIT | Restringe o número de linhas retornadas no SELECT | SELECT * FROM table_name LIMIT number; |



















