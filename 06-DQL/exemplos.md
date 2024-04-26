### SELECT e ALIAS(AS)

1. SELECT ALL
```sql
SELECT * FROM produtos;
```
- devolve todos (*) os dados de todos os itens da tabela "produtos"

---

2. SELECT ONLY

```sql
SELECT id,nome,preco FROM produtos;
```
- devolve somente id, nome e preço de todos os itens da tabela "produtos"

---

3. ALIAS (apelido)

```sql
SELECT prod.id AS codigo, prod.nome AS nome_poduto ,prod.preco AS preco_produto FROM produtos AS prod;
```

- define o nome da tabela busca chamando a tabela "produtos" pelo nome de "prod"
- usa o apelido "prod" para selecionar as colunas da tabela "produtos"\
- renomeia os campos (somente para essa consulta)