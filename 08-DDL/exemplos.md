### CREATE, ALTER, DROP

1. CREATE DATABASE

```sql
CREATE DATABASE projeto_estoque;
```
- cria um banco de dados com o nome "projeto_estoque"

---

2. CREATE TABLE

```sql
CREATE TABLE produtos (id INT PRIMARY KEY, nome VARCHAR(50), preco DECIMAL(8,2));
```
- cria uma tabela com o nome "produtos"
- cria os campos :
  - id - inteiro e chave primária
  - nome - texto (caracteres variados) com máximo de 50 caracteres
  - preco - numero decimal com até 8 dígitos antes da vírgula e até 2 depois da vírgula
- isso cria uma tabela no banco de dados criado no comando anterior e disponibiliza a tabela criada agora para inserção de dados

---

3. ALTER TABLE

```sql
CREATE TABLE produtos ADD preco_com_desconto DECIMAL(8,2));
```
- adiciona na tabela produtos o campo:
  - preco - numero decimal com até 8 dígitos antes da vírgula e até 2 depois da vírgula
---

3. DROP TABLE

```sql
CREATE TABLE produtos;
```
- apaga a tabela "produtos" e todos os seus dados
---

4. DROP DATABASE

```sql
CREATE DATABASE projeto_estoque;
```
- apaga o banco de dados "projeto_estoque"
---