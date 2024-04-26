### INSERT, UPDATE e DELETE + WHERE

1. INSERT INTO
```sql
INSET INTO produtos (nome, preco) VALUES ('teclado gmk67', 170);
```
- insere na tebela produtos, um produto com os dados
  - nome = "teclado gmk67"
  - preco = 170
  - id = *foi definido com chave primária e é gerado via autoincrement*

---

2. UPDATE + WHERE

```sql
UPDATE produtos SET 
        nome = 'base teclado gmk67',
        preco = 185.80
    WHERE id = 1;
```
- altera o valor de nome para 'base teclado gmk67'
- altera o valor de preco para 185.80
- atualiza todos os dados da tabela que possuem id = 1
- **SEMPRE USAR WHERE!!!**
---

3. DELETE FROM + WHERE
```sql
DELETE  FROM produtos WHERE id = 2;
```
- deleta todos os dados da tabela que possuem id = 2
- **SEMPRE USAR WHERE!!!**