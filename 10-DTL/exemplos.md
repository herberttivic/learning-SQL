## BEGIN (ou START TRANSACTION), COMMIT, ROLLBACK

1. BEGIN + COMMIT
```sql
CREATE TABLE categorias (id INT PRIMARY KEY, nome VARCHAR(50));
BEGIN TRANSACTION;
      INSERT INTO categorias VALUES (1, "eletronicos");
      INSERT INTO categorias VALUES (2, "domésticos");
COMMIT;
```
- cria uma tabela categorias com id e nome
- inicia uma transaction
- insere dois itens na tabela
- sobe as alterações com o COMMIT
---

2. BEGIN + ROLLBACK
```sql
CREATE TABLE categorias (id INT PRIMARY KEY, nome VARCHAR(50));
BEGIN TRANSACTION;
INSERT INTO categorias VALUES (1, "eletronicos");
INSERT INTO categorias VALUES (1, "eletronicos");
ROLLBACK ;
```
- cria uma tabela categorias com id e nome
- inicia uma transaction
- insere dois itens na tabela
- descarta as alterações com o ROLLBACK
